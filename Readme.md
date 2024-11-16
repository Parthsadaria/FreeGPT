# Loki.AI API 🌟  
**Powerful AI Integration at Your Fingertips**  

Made With ❤️ by **Parth Sadaria**  

---

## 🚀 Quick Start Guide  

### **Base URL**  
`https://parthsadaria-lokiai.hf.space`  

### **Chat Completion URL**  
`https://parthsadaria-lokiai.hf.space/chat/completions`  

### **Searchgpt URL**  
`https://parthsadaria-lokiai.hf.space/searchgpt?q=todays news`  

Supports **stream** functionality! 🎉  

---

## 🔮 Models Endpoint  
`https://parthsadaria-lokiai.hf.space/models`  

---

## 🛡️ Authentication  
**NO AUTHENTICATION REQUIRED!**  
Yes, it's **FREE**! WOHOOOOO!! 🥳  

---

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

---

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

---

## 🛠️ Example Usage  
```python
import openai  

# Set API details  
api_key = ''  # No key needed, but hampe to he hi no :p  
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

---

## 🎨 Available Models  
For detailed info, visit:  
👉 [https://parthsadaria-lokiai.hf.space/models](https://parthsadaria-lokiai.hf.space/models)  

Here’s a list of supported models:  
- **GPT Family**  
  - `gpt-4`  
  - `gpt-4-turbo`  
  - `gpt-4o`  
  - `gpt-3.5-turbo`  
  - Many more...  

- **Llama Family**  
  - `llama-3.1-7b`  
  - `llama-3.1-405b`  
  - `llama-3.1-80b`  

- **Gemini**  
  - `gemini-pro`  
  - `gemini-pro-vision`  

- **Mistral**  
  - `mistral-medium`  
  - `mixtral-8x7b`  

- And a lot more!  

---

## 🚀 Get Started Now  
Ready to integrate Loki.AI into your application?  

Join our [**Discord Community**](dsc.gg/chadgang) to connect with other developers and share your experience!  
---

**Built with ❤️ by Parth Sadaria**  
```
