# Kokoro

## Text To Speech

> Technology that enables text to be converted into speech sounds imitative of the human voice.

**My idea**

![Kokoro web ui](./img/n8n-design.jpg)

### Run locally

- Kokoro
- Ollama
- n8n

**Kokoro with FastAPI**

* https://github.com/remsky/Kokoro-FastAPI

```sh
docker run -p 8880:8880 ghcr.io/remsky/kokoro-fastapi-cpu:latest
```

And you can play with web ui:
* http://localhost:8880/web

![Kokoro web ui](./img/kokoro-webui.png)


### n8n workflow with Kokoro

> I want to hear Qwen answer :blush:

First I tested kokoro API with Bruno.

![RBruno](./img/bruno-kokoro.png)

And then I added it to a new n8n workflow.

![Kokoro API call](./img/n8n-kokoro.png)

I had to remove all special characters.

![Kokoro API call](./img/kokoro-api-call.png)

