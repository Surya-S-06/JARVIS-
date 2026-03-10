<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&duration=3000&pause=1000&color=00AAFF&center=true&vCenter=true&width=800&lines=J.A.R.V.I.S+Voice+Assistant;Just+A+Rather+Very+Intelligent+System;Your+Personal+AI+Desktop+Assistant" alt="Typing SVG" />

<br/>

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white)
![PyQt5](https://img.shields.io/badge/PyQt5-5.15+-green?style=for-the-badge&logo=qt&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Windows-lightblue?style=for-the-badge&logo=windows&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/Surya-S-06/JARVIS-?style=for-the-badge)

<br/>

> 🤖 **A voice-activated AI desktop assistant inspired by Iron Man's J.A.R.V.I.S.**  
> Built with Python, Speech Recognition & a sleek PyQt5 GUI — your personal command-line superhero.

</div>

---

## 📖 Table of Contents

- [About the Project](#-about-the-project)
- [What Can JARVIS Do?](#-what-can-jarvis-do)
- [Voice Commands Reference](#-voice-commands-reference)
- [Requirements](#-requirements)
- [Installation & Setup](#️-installation--setup)
- [Configuration](#-configuration)
- [How to Run](#-how-to-run)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Future Roadmap](#-future-roadmap)
- [License](#-license)
- [Author](#-author)

---

## 🧠 About the Project

**J.A.R.V.I.S** (Just A Rather Very Intelligent System) is a fully offline-capable, voice-controlled desktop assistant for Windows. Unlike web-based AI tools, JARVIS runs locally on your machine with an animated graphical interface, responding to natural voice commands in real-time.

It's modular by design — each capability lives in its own Python file, making it easy to extend, customize, or replace any feature without touching the core engine.

---

## ✨ What Can JARVIS Do?

JARVIS supports **20+ voice-triggered features** out of the box:

| # | Category | What It Does |
|---|----------|-------------|
| 1 | 🕐 **Date & Time** | Speaks the current time and today's date |
| 2 | 🌐 **Open Websites** | Opens any website in your browser by name |
| 3 | ▶️ **Launch Apps** | Launches installed applications (Chrome, VLC, etc.) |
| 4 | 🔍 **Google Search** | Searches Google for anything you say |
| 5 | 🎬 **YouTube** | Plays any song or video on YouTube |
| 6 | 🌦️ **Weather** | Real-time weather for any city worldwide |
| 7 | 📖 **Wikipedia** | Gives a quick summary of any topic |
| 8 | 🧮 **Wolframalpha** | Answers math, science, and factual questions |
| 9 | 📰 **News** | Reads today's top headlines (Times of India RSS) |
| 10 | 📧 **Send Email** | Full voice-guided email composition and sending |
| 11 | 📝 **Notes** | Opens Notepad and writes down what you dictate |
| 12 | 😂 **Jokes** | Tells random programmer jokes |
| 13 | 💻 **System Stats** | Reports CPU usage, RAM usage, and battery level |
| 14 | 🌍 **Location Lookup** | Finds any place — city, state, country + distance from you |
| 15 | 📍 **Your Location** | Tells your current city, state, and country |
| 16 | 🌐 **Public IP** | Tells you your public IP address |
| 17 | 📅 **Google Calendar** | Reads your upcoming events (with Google auth) |
| 18 | 🪟 **Window Switcher** | Switches windows using Alt+Tab |
| 19 | 📸 **Screenshot** | Takes and saves a screenshot with your chosen name |
| 20 | 🙈 **File Hider** | Hides or reveals all files in a folder |
| 21 | 🎵 **Local Music** | Plays local music files from a folder you set |

---

## 🗣️ Voice Commands Reference

> Speak these commands after JARVIS says _"Please tell me how may I help you"_

### ⏰ Date & Time
| Say This | JARVIS Does |
|----------|------------|
| `"What's the date"` | Speaks today's date |
| `"What's the time"` | Speaks the current time |

### 🌐 Web & Apps
| Say This | JARVIS Does |
|----------|------------|
| `"Open youtube.com"` | Opens the URL in your browser |
| `"Open github.com"` | Opens any website you name |
| `"Launch chrome"` | Launches Chrome (or any configured app) |
| `"Search Google for Python tutorials"` | Googles the phrase |

### 🎬 Entertainment
| Say This | JARVIS Does |
|----------|------------|
| `"Youtube Believer Imagine Dragons"` | Plays the video on YouTube |
| `"Play music"` | Plays songs from your local music folder |
| `"Tell me a joke"` | Speaks a random programmer joke |

### 🌦️ Information
| Say This | JARVIS Does |
|----------|------------|
| `"What's the weather in Mumbai"` | Gives Mumbai's weather report |
| `"Tell me about Elon Musk"` | Wikipedia summary of the topic |
| `"What is the speed of light"` | Wolframalpha answer |
| `"Who is Albert Einstein"` | Wolframalpha answer |
| `"Calculate 452 + 89"` | Math computation result |
| `"Top headlines"` | Reads today's top news |
| `"What's buzzing"` | Same as top headlines |

### 📧 Communication
| Say This | JARVIS Does |
|----------|------------|
| `"Send email"` | Starts voice-guided email (asks Who, Subject, Body) |

### 💻 System
| Say This | JARVIS Does |
|----------|------------|
| `"System status"` | Speaks CPU %, RAM %, Battery % |
| `"What is my IP"` | Speaks your public IP |
| `"Switch window"` | Sends Alt+Tab |
| `"Take a screenshot"` | Saves screenshot (asks for filename) |

### 📍 Location
| Say This | JARVIS Does |
|----------|------------|
| `"Where is Paris"` | Locates Paris + distance from you |
| `"Where am I"` | Tells your current city and country |
| `"What do I have today"` | Reads Google Calendar events |

### 📝 Productivity
| Say This | JARVIS Does |
|----------|------------|
| `"Make a note"` | Opens Notepad, writes what you dictate |
| `"Write this down"` | Same as make a note |
| `"Hide all files"` | Hides all files in current folder |
| `"Make files visible"` | Un-hides files in current folder |

### 🔴 Shutdown
| Say This | JARVIS Does |
|----------|------------|
| `"Goodbye"` / `"Offline"` / `"Bye"` | JARVIS says farewell and exits |

---

## 📋 Requirements

### System Requirements
- ✅ **Windows OS** (required — uses SAPI5 TTS engine & Windows APIs)
- ✅ **Python 3.8 or newer**
- ✅ **Working microphone** (for voice input)
- ✅ **Internet connection** (for Weather, News, Wikipedia, Google STT)

### Python Packages (auto-installed via pip)

| Package | Purpose |
|---------|---------|
| `PyQt5` | Animated GUI window |
| `pyttsx3` | Text-to-speech (offline) |
| `SpeechRecognition` | Mic → text via Google STT |
| `PyAudio` | Microphone access |
| `wolframalpha` | Math & factual Q&A |
| `pywhatkit` | YouTube playback |
| `pyjokes` | Programmer jokes |
| `pyautogui` | Screenshots, Alt+Tab |
| `selenium` | Google search automation |
| `requests` | HTTP calls (IP, weather) |
| `beautifulsoup4` | News feed parsing |
| `wikipedia` | Wikipedia summaries |
| `psutil` | CPU / RAM / battery stats |
| `geopy` + `geocoder` | Location resolution |
| `Pillow` | Image / screenshot handling |
| `google-api-python-client` | Google Calendar API |
| `google-auth-oauthlib` | Google OAuth2 sign-in |

### Optional API Keys (for advanced features)

| Feature | API Key Needed | Get It Free From |
|---------|---------------|-----------------|
| ☁️ Weather | OpenWeatherMap API Key | [openweathermap.org/api](https://openweathermap.org/api) |
| 🧮 Math / Q&A | Wolframalpha App ID | [wolframalpha.com](https://developer.wolframalpha.com/) |
| 📅 Calendar | Google Calendar credentials.json | [Google Cloud Console](https://console.cloud.google.com/) |

---

## ⚙️ Installation & Setup

### Step 1 — Clone the Repository

```bash
git clone https://github.com/Surya-S-06/JARVIS-.git
cd JARVIS-
```

### Step 2 — Install All Dependencies

```bash
py -3 -m pip install PyQt5 pyttsx3 SpeechRecognition pyaudio wolframalpha pywhatkit pyjokes pyautogui selenium requests beautifulsoup4 wikipedia psutil geopy geocoder Pillow google-api-python-client google-auth-oauthlib pytz pywin32
```

> ⚠️ **If PyAudio fails** on your machine, install it manually:
> 1. Go to [PyAudio Wheels](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio)
> 2. Download the `.whl` for your Python version
> 3. Run: `py -3 -m pip install PyAudio‑0.2.11‑cp3x‑win_amd64.whl`

### Step 3 — Fill in Your Config File

Open `Jarvis/config/config.py` and replace the placeholders:

```python
email = "your_gmail@gmail.com"           # Gmail address for sending emails
email_password = "your_app_password"     # Gmail App Password (NOT your main password)
wolframalpha_id = "your_app_id_here"     # From Wolframalpha developer portal
```

> 🔐 **Gmail App Password**: Go to [myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords) — create an "App Password" for Mail. Use this instead of your real password.

> 🔐 This `config.py` file is in `.gitignore` and will **never** be pushed to GitHub.

### Step 4 — Add Your Email Contacts (Optional)

In `main.py`, find the `EMAIL_DIC` dictionary and add your contacts:

```python
EMAIL_DIC = {
    'myself': 'your_email@gmail.com',
    'mom': 'moms_email@gmail.com',
    'friend': 'friends_email@gmail.com',
}
```

Then say: _"Send email"_ → JARVIS asks _"Whom?"_ → you say _"mom"_

### Step 5 — Set Up Google Calendar (Optional)

1. Go to [Google Calendar API Console](https://developers.google.com/calendar/auth)
2. Create credentials → download `credentials.json`
3. Place `credentials.json` in the project root
4. On first run, JARVIS opens a browser for OAuth sign-in — sign in once, it saves the token

---

## ▶️ How to Run

```bash
py -3 main.py
```

**What happens:**
1. 🖥️ The **animated JARVIS window** opens (full-screen PyQt5 GUI)
2. ▶️ Click the **Run** button — JARVIS starts booting up
3. 🔊 JARVIS speaks a startup sequence and greets you by time of day
4. 🎤 Say **"Hey Jarvis"** to wake it up
5. 🗣️ Speak any command from the list above
6. 🔴 Say **"Goodbye"** to shut down

> 💡 **Tip:** Keep the console window open — JARVIS prints all responses there too.

---

## 🛠 Tech Stack

| Layer | Technology | Purpose |
|-------|-----------|---------| 
| **Language** | Python 3.8+ | Core application logic |
| **GUI Framework** | PyQt5 5.15+ | Animated graphical interface with GIF wallpaper |
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

---

## 📁 Project Structure

```
JARVIS-/
├── main.py                  # 🚀 Main entry point — GUI + voice command dispatcher (heavily commented)
├── gui.ui                   # 🎨 Qt Designer UI layout file
├── requirements.txt         # 📦 All Python dependencies
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

**Surya S**

[![GitHub](https://img.shields.io/badge/GitHub-Surya--S--06-black?style=for-the-badge&logo=github)](https://github.com/Surya-S-06)

*"With great power comes great responsibility — and a great voice assistant."*

</div>

---

<div align="center">

⭐ **If you found this project useful, please give it a star!** ⭐

Made with ❤️ and Python

</div>
