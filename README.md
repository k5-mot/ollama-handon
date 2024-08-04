# Ollama Handon

## :scroll: Manual

```bash
docker compose up -d
docker exec -it ollama /bin/bash -c /root/ollama/setup.sh
```

## :bulb: VSCode Extensions "Continue"

```json:config.json
{
    // ...
    "models": [
        {
            "title": "Ollama",
            "provider": "ollama",
            "model": "AUTODETECT",
            "apiBase": "http://localhost:11434/"
        }
    ],
    "tabAutocompleteModel": {
        "title": "deepseek-coder-v2:16b",
        "provider": "ollama",
        "model": "deepseek-coder-v2:16b",
        "apiBase": "http://localhost:11434/"
    },
    "embeddingsProvider": {
        "provider": "ollama",
        "model": "nomic-embed-text",
        "apiBase": "http://localhost:11434/"
    },
    // ...
}
```
