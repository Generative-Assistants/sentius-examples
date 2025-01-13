# Overview

Sentius API requires an API key and appropriate permissions.
Your API key must be added as a query parameter alongside every request.

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

We currently support a limited set of Browser Agent actions via API.

# Browser Agent API
Visit [Browser Agent API](api/browser-agent-api.md) section to learn how to integration **browser agent** directly into your applications.

# Workflow Engine API
Coming soon.