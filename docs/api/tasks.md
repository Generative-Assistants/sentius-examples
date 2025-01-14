# Tasks and instructions APIs

## Creating instructions

=== "Curl"

    ```bash
    curl -X POST "https://api.sentius.ai/tasks/instructions?api_key=your_api_key" \
         -H "Content-Type: application/json" \
         -d '{
           "request": "example_request",
           "web_url": "https://example.com",
           "snippets": []
         }'
    ```

=== "Python"

    ```python
    import requests
    
    url = "https://api.sentius.ai/tasks/instructions"
    params = {"api_key": "your_api_key"}
    data = {
        "request": "example_request",
        "web_url": "https://example.com",
        "snippets": []
    }
    response = requests.post(url, json=data, params=params)
    print(response.json())
    ```


## Retrieving instructions

### Personal

=== "Curl"

    ```bash
    curl -X GET "https://api.sentius.ai/tasks/instructions?api_key=your_api_key" \
         -H "Content-Type: application/json"
    ```

=== "Python"

    ```python
    import requests
    
    url = "https://api.sentius.ai/tasks/instructions"
    params = {"api_key": "your_api_key"}
    response = requests.get(url, params=params)
    print(response.json())
    ```

### Common


=== "Curl"

    ```bash
    curl -X GET "https://api.sentius.ai/tasks/instructions/common?api_key=your_api_key" \
         -H "Content-Type: application/json"
    ```

=== "Python"

    ```python
    import requests
    
    url = "https://api.sentius.ai/tasks/instructions/common"
    params = {"api_key": "your_api_key"}
    response = requests.get(url, params=params)
    print(response.json())
    ```

### All


=== "Curl"

    ```bash
    curl -X GET "https://api.sentius.ai/tasks/instructions/all?api_key=your_api_key" \
         -H "Content-Type: application/json"
    ```

=== "Python"

    ```python
    import requests
    
    url = "https://api.sentius.ai/tasks/instructions/all"
    params = {"api_key": "your_api_key"}
    response = requests.get(url, params=params)
    print(response.json())
    ```


## Deleting instructions

Assuming your instruction `id` is `258`

=== "Curl"

    ```bash
    curl -X DELETE "https://api.example.com/tasks/instructions/258?api_key=your_api_key" \
         -H "Content-Type: application/json"
    ```

=== "Python"

    ```python
    import requests
    
    url = f"https://api.example.com/tasks/instructions/258"
    params = {"api_key": "your_api_key"}
    response = requests.delete(url, params=params)
    print(response.status_code)
    ```
