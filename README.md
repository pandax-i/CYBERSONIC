🎵 CyberSonic 智能云音乐播放器

一个基于 Web 技术的现代化、极简风格在线音乐播放器。采用赛博朋克 (Cyberpunk) 视觉设计，支持多端响应式布局，集成了全网音乐搜索、歌词海报生成及 PWA 离线安装能力。

✨ 核心功能

🔮 沉浸式视觉：全屏动态模糊背景 + 玻璃拟态 UI，支持频谱律动可视化。

📡 音乐雷达：一键扫描全网热歌，随机探索不同风格的音乐（优先网易云源）。

📻 时光电台 (Retro FM)：独特的复古磁带机模式，带你回到 80-10s 年代，伴随真实的白噪音体验。

📸 歌词海报：

支持点击歌词行多选。

自动抓取高清封面。

一键生成精美海报（支持现代/复古两种滤镜风格）。

❤️ 本地收藏：利用 LocalStorage 实现无数据库的收藏夹功能，数据持久化保存。

📱 PWA 支持：

支持安装到桌面或手机主屏幕。

全屏沉浸式运行。

离线缓存 UI 资源。

⬇️ 智能下载：自动解析高音质下载链接，支持 ID3 信息补全（文件名自动重命名）。

🛠️ 技术栈

核心：原生 HTML5, CSS3, JavaScript (ES6+)。

音频：HTML5 Audio API + Web Audio API (可视化)。

渲染：html2canvas (用于生成海报)。

图标：FontAwesome 6。

API：基于 music-api.gdstudio.xyz 的聚合接口。

🚀 如何运行

由于项目使用了 Service Worker (PWA) 和 跨域图片渲染，直接双击 .html 文件可能会导致部分功能报错。请务必在 本地服务器 (Localhost) 环境下运行。

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

CyberSonic.html - 主程序入口。

manifest.json - PWA 配置文件，定义图标和应用名称。

sw.js - Service Worker 脚本，负责离线缓存策略。

README.md - 项目说明文档。
