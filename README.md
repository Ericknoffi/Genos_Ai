# Genos AI - Voice Assistant

A Python-based voice-activated personal assistant that can perform various tasks through voice commands, including web searches, opening/closing applications, and providing information.

## Features

- 🎤 **Voice Recognition**: Listen and respond to voice commands
- 🗣️ **Text-to-Speech**: Provides audio feedback using natural-sounding voices
- 🔍 **Web Search**: Search Google, YouTube, and Wikipedia
- 💻 **Application Control**: Open and close applications with voice commands
- 🌐 **Web Navigation**: Open websites directly
- ⏰ **Smart Greeting**: Greets you based on the time of day
- 😴 **Sleep Mode**: Wake up/sleep functionality to save resources

## Prerequisites

- Python 3.x
- Microphone for voice input
- Speakers for audio output
- Windows OS (for application control features)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/genos-ai.git
cd genos-ai
```

2. Install required dependencies:
```bash
pip install pyttsx3
pip install SpeechRecognition
pip install pyautogui
pip install pywhatkit
pip install wikipedia
```

## Usage

1. Run the main program:
```bash
python Genos.py
```

2. Wake up the assistant:
```
Say: "Wake up"
```

3. Give commands:
```
- "Open Chrome"
- "Search Google for Python tutorials"
- "Search YouTube for music"
- "Search Wikipedia for artificial intelligence"
- "Close Chrome"
- "Hello"
- "How are you"
- "Sleep mode" or "Exit"
```

## Project Structure

```
genos-ai/
├── Genos.py          # Main application entry point
├── assistant.py      # Text-to-speech and greeting functions
├── utils.py          # Voice recognition utilities
├── search.py         # Web search functionality (Google, YouTube, Wikipedia)
├── Dictapp.py        # Application and website control
└── installer.py      # Dependency installer helper
```

## Supported Commands

### Basic Interaction
- **Wake up** - Activate the assistant
- **Hello** - Greet the assistant
- **How are you** - Check assistant status
- **Thank you** - Express gratitude
- **Exit/Quit/Sleep mode** - Deactivate the assistant

### Web Search
- **Google [query]** - Search Google and get a quick summary
- **YouTube [query]** - Search YouTube videos
- **Wikipedia [query]** - Get information from Wikipedia

### Application Control
- **Open [app name]** - Launch applications
  - Supported apps: Chrome, Brave, VS Code, Word, Excel, PowerPoint, File Manager, Command Prompt, Settings
- **Open [website.com]** - Open websites in browser
- **Close [app name]** - Close running applications
- **Close [number] tabs** - Close browser tabs

## Supported Applications

The assistant can open and close the following applications:
- Web Browsers: Chrome, Brave
- Microsoft Office: Word, Excel, PowerPoint
- Development Tools: VS Code
- System Tools: File Manager, Command Prompt, Settings

## Configuration

### Voice Settings
You can modify voice properties in [assistant.py](assistant.py):
- Voice type (male/female)
- Speech rate
- Volume

### Application Dictionary
Add or modify supported applications in [Dictapp.py](Dictapp.py) by editing the `dictapp` dictionary.

## Troubleshooting

**Microphone not working:**
- Check microphone permissions in Windows settings
- Ensure microphone is set as default recording device

**Voice recognition errors:**
- Speak clearly and at a moderate pace
- Reduce background noise
- Adjust `energy_threshold` in [utils.py](utils.py)

**Applications not opening:**
- Ensure applications are installed and in system PATH
- Run the script with appropriate permissions

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Built with Python
- Uses Google Speech Recognition API
- Powered by pyttsx3 for text-to-speech
- Wikipedia API for information retrieval

## Future Enhancements

- [ ] Add support for more applications
- [ ] Implement weather information
- [ ] Add calendar integration
- [ ] Support for multiple languages
- [ ] Add automation for common tasks
- [ ] Implement reminders and alarms

---

**Note:** This assistant requires an active internet connection for voice recognition and web search features.
