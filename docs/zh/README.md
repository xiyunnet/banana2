# 云羲AI绘图分影工具 (Nano Banana V2)

**[English](../../README.md)** | **简体中文**

<div align="center">

![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Node](https://img.shields.io/badge/node-%3E%3D16.0.0-brightgreen.svg)

**一键AI图片生成 · 智能切割分影 · 多语言支持**

[在线演示](https://banana2.zjhn.com) · [问题反馈](https://github.com/xiyunnet/banana2/issues)

</div>

---

## 📖 项目简介

云羲AI绘图分影工具是一款基于 Web 的 AI 图片生成与管理工具，支持：

- 🎨 **AI 图片生成** - 支持多种模型、分辨率、比例
- ✂️ **智能切割** - 自动将图片切割为 2/4/6/9 宫格
- 🌐 **多语言支持** - 简体中文、English、繁體中文、日本語、한국어
- 📁 **本地管理** - 图片自动保存到本地目录
- 🔄 **任务管理** - 实时轮询、状态追踪

---

## 🚀 快速开始

### 环境要求

- Node.js >= 16.0.0
- npm 或 yarn

### 安装步骤

```bash
# 克隆仓库
git clone https://github.com/xiyunnet/banana2.git

# 进入目录
cd banana2

# 安装依赖
npm install

# 启动服务
npm start
```

服务启动后访问：http://localhost:2688

---

## ⚙️ 配置说明

### API Key 获取

本项目使用 [Ace Data](https://share.acedata.cloud/r/1uN88BrUTQ) 平台提供的 API 服务：

1. 访问 [Ace Data](https://share.acedata.cloud/r/1uN88BrUTQ) 注册账号
2. 获取 **API Key**（用于图片生成）
3. 获取 **Platform Token**（用于图片上传，可选）

### 后台设置

首次使用请访问设置页面配置：

1. 点击右上角 **设置** 按钮
2. 填写 API Key（必填）
3. 填写 Platform Token（可选，图生图功能需要）
4. 填写大模型 API Key（可选，AI 生成提示词功能需要）

---

## 🌐 多语言支持

| 语言 | 代码 | 状态 |
|------|------|------|
| 简体中文 | zh | ✅ 完成 |
| English | en | ✅ 完成 |
| 繁體中文 | zh-TW | ✅ 完成 |
| 日本語 | ja | ✅ 完成 |
| 한국어 | ko | ✅ 完成 |

---

## 🛠️ 技术栈

- **后端**: Node.js + Express + SQLite
- **前端**: HTML5 + CSS3 + JavaScript (jQuery)
- **图片处理**: Sharp
- **HTTP 客户端**: Axios

---

## 📝 更新日志

### v1.1.0 (2026-03-30)

- 新增韩语支持
- 完善多语言翻译
- 优化图片路径映射
- 清理冗余 API 接口
- 修复已知问题

### v1.0.0 (2026-03-26)

- 初始版本发布
- AI 图片生成功能
- 智能切割功能
- 多语言基础支持

---

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 提交 Pull Request

---

## 📄 许可证

本项目基于 [MIT](../../LICENSE) 许可证开源。

---

## 📮 联系方式

- **作者**: 小潴
- **Email**: zhuxi0906@gmail.com
- **微信**: jakeycis
- **主页**: https://banana2.zjhn.com

---

<div align="center">

**⭐ 如果这个项目对你有帮助，请给一个 Star！**

Made with ❤️ by 小潴

</div>
