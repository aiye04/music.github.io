# 🎵 Music Player

一个简洁优雅的在线音乐播放器，基于原生 HTML、CSS 和 JavaScript 构建。无需任何依赖，即可在浏览器中播放音乐并支持歌词显示。

> 🎓 **项目背景**：本项目为专业课学习项目作业，旨在通过实践掌握 Web 前端开发技术（HTML5、CSS3、JavaScript）及 Web Audio API 的应用。

**在线体验：** https://aiye04.github.io/music.github.io/

---

## ✨ 功能特点

### 🎧 音乐播放
- ▶️ 播放/暂停控制
- ⏭️ 上一曲/下一曲切换
- 🔀 顺序播放/随机播放模式
- 🔁 单曲循环/列表循环
- 📊 播放进度条（支持点击跳转）
- 🔊 音量控制（滑块调节）

### 📝 歌词显示
- LRC 格式歌词解析
- 🎼 歌词滚动高亮
- 🌐 双语歌词支持
- ⏱️ 歌词时间同步

### 💿 视觉特效
- 💫 唱片旋转动画
- 🔮 背景模糊效果
- 🎨 玻璃拟态（Glassmorphism）设计
- ✨ 流畅的过渡动画

### 🎬 MV 播放
- 独立的 MV 播放页面
- 全屏播放支持
- 简洁的播放器控件

---

## 🛠️ 技术栈

| 技术 | 说明 |
|------|------|
| **HTML5** | 语义化页面结构 |
| **CSS3** | 样式设计与动画效果 |
| **JavaScript** | 播放器逻辑控制 |
| **Web Audio API** | 音频处理 |
| **SmileySans** | 中文字体（得意黑） |

---

## 📁 项目结构

```
music.github.io/
├── index.html          # 主页面（音乐播放器）
├── mv-player.html      # MV 播放器页面
├── CSS/
│   └── audio.css       # 播放器样式文件
├── JS/
│   └── main.js         # 播放器核心逻辑
├── img/                # 图片资源目录
├── mp3/                # 音频文件目录
├── mp4/                # 视频文件目录
└── SmileySans-Oblique.ttf  # 字体文件
```

---

## 🚀 快速开始

### 方式一：直接使用

1. 克隆或下载本仓库
2. 直接在浏览器中打开 `index.html`

```bash
git clone https://github.com/aiye04/music.github.io.git
cd music.github.io
# 打开 index.html
```

### 方式二：部署到 GitHub Pages

1. Fork 本仓库
2. 进入仓库 **Settings** → **Pages**
3. 在 **Source** 中选择 `main` 分支和 `/ (root)` 目录
4. 点击 **Save**，等待部署完成
5. 访问 `https://你的用户名.github.io/music.github.io/`

### 方式三：本地服务器

```bash
# 使用 Python
python -m http.server 8000

# 使用 Node.js (npx)
npx serve

# 使用 PHP
php -S localhost:8000
```

然后访问 `http://localhost:8000`

---

## 📖 使用指南

### 添加音乐

1. 将 MP3 文件放入 `mp3/` 目录
2. 在 `JS/main.js` 中找到 `musicData` 数组
3. 添加新的音乐信息：

```javascript
{
    name: "歌曲名称",
    artist: "歌手",
    album: "专辑名",
    url: "mp3/你的音乐文件.mp3",
    cover: "img/封面图.jpg",
    lrc: "歌词.lrc"  // 可选
}
```

### 添加歌词

歌词文件需使用 LRC 格式，示例：

```
[00:00.00] 第一行歌词
[00:05.50] 第二行歌词
[00:11.20] <双语>第三行歌词
```

### 自定义样式

- 播放器主样式：`CSS/audio.css`
- 可修改主题颜色、动画效果等

---

## 🎨 界面预览

播放器采用现代玻璃拟态设计，包含以下核心元素：

```
┌─────────────────────────────────────┐
│         [背景模糊效果]              │
│  ┌─────────────────────────────┐   │
│  │    💿 旋转唱片封面           │   │
│  │                             │   │
│  │    🎵 歌曲名称               │   │
│  │    👤 歌手 - 专辑            │   │
│  │                             │   │
│  │  00:00 ━━━━━●━━━━━ 03:45   │   │
│  │                             │   │
│  │   ⏮️   ▶️   ⏭️   🔀   🔁   │   │
│  │                             │   │
│  │   🔊 ━━━━━●━━━             │   │
│  │                             │   │
│  │   ┌─────────────────────┐   │   │
│  │   │  🎼 歌词显示区域     │   │   │
│  │   │  （滚动高亮同步）    │   │   │
│  │   └─────────────────────┘   │   │
│  └─────────────────────────────┘   │
└─────────────────────────────────────┘
```

---

## 🔧 开发说明

### 环境要求

- 现代浏览器（Chrome、Firefox、Safari、Edge）
- 无需构建工具或依赖安装

### 调试

1. 直接修改源代码
2. 在浏览器中刷新页面即可查看效果
3. 推荐使用 Chrome DevTools 进行调试

---

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. **Fork** 本仓库
2. 创建特性分支：`git checkout -b feature/新功能`
3. 提交更改：`git commit -m '添加新功能'`
4. 推送分支：`git push origin feature/新功能`
5. 提交 Pull Request

---

## 📄 许可证

本项目基于 [MIT License](LICENSE) 开源，您可以自由使用、修改和分发。

---

## 🙏 致谢

- 字体：[SmileySans 得意黑](https://github.com/atelier-anchor/smileySans)
- 设计灵感：各开源音乐播放器项目

---

**如果这个项目对您有帮助，欢迎 Star ⭐ 支持！**
