# Overview

Sentius API requires an API key and appropriate permissions.
Your API key must be added as a query parameter alongside every request.

```shell
curl -X 'GET' \
  'https://api.sentius.ai/dialog_sessions?api_key=y0urAPIkey' \
  -H 'accept: application/json'
```

We currently support a limited set of Browser Agent actions via API.
