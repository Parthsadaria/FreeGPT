# 🌟 Loki.AI API Documentation
> *Powerful AI Integration at Your Fingertips*

[![Made with Love](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F-red.svg)](https://github.com/parthsadaria) 
[![Developer](https://img.shields.io/badge/Developer-Parth%20Sadaria-blue.svg)](https://github.com/parthsadaria)

## 🚀 Quick Start Guide

### Base URL
```
https://parthsadaria-lokiai.hf.space
```

### API Endpoints
| Endpoint | URL | Description |
|----------|-----|-------------|
| Chat Completions | `/chat/completions` | Main chat interface |
| SearchGPT | `/searchgpt?q=todays news` | Search functionality |
| Models | `/models` | Available models list |

> 🎉 **Supports streaming functionality!**

## 🛡️ Authentication
**No authentication required!** 

🎊 **It's completely FREE!** 

## 📦 Request Format

```json
{
    "model": "gpt-4o",
    "messages": [
        {
            "role": "user",
            "content": "Hello, AI!"
        }
    ],
    "stream": false
}
```

## 📤 Response Format

```json
{
  "id": "chatcmpl-89DmxGJl4oqEultjlLBnGfdkV7Euk",
  "model": "gpt-4o",
  "object": "chat.completion",
  "created": 1731674826,
  "choices": [
    {
      "index": 0,
      "message": {
        "role": "assistant",
        "content": "Hello! How can I assist you today?"
      },
      "finish_reason": "stop"
    }
  ],
  "usage": {
    "prompt_tokens": 11,
    "completion_tokens": 9,
    "total_tokens": 20
  }
}
```

## 🛠️ Example Usage

```python
import openai

# Set API details
api_key = ''  # No key needed!
openai.api_base = "https://parthsadaria-lokiai.hf.space"
openai.api_key = api_key

def chat_with_gpt():
    try:
        response = openai.ChatCompletion.create(
            model="gpt-4o", 
            messages=[{"role": "user", "content": "hi homie"}],
            stream=False
        )
        print(response['choices'][0]['message']['content'])
    except Exception as e:
        print(f"Error: {e}")

chat_with_gpt()
```

## 🎨 Available Models

### GPT Family
- `gpt-4o`
- `gpt-4o-mini`
- `gpt-3.5-turbo`

### Llama Family
- `llama-3.1-7b`
- `llama-3.1-405b`
- `llama-3.1-80b`

### Gemini Models
- `gemini-pro`
- `gemini-1.5-flash`

### Mistral Models
- `mistral-medium`
- `mixtral-8x7b`

> 📚 For a complete list of models, visit: [Models Documentation](https://parthsadaria-lokiai.hf.space/models)
---

<div align="center">
  
### Built with ❤️ by Parth Sadaria

</div>
