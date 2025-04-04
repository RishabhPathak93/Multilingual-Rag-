# 🏡 Real Estate Voice Assistant (Multilingual) 🎤🤖

This project is a smart multilingual **real estate assistant** that leverages **Whisper**, **Gemini Pro**, **ChromaDB**, and **Google Translate** to:
- Transcribe audio input from clients.
- Detect and translate languages.
- Extract key real estate preferences (like location, budget, and timeline).
- Generate smart, real-time suggestions using Google Gemini.
- Save conversations and follow-ups in ChromaDB.
- Convert assistant responses to speech using gTTS.

---

## 🚀 Features

- 🎙️ **Voice to Text:** Transcribes client audio using OpenAI's Whisper model (supports multilingual input).
- 🌐 **Language Detection & Translation:** Detects non-English languages and translates them to English for processing.
- 🧠 **NLP Extraction:** Extracts real estate-relevant entities like `location`, `budget`, `property type`, and `timeline` using spaCy.
- 💡 **AI Suggestions:** Uses Google Gemini Pro to generate real estate agent follow-ups and suggestions.
- 📦 **Database Logging:** Stores client interactions in a persistent ChromaDB instance for future access.
- 🔊 **Text-to-Speech:** Converts final assistant suggestions back to audio using gTTS.

---

## 🛠️ Tech Stack

- **Python**
- [OpenAI Whisper](https://github.com/openai/whisper)
- [Google Gemini](https://ai.google.dev)
- [spaCy](https://spacy.io/)
- [Google Translate](https://pypi.org/project/googletrans/)
- [gTTS (Google Text-to-Speech)](https://pypi.org/project/gTTS/)
- [langdetect](https://pypi.org/project/langdetect/)
- [ChromaDB](https://www.trychroma.com/)

---

## 📦 Installation

```bash
pip install openai-whisper googletrans==4.0.0-rc1 spacy transformers tqdm langdetect google-generativeai chromadb gtts
python -m spacy download en_core_web_sm
