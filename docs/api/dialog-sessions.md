# Dialog Sessions

Each time you chat with Browser Agent, your message is attached to one of the dialog sessions.

You start with either getting an active session
```shell
curl -X 'GET' \
  'https://api.sentius.ai/dialog_sessions?api_key=y0urAPIkey' \
  -H 'accept: application/json'
```

or creating a new one
```shell
curl -X 'POST' \
  'https://api.sentius.ai/dialog_sessions?api_key=y0urAPIkey' \
  -H 'accept: application/json' \
  -d ''
```

Either way you will receive a response containing your session `id`, e.g. `1337`.
Using this `id` value in the url, you can send a chat message
```shell
curl -X 'POST' \
  'https://api.sentius.ai/dialog_sessions/1337/chat?api_key=y0urAPIkey' \
  -H 'accept: application/json' \
  -H 'Content-Type: application/json' \
  -d '{
  "text": "Find me a plane ticket from Seattle to Vegas"
}'
```

retrieve session history
```shell
curl -X 'GET' \
  'https://api.sentius.ai/dialog_sessions/1337/history?api_key=y0urAPIkey' \
  -H 'accept: application/json'
```
