🎵 CyberSonic Smart Cloud Music Player

中文 | English

A modern, minimalist online music player built with web technologies. Featuring a Cyberpunk visual design, responsive layout, cross-platform music search, lyric poster generation, and PWA offline installation capabilities.

✨ Key Features

🔮 Immersive Visuals: Full-screen dynamic blur background + glassmorphism UI, featuring rhythmic spectrum visualization.

📡 Music Radar: One-click scan for trending songs across the web, randomly exploring different music styles (prioritizing NetEase Cloud Music source).

📻 Retro FM: A unique retro cassette player mode that takes you back to the 80s-10s, accompanied by realistic white noise experiences.

📸 Lyric Poster:

Support multi-selection of lyric lines.

Automatically fetch high-definition covers.

One-click generation of exquisite posters (supports modern/retro filter styles).

❤️ Local Favorites: Implements a database-free favorites function using LocalStorage for persistent data storage.

📱 PWA Support:

Installable to desktop or mobile home screens.

Full-screen immersive runtime.

Offline caching of UI resources.

⬇️ Smart Download: Automatically resolves high-quality download links and supports ID3 information completion (automatic filename renaming).

🛠️ Tech Stack

Core: Native HTML5, CSS3, JavaScript (ES6+).

Audio: HTML5 Audio API + Web Audio API (Visualization).

Rendering: html2canvas (For poster generation).

Icons: FontAwesome 6.

API: Based on music-api.gdstudio.xyz aggregation interface.

🚀 How to Run

Due to the project's use of Service Worker (PWA) and Cross-Origin Image Rendering, directly opening the .html file may cause some features to fail. Please ensure to run it in a Local Server (Localhost) environment.

Method 1: VS Code (Recommended)

Install the Live Server extension.

Open the project folder in VS Code.

Right-click CyberSonic.html and select "Open with Live Server".

Method 2: Python

If you have Python installed, open a terminal in the project root directory:

# Python 3
python -m http.server 8000


Then visit: http://localhost:8000/CyberSonic.html

Method 3: Deploy to Web

You can upload the folder directly to GitHub Pages, Vercel, or Netlify to get a permanent online address (with automatic HTTPS support, perfectly compatible with PWA).

📂 File Structure

CyberSonic.html - Main application entry.

manifest.json - PWA configuration file, defining icons and app name.

sw.js - Service Worker script, responsible for offline caching strategies.

README.md - Project documentation (Chinese).

README_EN.md - Project documentation (English).
