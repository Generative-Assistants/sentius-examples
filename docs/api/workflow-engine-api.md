# Workflow Engine API

## Creating workflows

### Pre-requisites

We assume you have already created a dialog session and have an active session `id`. If not, please refer to the
[Dialog Sessions API](dialog-sessions.md) section.

### Workflow configuration

TODO: Add workflow configuration details

### Submitting a workflow

=== "Curl"

    ```bash
    curl -X POST "https://api.sentius.ai/dialog_sessions/{dialog_session_id}/workflows?api_key=<YOUR_API_KEY>" \
            -H "Content-Type: application/json"
            -d '{
                "config": <YOUR_WORKFLOW_CONFIG>
            }'
    ```

=== "Python"
    
        ```python
        import requests
    
        url = f"https://api.sentius.ai/dialog_sessions/{dialog_session_id}/workflows"
        params = {"api_key": "your_api_key"}
        response = requests.post(url, params=params, json={"config": <YOUR_WORKFLOW_CONFIG>})
        ```

### Using submitted workflow

=== "Curl"

    ```bash
    curl -X POST "https://api.sentius.ai/dialog_sessions/{dialog_session_id}/workflows/run?api_key=<YOUR_API_KEY" \
            -H "Content-Type: application/json"
            -d '{
                "data": <YOUR_DATA>
            }'
    ```

=== "Python"
    
        ```python
        import requests
    
        url = f"https://api.sentius.ai/dialog_sessions/{dialog_session_id}/workflows/run"
        params = {"api_key": "your_api_key"}
        response = requests.post(url, params=params, json={"data": <YOUR_DATA>})
        ```
