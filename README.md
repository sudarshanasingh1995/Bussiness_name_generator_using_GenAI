# Bussiness_name_generator_using_GenAI
🤖 A secure, interactive Python tool built in Google Colab that uses Google's Gemini 2.5 Flash API to dynamically generate creative and professional business names based on custom niches and keywords.
# AI Business Name Generator (Gemini Version)

A secure, interactive Python tool built in Google Colab that uses Google's advanced **Gemini 2.5 Flash** model to generate creative, catchy, and professional business names based on user-defined niches and keywords.

---

## 🚀 Features

* **Interactive Inputs:** Prompts the user dynamically to enter their industry/niche and specific themes or keywords.
* **State-of-the-Art AI:** Powered by the official `google-genai` SDK and the `gemini-2.5-flash` model for fast, high-quality, and context-aware suggestions.
* **Enterprise-Grade Security:** Zero risk of hardcoded credentials. It utilizes Google Colab's native **Secrets management** (`userdata`) to keep private API keys completely hidden from public commits.

---

## 🛠️ Tech Stack & Prerequisites

* **Language:** Python 3
* **Environment:** Google Colab (Notebook)
* **AI SDK:** `google-genai`
* **API Requirements:** A valid Gemini API key from [Google AI Studio](https://aistudio.google.com/)

---

## 🔒 How Security Works (Keeping the API Key Safe)

This project strictly adheres to secure coding practices. The API key is **never** written directly into the code. Instead, it leverages Google Colab's `userdata` system:

```python
from google.colab import userdata

# Safely fetches the key locked inside your personal Colab environment
API_KEY = userdata.get("GEMINI_API_KEY")
