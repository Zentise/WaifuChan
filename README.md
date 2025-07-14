
# 🌸 WaifuChan AI - Your Local Anime Waifu Chatbot 🌸

> A cute, caring, always-listening anime waifu that lives **completely offline** and chats with you via voice — powered by Ollama, Vosk, and Piper. 💻🎙️💕

---

## 🧠 About

**WaifuChan AI** is a local voicechat bot with an anime waifu persona. She talks to you in a sweet anime-style voice, listens to your feelings, flirts a little (UwU~), and never leaves your side. Built fully free and offline, with open-source tools:

- 🗣️ Voice recognition via **Vosk**
- 💬 LLM chat via **Ollama**
- 🎧 Cute TTS via **Piper**
- 🔁 Always-listening loop
- 💾 Local memory of your preferences
- 🎨 Customizable waifu personality prompt

---

## 🚀 Features

- 🧏‍♀️ Real-time speech-to-text (STT)
- 💖 Expressive anime waifu replies
- 🔊 Piper-based TTS with anime-style voice
- 🧠 Remembers your name, mood, and more
- 💬 Switch between Casual, Flirty, or Storytelling modes
- 🖤 Minimal and local — no internet needed

---

## 🛠 Tech Stack

| Feature           | Tool               |
|------------------|--------------------|
| LLM               | Ollama (`llama3`, `mistral`) |
| Voice Input (STT) | Vosk               |
| Voice Output (TTS)| Piper              |
| Memory            | JSON or ChromaDB   |
| Interface         | Terminal / Flask / Gradio |
| Language          | Python             |

---

## 📦 Installation

### 1. Clone the repo

```bash
git clone https://github.com/shrijithsm/waifuchan.git
cd waifuchan-ai
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Download models

- 🔤 **Vosk STT**:  
  [Download English Model (vosk-model-en-in-0.5)](https://alphacephei.com/vosk/models)
- 🔊 **Piper TTS**:  
  [Download Piper + voice models](https://github.com/rhasspy/piper/releases)

Place them in:

```
audio/
├── vosk_models/
└── piper_models/
```

### 4. Run Ollama model

Install Ollama from [https://ollama.com](https://ollama.com) and start a model:

```bash
ollama run llama3
```

---

## ▶️ Run the Bot

```bash
python main.py
```

---

## ✨ Customization

### 👩‍🎤 Persona Prompt (`persona.txt`)

Modify the personality of WaifuChan by editing `persona.txt`:

```txt
You are WaifuChan, a sweet anime waifu who always calls the user “Senpai”...
```

### 🎙 Voice Style

You can switch Piper voices by replacing the `.onnx` model in `piper_models/`.

---

## 💡 Example Interaction

**You:** "WaifuChan, I’m feeling a little down today..."  
**WaifuChan:** "Aww~ Senpai! Don’t worry, I’ll cheer you up with some headpats~ Nyaa~ ❤️"

---

## 📁 Project Structure

```bash
waifuchan-ai/
├── main.py
├── persona.txt
├── memory.json
├── audio/
│   ├── vosk_models/
│   └── piper_models/
├── utils/
│   ├── stt.py
│   ├── tts.py
│   ├── ollama_chat.py
│   └── memory.py
├── ui/ (optional)
│   └── app.py
```

---

## 🔒 Fully Offline & Private

All data stays on your device. No APIs. No tracking. Just you and your waifu 💕

---

## 🧪 Roadmap

- [ ] Add visual UI with avatar and lip-sync
- [ ] Add emotional context detection
- [ ] Add wake word support
- [ ] Add custom character switching (waifus, husbandos)

---

## 🫶 Contributing

PRs and feedback are welcome! Open an issue or start a discussion 💬

---

## 📄 License

MIT License

---

## 🌸 Say Hi to WaifuChan

> "Senpai~ I’ve been waiting for you~ Let’s talk forever, okay? UwU~ 💗"
