---
name: Nano-Banana-V2
version: 1.1.0
description: AI image generation and smart splitting tool based on AceData Nano Banana model. Supports multiple resolutions and sizes, automatic 2/4/6/9 grid splitting, waterfall gallery management, and batch download. Supports 5 languages: Chinese, English, Traditional Chinese, Japanese, Korean.
author: Xiao Zhu
email: zhuxi0906@gmail.com
wechat: jakeycis
tags: [ai-image, banana2, nodejs, openclaw, skill, multi-language]
icon: https://ext.zjhn.com/banana2/logo.png
homepage: https://banana2.zjhn.com
repository: https://github.com/xiyunnet/banana2
license: MIT
---

# Nano Banana V2 - AI Image Creation Tool

**English** | **[简体中文](docs/zh/SKILL.md)**

## Overview

Nano Banana V2 is a powerful AI image generation and smart splitting tool based on the AceData Nano Banana series models. It provides a complete web interface for image generation, editing, splitting, and management.

### Core Features

#### 🎨 Image Generation
- **Multiple Models**: Nano Banana Pro, Nano Banana 2
- **Multiple Resolutions**: 1:1 (Square), 16:9 (Landscape), 9:16 (Portrait), 4:3 (Standard), 3:4 (Portrait)
- **Multiple Qualities**: 1K (1024px), 2K (2048px), 4K (4096px)
- **Image-to-Image**: Support up to 6 reference images for editing

#### ✂️ Smart Splitting
- **Multiple Grids**: Support 2/4/6/9 grid splitting
- **Smart Adaptation**: Automatically detect aspect ratio and choose optimal splitting method

#### 🖼️ Gallery Management
- **Waterfall Layout**: Automatically adapt to different image ratios
- **Thumbnail Generation**: Automatic thumbnail creation
- **Batch Download**: Support ZIP packaging
- **File Management**: One-click open file directory

#### 🌐 Multi-Language Support
- **简体中文** (zh)
- **English** (en)
- **繁體中文** (zh-TW)
- **日本語** (ja)
- **한국어** (ko)

#### 🎨 User Experience
- **Dual Themes**: Light/Dark theme switching
- **Real-time Preview**: Image preview, split preview
- **Modern UI**: Frosted glass effect, smooth animations, waterfall layout
- **AI Prompt Generation**: Integrated LLM for intelligent prompt generation

---

## Quick Start

### 1. Install Dependencies

```bash
cd ~/.openclaw/workspace/skills/nano-banana-v2
npm install
```

### 2. Start Service

```bash
npm start
```

### 3. Access Application

Open browser at http://localhost:2688

---

## Configuration

### Get API Key

First-time use requires API Key configuration:
1. Visit: https://share.acedata.cloud/r/1uN88BrUTQ
2. Register and get API Key
3. Fill in API Key in settings page

### Configuration Items

| Item | Required | Description |
|------|----------|-------------|
| API Key | ✅ | For image generation |
| Platform Token | ❌ | For image-to-image feature |
| LLM API Key | ❌ | For AI prompt generation |
| Save Path | ❌ | Image save directory (Default: Desktop/banana2) |

---

## Usage

### Generate Image

1. Enter prompt in the bottom editor
2. Select model, resolution, quality
3. Select splitting method (optional)
4. Click generate button
5. Wait for completion

### Image-to-Image

1. Click upload button to select images (max 6)
2. Enter description
3. Click generate

### AI Prompt Generation

1. Click AI button to open prompt generation window
2. Enter simple description
3. Click generate, AI will create detailed prompt

### View Works

- Click image to view full size
- View split image list
- Download, delete works

---

## Tech Stack

- **Backend**: Node.js + Express + SQLite
- **Frontend**: HTML5 + CSS3 + JavaScript (jQuery)
- **Image Processing**: Sharp
- **API**: AceData Nano Banana API

---

## Directory Structure

```
nano-banana-v2/
├── server/
│   ├── index.js              # Main server
│   └── services/             # Service classes
│       ├── database.js       # Database service
│       ├── request.js        # Request handling
│       ├── task.js           # Task processing
│       └── upload.js         # Upload handling
├── public/
│   ├── index.html            # Main page
│   ├── list.html             # List page
│   ├── set.html              # Settings page
│   ├── components/           # UI components
│   ├── css/                  # Styles
│   ├── js/                   # Application logic
│   └── lan/                  # Language files
├── config/
│   ├── set.json              # Main config
│   ├── system.prompt         # AI system prompt
│   └── cut_*.prompt          # Split prompts
├── database/
│   ├── 1.sql                 # Database init
│   └── 2.sql                 # Database migration
├── package.json
├── README.md
├── LICENSE
└── CHANGELOG.md
```

---

## API Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | /api/get_set | Get config |
| POST | /api/generate | Submit generation task |
| POST | /api/poll/:id | Poll task status |
| POST | /api/upload | Upload image |
| GET | /api/works | Get works list |
| GET | /api/work/:id | Get single work |
| POST | /api/tasks/add | Add task manually |
| POST | /api/admin/delete/:id | Delete work |
| POST | /api/open-folder | Open folder |
| POST | /api/generate-prompt | AI generate prompt |
| POST | /api/shutdown | Shutdown service |

---

## Changelog

### v1.1.0 (2026-03-30)
- Added Korean (한국어) support
- Completed multi-language translation for all components
- Optimized dynamic image path mapping
- Cleaned up redundant API endpoints
- Fixed known issues

### v1.0.0 (2026-03-26)
- Initial release

---

## Open Source Info

- **License**: MIT License
- **Repository**: https://github.com/xiyunnet/banana2
- **Issues**: https://github.com/xiyunnet/banana2/issues
- **Homepage**: https://banana2.zjhn.com

---

## Contact

- **Author**: Xiao Zhu
- **Email**: zhuxi0906@gmail.com
- **WeChat**: jakeycis
