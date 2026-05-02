# local-llm

Minimal Python client that talks to a **local LLM** via [Ollama](https://ollama.com/)’s OpenAI-compatible API (`openai` Python package).

## Prerequisites

- Python 3.10+
- [Poetry](https://python-poetry.org/)
- Ollama running locally with the OpenAI-compatible server (default API base `http://localhost:11434/v1`)
- A model pulled in Ollama (the sample script uses `llama3.2`; change it in `chat.py` if you use another tag)

## Setup

```bash
poetry install
```

## Run

```bash
poetry run python chat.py
```

`chat.py` sends a short chat completion to `http://localhost:11434/v1`. Set `model=` to whatever you have available in Ollama.
