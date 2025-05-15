# Jarvis Voice Assistant

## Project Description
Jarvis is a simple voice assistant application built in Python. It listens for the wake word "hey jarvis" and responds to voice commands to perform various tasks such as opening popular websites, playing songs from a predefined music library, and reading the latest news headlines.

## Features
- Wake word detection ("hey jarvis") to activate the assistant.
- Open popular websites like Google, YouTube, Facebook, and LinkedIn via voice commands.
- Play songs from a predefined music library by voice command.
- Fetch and read out the latest news headlines using the NewsAPI.
- Text-to-speech functionality using both `pyttsx3` and Google Text-to-Speech (`gTTS`).
- Uses speech recognition to convert spoken commands into text.

## Dependencies
The project requires the following Python packages:
- `speech_recognition`
- `pyttsx3`
- `gtts`
- `pygame`
- `requests`
- `webbrowser` (standard library)

You can install the required packages using pip:
```bash
pip install SpeechRecognition pyttsx3 gTTS pygame requests
```

## How to Run
1. Ensure you have a working microphone connected to your system.
2. Run the `main.py` script:
```bash
python main.py
```
3. Say "hey jarvis" to activate the assistant.
4. After activation, speak your command clearly.

## Supported Commands
- **Open websites:**  
  - "open google"  
  - "open youtube"  
  - "open facebook"  
  - "open linkedin"  
- **Play songs:**  
  Say "play" followed by the song name. Supported songs are:  
  - kinna sona  
  - iktara  
  - jaan ban gae  
  - mere bina  
- **Get news:**  
  Say "news" to hear the latest news headlines.

## Music Library
The music library is defined in `musicLibrary.py` as a dictionary mapping song names to YouTube URLs. You can add or modify songs by editing this file.

Example:
```python
music = {
    "kinna sona": "https://youtu.be/XrjwsY-BFck?si=dRtlcz5hTkVJbYon",
    "iktara": "https://youtu.be/fSS_R91Nimw?si=AhOiO2vJW2WUtbjb",
    "jaan ban gae": "https://youtu.be/rp5QKYqHV-k?si=rzE72T_MQztwPc0d",
    "mere bina": "https://youtu.be/XvUSsh3gdO4?si=rbaZiDkBQv-Km6VH"
}
```

## Notes
- The news feature uses the NewsAPI and requires a valid API key. The current key is set in `main.py`.
- The assistant uses Google Speech Recognition for converting speech to text.
- The text-to-speech uses `gTTS` for better voice quality and `pygame` to play the audio.

## License
This project is open source and free to use.
