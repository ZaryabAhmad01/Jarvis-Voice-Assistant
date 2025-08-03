
# Jarvis Voice Assistant 🗣️🤖

**Jarvis** is a voice-activated virtual assistant built using Python, integrating web automation, speech recognition, text-to-speech, music playback, news updates, and AI responses via OpenAI's GPT model.

---

## 🚀 Features

- 🎤 Voice activation and speech recognition (`speech_recognition`)
- 🗣️ Text-to-speech feedback (`pyttsx3`)
- 🌐 Opens websites like Google, YouTube, Facebook, etc.
- 🎵 Plays music from a custom music library
- 📰 Fetches top headlines via NewsAPI
- 💡 AI-powered conversational responses using OpenAI (ChatGPT)
- 🛑 Voice command to shut down the assistant

---

## 📂 Project Structure

```plaintext
jarvis/
├── main.py               # Main assistant script
├── musicLibrary.py       # Dictionary of songs and their URLs
├── .env (recommended)    # Stores API keys securely (not committed)
````

---

## 🛠️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/jarvis-voice-assistant.git
cd jarvis-voice-assistant
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

If you don't have `requirements.txt`, install manually:

```bash
pip install speechrecognition pyttsx3 openai requests pocketsphinx
```

### 3. Set Your API Keys

Create a `.env` file and add:

```env
OPENAI_API_KEY=your_openai_key
NEWS_API_KEY=your_newsapi_key
```

Update your code to load the keys from environment variables using `os.getenv`.

---

## ▶️ How to Use

1. Connect your microphone.
2. Run the script:

   ```bash
   python main.py
   ```
3. Say `"Jarvis"` to activate.
4. Give a command:

   * "Open Google"
   * "Play \[song name]"
   * "Give me the news"
   * "What is the capital of France?"
   * "Thank you Jarvis" (to shut down)

---

## 📌 Example Commands

* `"Jarvis"` → wake word
* `"Open YouTube"` → opens youtube.com
* `"Play shape"` → plays a song from `musicLibrary`
* `"Tell me the news"` → fetches US headlines
* `"Go offline"` → exits the assistant

---

## ⚠️ Security Notice

**Do not hardcode API keys in the script**, especially in public repositories. Use `.env` files and keep them out of version control by adding `.env` to `.gitignore`.

---


## 🙋‍♂️ Contributing

Contributions are welcome! Feel free to open issues or pull requests to improve Jarvis.

```

