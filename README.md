# Yunxi AI Image Generator & Splitter (Nano Banana V2)

**English** | **[简体中文](docs/zh/README.md)**

<div align="center">

![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Node](https://img.shields.io/badge/node-%3E%3D16.0.0-brightgreen.svg)

**One-Click AI Image Generation · Smart Splitting · Multi-Language Support**

[Live Demo](https://banana2.zjhn.com) · [Report Issue](https://github.com/xiyunnet/banana2/issues)

</div>

---

## 📖 Overview

Yunxi AI Image Generator & Splitter is a web-based AI image generation and management tool that supports:

- 🎨 **AI Image Generation** - Multiple models, resolutions, and aspect ratios
- ✂️ **Smart Splitting** - Automatically split images into 2/4/6/9 grids
- 🌐 **Multi-Language Support** - Chinese, English, Traditional Chinese, Japanese, Korean
- 📁 **Local Management** - Images automatically saved to local directory
- 🔄 **Task Management** - Real-time polling and status tracking

---

## 🚀 Quick Start

### Requirements

- Node.js >= 16.0.0
- npm or yarn

### Installation

```bash
# Clone repository
git clone https://github.com/xiyunnet/banana2.git

# Enter directory
cd banana2

# Install dependencies
npm install

# Start service
npm start
```

Access the application at: http://localhost:2688

---

## ⚙️ Configuration

### Get API Key

This project uses API services from [Ace Data](https://share.acedata.cloud/r/1uN88BrUTQ):

1. Visit [Ace Data](https://share.acedata.cloud/r/1uN88BrUTQ) to register
2. Get **API Key** (for image generation)
3. Get **Platform Token** (for image upload, optional)

### Settings

Configure on first use:

1. Click **Settings** button in top right
2. Enter API Key (required)
3. Enter Platform Token (optional, for image-to-image)
4. Enter LLM API Key (optional, for AI prompt generation)

---

## 📁 Project Structure

```
nano-banana-v2/
├── server/                 # Backend service
│   ├── index.js           # Main entry
│   └── services/          # Business logic
├── public/                 # Frontend files
│   ├── index.html         # Main page
│   ├── list.html          # List page
│   ├── set.html           # Settings page
│   ├── components/        # Components
│   ├── css/               # Styles
│   ├── js/                # Scripts
│   └── lan/               # Languages
├── config/                 # Config files
├── database/              # Database files
└── docs/                  # Documentation
    ├── en/                # English docs
    └── zh/                # Chinese docs
```

---

## 🌐 Multi-Language Support

| Language | Code | Status |
|----------|------|--------|
| Simplified Chinese | zh | ✅ Complete |
| English | en | ✅ Complete |
| Traditional Chinese | zh-TW | ✅ Complete |
| Japanese | ja | ✅ Complete |
| Korean | ko | ✅ Complete |

---

## 🛠️ Tech Stack

- **Backend**: Node.js + Express + SQLite
- **Frontend**: HTML5 + CSS3 + JavaScript (jQuery)
- **Image Processing**: Sharp
- **HTTP Client**: Axios

---

## 📝 Changelog

### v1.1.0 (2026-03-30)

- Added Korean language support
- Completed multi-language translations
- Optimized image path mapping
- Cleaned up redundant API endpoints
- Fixed known issues

### v1.0.0 (2026-03-26)

- Initial release
- AI image generation feature
- Smart splitting feature
- Basic multi-language support

---

## 🤝 Contributing

Issues and Pull Requests are welcome!

1. Fork this repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Submit Pull Request

---

## 📄 License

This project is open-sourced under the [MIT](LICENSE) license.

---

## 📮 Contact

- **Author**: Xiao Zhu
- **Email**: zhuxi0906@gmail.com
- **WeChat**: jakeycis
- **Homepage**: https://banana2.zjhn.com

---

<div align="center">

**⭐ If this project helps you, please give it a Star!**

Made with ❤️ by Xiao Zhu

</div>
