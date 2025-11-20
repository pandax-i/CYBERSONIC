🎵 CyberSonic 智能云音乐播放器

在线体验https://m.shanku.lol/

CyberSonic 是一个基于 Web 技术的现代化、极简风格在线音乐播放器。它融合了赛博朋克 (Cyberpunk) 的视觉美学与复古情怀，支持多端响应式布局，集成了全网音乐搜索、本地音乐播放、歌词海报生成及 PWA 离线安装能力。

无需后端数据库，数据纯本地存储，即开即用。

✨ 核心功能

🎧 极致听感

聚合搜索：一键搜索网易云、QQ音乐、酷我音乐资源（默认优先网易云，智能自动换源）。

音乐雷达：随机扫描全网热歌，发现不同风格的惊喜音乐。

本地音乐：支持拖拽或选择本地 MP3/FLAC/WAV 文件进行播放，享受无损音质。

智能下载：自动解析高音质下载链接，支持自动重命名（歌手 - 歌名.mp3）。

📺 沉浸视觉

赛博朋克 UI：全屏动态模糊背景 + 玻璃拟态设计 + 霓虹配色。

音频可视化：底部的 Canvas 频谱条随音乐律动跳跃。

黑胶动画：经典的旋转唱片封面设计。

📻 特色模式：时光电台 (Retro FM)

复古拟物：一键切换至 80-10s 年代的磁带收音机界面。

沉浸体验：真实的 VFD 荧光屏显示、实体按键交互音效、调频时的白噪音过渡。

年代频道：精选 80年代、90年代、00年代、10年代金曲频道。

🛠️ 实用工具

歌词海报：支持多选歌词行，自动生成精美的歌词海报（支持现代/复古两种滤镜风格）。

数据管理：

本地收藏：利用 LocalStorage 实现无数据库收藏夹。

备份与恢复：支持将收藏数据导出为 JSON 文件，或从文件恢复，防止数据丢失。

PWA 支持：可安装至桌面或手机主屏，支持全屏运行和离线缓存。

⌨️ 键盘快捷键

按键

功能

空格 (Space)

播放 / 暂停

← / →

快退 / 快进 5秒

Ctrl + ← / →

上一首 / 下一首

↑ / ↓

音量增加 / 减少

🛠️ 技术栈

核心：原生 HTML5, CSS3 (Flex/Grid), JavaScript (ES6+)。

音频：HTML5 Audio API + Web Audio API (可视化)。

渲染：html2canvas (用于生成海报)。

图标：FontAwesome 6 + Google Fonts (Caveat, VT323)。

API：基于 music-api.gdstudio.xyz 的聚合接口。

🚀 如何运行

由于项目使用了 Service Worker (PWA) 和 跨域图片渲染，请勿直接双击 .html 文件打开，否则会导致功能异常。请务必在 本地服务器 (Localhost) 环境下运行。

方法 1：使用 VS Code (推荐)

安装 Live Server 插件。

在 VS Code 中打开项目文件夹。

右键点击 CyberSonic.html，选择 "Open with Live Server"。

方法 2：使用 Python

如果你安装了 Python，可以在项目根目录打开终端：

# Python 3
python -m http.server 8000


然后访问：http://localhost:8000/CyberSonic.html

方法 3：部署到网络

你可以直接将文件夹上传到 GitHub Pages、Vercel 或 Netlify，即可获得一个永久可访问的在线地址（且自动支持 HTTPS，完美兼容 PWA）。

📂 文件结构

CyberSonic.html - 主程序入口（包含所有逻辑与样式）。

manifest.json - PWA 配置文件。

sw.js - Service Worker 离线缓存脚本。

README.md - 中文说明文档。

README_EN.md - 英文说明文档。
