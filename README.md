<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&duration=3000&pause=1000&color=00AAFF&center=true&vCenter=true&width=800&lines=J.A.R.V.I.S+Voice+Assistant;Just+A+Rather+Very+Intelligent+System;Your+Personal+AI+Desktop+Assistant" alt="Typing SVG" />

<br/>

![Python](https://img.shields.io/badge/Python-3.8.5-blue?style=for-the-badge&logo=python&logoColor=white)
![PyQt5](https://img.shields.io/badge/PyQt5-5.15.2-green?style=for-the-badge&logo=qt&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Windows-lightblue?style=for-the-badge&logo=windows&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/Gladiator07/JARVIS?style=for-the-badge)

<br/>

> 🤖 **A voice-activated AI desktop assistant inspired by Iron Man's J.A.R.V.I.S.**  
> Built with Python, Speech Recognition & a sleek PyQt5 GUI — your personal command-line superhero.

</div>

---



## 📖 Table of Contents

- [About the Project](#-about-the-project)
- [Tech Stack](#-tech-stack)
- [Features](#-features)
- [Project Structure](#-project-structure)
- [API Keys Required](#-api-keys-required)
- [Installation & Setup](#-installation--setup)
- [Usage](#-usage)
- [Voice Commands Reference](#-voice-commands-reference)
- [Configuration](#️-configuration)
- [Contributing](#-contributing)
- [License](#-license)
- [Future Roadmap](#-future-roadmap)
- [Author](#-author)

---

## 🧠 About the Project

**J.A.R.V.I.S** (Just A Rather Very Intelligent System) is a fully offline-capable, voice-controlled desktop assistant for Windows. Unlike web-based AI tools, JARVIS runs locally on your machine with an animated graphical interface, responding to natural voice commands in real-time.

It's modular by design — each capability lives in its own Python file, making it easy to extend, customize, or replace any feature without touching the core engine.

---

## 🛠 Tech Stack

| Layer | Technology | Purpose |
|-------|-----------|---------|
| **Language** | Python 3.8.5 | Core application logic |
| **GUI Framework** | PyQt5 5.15.2 | Animated graphical interface with GIF wallpaper |
| **Speech Recognition** | SpeechRecognition + Google STT API | Converts microphone audio to text commands |
| **Text-to-Speech** | pyttsx3 (SAPI5 engine) | Converts assistant responses to voice (offline) |
| **Web Automation** | Selenium, Requests | Browser automation, API calls |
| **Web Scraping** | BeautifulSoup4 | Parsing web pages (news, weather) |
| **AI / QA** | Wolframalpha API | Answers computational & factual questions |
| **Wikipedia NLP** | wikipedia library | Fetches encyclopedic summaries |
| **Maps & Geolocation** | geopy, geocoder | Location resolution & distance calculation |
| **Weather** | OpenWeatherMap API | Real-time weather data |
| **Calendar** | Google Calendar API (OAuth2) | Reads your upcoming events |
| **Email** | smtplib (SMTP) | Sends emails via voice command |
| **System Utilities** | psutil, pywin32, pyautogui | RAM/CPU stats, window switching, screenshots |
| **YouTube** | pywhatkit | Plays YouTube videos via voice |
| **News** | Times of India RSS | Top daily headlines |
| **Jokes** | pyjokes | Random programmer jokes |
| **Image Handling** | Pillow | Screenshot display |
| **Dependency Mgmt** | pip + conda | Environment & package management |

---

## ✨ Features

<details>
<summary><b>🗓️ Date & Time</b></summary>

- Tells the current time and date on voice command
</details>

<details>
<summary><b>🌐 Web & App Control</b></summary>

- Open any website by name (`"open youtube.com"`)
- Launch any installed Windows application by path
- Search anything on Google (`"search google for..."`)
- Play any video/song on YouTube (`"youtube <song name>"`)
</details>

<details>
<summary><b>🌦️ Weather</b></summary>

- Real-time weather report for any city worldwide using OpenWeatherMap
</details>

<details>
<summary><b>📍 Location Services</b></summary>

- `"where is <place>"` — finds city, state, country + distance from your location
- `"where am I"` — tells your current location
</details>

<details>
<summary><b>💻 System Monitor</b></summary>

- CPU usage, RAM usage, battery health via psutil
</details>

<details>
<summary><b>📅 Google Calendar</b></summary>

- Reads your upcoming events via Google Calendar API with OAuth2 authentication
</details>

<details>
<summary><b>📚 Knowledge & AI</b></summary>

- Wikipedia summaries for any topic (`"tell me about <topic>"`)
- Answers factual/math questions via Wolframalpha (`"what is..."`, `"calculate..."`)
</details>

<details>
<summary><b>📰 News</b></summary>

- Top daily headlines from Times of India
</details>

<details>
<summary><b>📧 Email</b></summary>

- Send emails entirely by voice — recipient, subject, and body dictated via mic
</details>

<details>
<summary><b>📝 Notes</b></summary>

- `"make a note"` — opens Notepad and writes down what you dictate
</details>

<details>
<summary><b>🖼️ Screenshots</b></summary>

- Takes and saves a screenshot with a custom filename you speak
</details>

<details>
<summary><b>🙈 File Visibility Control</b></summary>

- `"hide all files"` — hides all files in a folder (Windows attrib)
- `"make files visible"` — restores visibility
</details>

<details>
<summary><b>🪟 Window Management</b></summary>

- Switches the active window using Alt+Tab
</details>

<details>
<summary><b>😂 Entertainment</b></summary>

- Tells a random programmer joke
- Plays local music from a specified folder
</details>

<details>
<summary><b>🎨 GUI</b></summary>

- Full-screen animated PyQt5 window with live GIF wallpaper
- Real-time clock and date on the interface
- Run/Exit controls on the GUI
</details>

---

## 📁 Project Structure

```
JARVIS/
├── main.py                  # 🚀 Main entry point — GUI + voice command dispatcher
├── gui.ui                   # 🎨 Qt Designer UI layout file
├── requirements.txt         # 📦 All Python dependencies with pinned versions
├── .gitignore               # 🚫 Excludes credentials, cache, and logs
├── LICENSE                  # 📜 MIT License
├── CONTRIBUTING.md          # 🤝 Contribution guidelines
│
└── Jarvis/
    ├── __init__.py          # 🔗 JarvisAssistant class — aggregates all features
    │
    ├── config/
    │   └── config.py        # 🔐 API keys & credentials (NOT committed to Git)
    │
    ├── features/            # 🧩 Each feature is its own module
    │   ├── date_time.py     # 🕐 Date & time utilities
    │   ├── google_calendar.py # 📅 Google Calendar OAuth + event fetching
    │   ├── google_search.py # 🔍 Google search via Selenium
    │   ├── gui.py           # 🖼️ PyQt5 UI_MainWindow class (auto-generated)
    │   ├── launch_app.py    # ▶️ Launch Windows apps by path
    │   ├── loc.py           # 📍 Location + geolocation + distance
    │   ├── news.py          # 📰 RSS news feed parser
    │   ├── note.py          # 📝 Notepad integration
    │   ├── send_email.py    # 📧 SMTP email sender
    │   ├── system_stats.py  # 💻 CPU / RAM / battery stats
    │   ├── weather.py       # 🌦️ OpenWeatherMap integration
    │   ├── website_open.py  # 🌐 Open URLs in browser
    │   ├── wikipedia.py     # 📖 Wikipedia search
    │   └── youtube_search.py # 🎬 YouTube playback via pywhatkit
    │
    └── utils/
        └── images/          # 🖼️ GIF assets for animated GUI
```

---

## 🔑 API Keys Required

Before running JARVIS, register for the following free API keys:

| API | Link | Used For |
|-----|------|---------|
| OpenWeatherMap | [Register](https://openweathermap.org/api) | Weather data |
| Wolframalpha | [Register](https://www.wolframalpha.com/) | Computational Q&A |
| Google Calendar API | [Register](https://developers.google.com/calendar/auth) | Reading calendar events |

---

## ⚙️ Installation & Setup

### Prerequisites

- Windows OS (required for SAPI5 TTS engine and Windows-specific features)
- Python 3.8.5 (recommended via Anaconda)
- A working microphone
- [PyAudio wheel](https://stackoverflow.com/a/55630212) (not available directly via pip on Windows)

---

### Step 1 — Clone the Repository

```bash
git clone https://github.com/Gladiator07/JARVIS.git
cd JARVIS
```

### Step 2 — Create a Python Environment

Using **Anaconda** (recommended):

```bash
conda create -n jarvis python==3.8.5
conda activate jarvis
```

### Step 3 — Install Dependencies

```bash
pip install -r requirements.txt
```

> ⚠️ **PyAudio** must be installed from a `.whl` wheel file on Windows.  
> Follow the guide: [https://stackoverflow.com/a/55630212](https://stackoverflow.com/a/55630212)

### Step 4 — Create the Config File

Create a file at `Jarvis/config/config.py` with the following content:

```python
weather_api_key = "<your_openweathermap_api_key>"
email = "<your_email_address>"
email_password = "<your_email_password>"
wolframalpha_id = "<your_wolframalpha_app_id>"
```

> 🔐 This file is listed in `.gitignore` and will **never** be pushed to GitHub.

### Step 5 — Set Up Google Calendar (Optional)

1. Go to [Google Calendar API Console](https://developers.google.com/calendar/auth)
2. Create credentials and download `credentials.json`
3. Place `credentials.json` in the project root
4. On first run, JARVIS will open a browser for OAuth sign-in

### Step 6 — Run JARVIS

```bash
python main.py
```

---

## 🎮 Usage

1. Launch `main.py` — the animated PyQt5 GUI will appear
2. Click **Run** to start the voice recognition engine
3. Wait for JARVIS to greet you and say _"Please tell me how may I help you"_
4. Speak any supported command from the list below
5. Click **Exit** or say _"goodbye"_ / _"offline"_ to shut down

---

## 🗣️ Voice Commands Reference

| Command Example | What JARVIS Does |
|----------------|-----------------|
| `"Hey Jarvis"` / `"Wake up Jarvis"` | Wakes up and greets you |
| `"What's the date"` | Speaks today's date |
| `"What's the time"` | Speaks current time |
| `"Open youtube.com"` | Opens the URL in browser |
| `"Launch chrome"` | Launches Google Chrome |
| `"Search Google for Python tutorials"` | Googles the query |
| `"Youtube Believer Imagine Dragons"` | Plays song on YouTube |
| `"What's the weather in Mumbai"` | Reports Mumbai's weather |
| `"Where is Paris"` | Locates Paris + distance |
| `"Where am I"` | Tells your current city/state |
| `"Tell me about Elon Musk"` | Wikipedia summary |
| `"What is the speed of light"` | Wolframalpha answer |
| `"Calculate 452 + 89"` | Math computation |
| `"What do I have today"` | Google Calendar events |
| `"Top headlines"` / `"What's buzzing"` | Top news headlines |
| `"Send email"` | Voice-guided email composition |
| `"Make a note"` | Writes a note in Notepad |
| `"Tell me a joke"` | Random programmer joke |
| `"System status"` | CPU / RAM / battery info |
| `"What is my IP"` | Shows your public IP address |
| `"Switch window"` | Alt+Tab window switch |
| `"Take a screenshot"` | Saves a screenshot |
| `"Hide all files"` | Hides folder contents |
| `"Make files visible"` | Unhides folder contents |
| `"Goodbye"` / `"Offline"` | Shuts down JARVIS |

---

## 🏗️ Configuration

To add a **new feature**:

1. Create a Python file in `Jarvis/features/` (e.g., `my_feature.py`)
2. Write your function inside it
3. Import and expose it in `Jarvis/__init__.py` in the `JarvisAssistant` class
4. Add the voice command trigger in `main.py`'s `TaskExecution()` loop

The modular architecture ensures zero coupling between features — each one can be independently tested and replaced.

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for our code of conduct and the process for submitting pull requests.

```
1. Fork the repository
2. Create a feature branch: git checkout -b feature/AmazingFeature
3. Commit your changes: git commit -m 'Add some AmazingFeature'
4. Push to the branch: git push origin feature/AmazingFeature
5. Open a Pull Request
```

---

## 🗺️ Future Roadmap

- [ ] 🤖 **NLP Integration** — Generalized conversation using NLP models (e.g., GPT, Llama)
- [ ] 🎨 **Improved GUI** — More polished and responsive interface
- [ ] 🔌 **Plugin System** — Hot-reload new features without restarting
- [ ] 🌍 **Multi-language Support** — Hindi, French, Spanish voice commands
- [ ] 📡 **Smart Home Control** — IoT device control via voice
- [ ] 🧪 **Unit Tests** — Test coverage for all feature modules
- [ ] 🐧 **Cross-Platform Support** — Linux and macOS compatibility

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

<div align="center">

**Atharva Ingle**

[![GitHub](https://img.shields.io/badge/GitHub-Gladiator07-black?style=for-the-badge&logo=github)](https://github.com/Gladiator07)

*"With great power comes great responsibility — and a great voice assistant."*

</div>

---

<div align="center">

⭐ **If you found this project useful, please give it a star!** ⭐

Made with ❤️ and Python

</div>
