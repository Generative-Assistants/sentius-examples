# Dialog Sessions

## Creating or retrieving a session

Each time you chat with Browser Agent, your message is attached to one of the dialog sessions.

You start with either getting an active session

=== "Curl"

    ```bash
    curl -X GET "https://api.sentius.ai/dialog_sessions?api_key=your_api_key" \
         -H "Content-Type: application/json"
    ```

=== "Python"

    ```python
    import requests
    
    url = "https://api.sentius.ai/dialog_sessions"
    params = {"api_key": "your_api_key"}
    response = requests.get(url, params=params)
    print(response.json())
    ```

or creating a new one

=== "Curl"

    ```bash
    curl -X POST "https://api.sentius.ai/dialog_sessions?api_key=your_api_key" \
         -H "Content-Type: application/json"
    ```

=== "Python"

    ```python
    import requests
    
    url = "https://api.sentius.ai/dialog_sessions"
    params = {"api_key": "your_api_key"}
    response = requests.post(url, params=params)
    print(response.json())
    ```



Either way you will receive a response containing your session `id`, e.g. `1337`.
Using this `id` value in the url, you can now interact with the session.


## Sending messages

=== "Curl"

    ```bash
    curl -X POST "https://api.sentius.ai/dialog_sessions/1337/chat?api_key=your_api_key" \
         -H "Content-Type: application/json" \
         -d '{
           "text": "Hello, world!"
         }'
    ```

=== "Python"

    ```python
    import requests
    
    url = f"https://api.sentius.ai/dialog_sessions/1337/chat"
    params = {"api_key": "your_api_key"}
    data = {"text": "Hello, world!"}
    response = requests.post(url, json=data, params=params)
    print(response.json())
    ```


## Retrieving session history

=== "Curl"

    ```bash
    curl -X GET "https://api.sentius.ai/dialog_sessions/{dialog_session_id}/history?api_key=your_api_key" \
         -H "Content-Type: application/json"
    ```

=== "Python"

    ```python
    import requests
    
    url = f"https://api.sentius.ai/dialog_sessions/{{dialog_session_id}}/history"
    params = {"api_key": "your_api_key"}
    response = requests.get(url, params=params)
    print(response.json())
    ```
