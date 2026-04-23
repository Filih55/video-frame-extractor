# 🚀 Gallery-dl ULTIMATE Pro v2.0

**Professional Multi-Platform Media Downloader** – A powerful batch script wrapper for `gallery-dl` with an interactive menu, organized downloads, cookie support, logging, and per-platform settings.

![Windows](https://img.shields.io/badge/Platform-Windows-blue?logo=windows)
![License](https://img.shields.io/badge/License-MIT-green)
![gallery-dl](https://img.shields.io/badge/gallery--dl-required-red)

---

## ✨ Features

- 🎯 **Interactive menu** for 6 major platforms  
  Twitter/X · TikTok · YouTube · Instagram · Reddit · Generic URL  
- 📁 **Automatic folder structure**  
  `Downloads/Twitter`, `Downloads/TikTok`, `Downloads/YouTube`, …  
- 🧾 **Download archives** – never redownload the same file  
- 🍪 **Cookie support** for private/liked content (Twitter, Instagram, TikTok)  
- 📝 **Session logging** – every download is recorded with timestamps  
- ⚙️ **Built-in settings**  
  - Update cookie file  
  - Reset archive  
  - Check/update gallery-dl  
  - Open downloads or config folder  
- 🛡️ **Retry & sleep** – respects rate limits (3 retries, 2–4 sec sleep)  
- 🧹 **No metadata JSON clutter** – configurable to save only media files  

---

## 📦 Requirements

- **Windows** (7, 8, 10, 11)
- **[gallery-dl](https://github.com/mikf/gallery-dl)** installed and available in `PATH`  
  *or* place `gallery-dl.exe` in the same folder as the script.

Optional:  
- `pip` (for updating gallery-dl)  
- Browser extension to export cookies (e.g. *Get cookies.txt LOCALLY*)

---

## 🚀 Installation

1. **Download this repository** or copy `Gallery-dl ULTIMATE Pro v2.0.bat`
2. **Install gallery-dl**  
   ```cmd
   pip install gallery-dl
