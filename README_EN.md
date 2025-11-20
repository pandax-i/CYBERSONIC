🎵 CyberSonic Smart Cloud Music Player

https://m.shanku.lol/

A modern, minimalist online music player built with web technologies. It fuses Cyberpunk visual aesthetics with Retro nostalgia, featuring a responsive layout, cross-platform music search, local file playback, lyric poster generation, and PWA offline installation capabilities.

No backend database required. Data is stored locally. Ready to use out of the box.

✨ Key Features

🎧 Ultimate Audio Experience

Aggregated Search: One-click search across NetEase, QQ Music, and Kuwo (Prioritizes NetEase, with smart auto-fallback).

Music Radar: Randomly scans the web for trending songs to discover hidden gems.

Local Music: Support drag-and-drop or file selection for local MP3/FLAC/WAV playback with lossless quality (includes local spectrum visualization).

Smart Download: Automatically resolves high-quality download links and supports file renaming (Artist - Song Name.mp3).

📺 Immersive Visuals

Cyberpunk UI: Full-screen dynamic blur background + Glassmorphism design + Neon color scheme.

Audio Visualization: Bottom Canvas spectrum bars dance to the rhythm of the music.

Vinyl Animation: Classic rotating record cover design.

📻 Special Mode: Retro FM

Skeuomorphic Design: Switch to an 80s-10s style cassette radio interface with one click.

Immersive Experience:

Real VFD fluorescent display.

Tactile physical button sound effects and interaction.

Realistic white noise transitions when tuning.

Decade Channels: Curated channels for 80s, 90s, 00s, and 10s hits.

🛠️ Utility Tools

Lyric Poster: Select multiple lyric lines to generate exquisite posters (supports automatic switching between Modern Minimalist or Retro Polaroid styles).

Social Sharing: Generate deep links (e.g., ?share=...) to share songs. Friends can open the link to automatically play the specific song.

Data Management:

Local Favorites: Database-free favorites using LocalStorage.

Multi-Playlist System: Create and manage custom playlists.

External Import: Support parsing and importing NetEase/QQ Music playlist links.

Backup & Restore: Export collection to JSON or import from file to prevent data loss.

PWA Support: Installable to desktop or mobile home screens, supports full-screen runtime and offline caching.

⌨️ Keyboard Shortcuts

Key

Function

Space

Play / Pause

← / →

Rewind / Fast Forward 5s

Ctrl + ←

Previous Song

Ctrl + →

Next Song

🛠️ Tech Stack

Core: Native HTML5, CSS3 (Flex/Grid), JavaScript (ES6+).

Audio: HTML5 Audio API + Web Audio API (Visualization).

Rendering: html2canvas (For poster generation).

Icons: FontAwesome 6 + Google Fonts (Caveat, VT323).

API: Based on music-api.gdstudio.xyz aggregation interface.

🚀 How to Run

Due to the project's use of Service Worker (PWA) and Cross-Origin Image Rendering, DO NOT open the .html file directly. It may cause features like poster generation or PWA registration to fail. Please ensure to run it in a Local Server (Localhost) or HTTPS environment.

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

CyberSonic.html - Main application entry (Contains logic & styles).

manifest.json - PWA configuration file.

sw.js - Service Worker script.

README.md - Documentation in Chinese.

README_EN.md - Documentation in English.
