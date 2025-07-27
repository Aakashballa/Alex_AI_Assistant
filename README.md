# 🤖 Jarvis AI Assistant

A personal AI voice assistant inspired by J.A.R.V.I.S from Iron Man — using offline voice recognition and LLM integration (KoboldCpp).

## ✨ Features

- Wake word detection ("Alex")
- Offline speech recognition using VOSK
- Text-to-speech via pyttsx3
- GUI with waveform + Jarvis avatar + manual input
- AI responses from [KoboldCpp](https://github.com/LostRuins/koboldcpp)
- "Stop" button to interrupt responses
- Runs fully offline (except KoboldCpp model download)

## 🛠️ Setup Instructions

### 1. Clone this repository

```bash
git clone https://github.com/Aakashballa/Alex.git
cd Alex

```

### 2. Install Python packages

```bash
python -m venv venv
venv\Scripts\activate       # For Windows
pip install -r requirements.txt
```

### 3. Download VOSK model (not included)

🔗 [Download vosk-model-en-us-0.22](https://alphacephei.com/vosk/models)  
Unzip and place it in:  
`models/vosk-model-en-us-0.22`

### 4. Start KoboldCpp

Install and run [KoboldCpp](https://github.com/LostRuins/koboldcpp) locally on port `5001`.

### 5. Run the assistant

```bash
python jarvis.py
```

## 📁 Project Files

| File | Purpose |
|------|---------|
| `jarvis.py` | Main controller |
| `assistant.py` | AI logic, KoboldCpp, voice |
| `wakeword.py` | Vosk-based wake word detection |
| `gui.py` | GUI: waveform, text box, avatar |
| `requirements.txt` | Python libraries |
| `logo.png` | Optional Jarvis logo (shown in GUI) |

## 🧪 Requirements

- Python 3.10+
- Vosk
- Pyttsx3
- SpeechRecognition
- KoboldCpp running on localhost

## 📄 License

MIT License
