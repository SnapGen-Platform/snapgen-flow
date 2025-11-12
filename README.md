# SnapGen Flow - Configuration & Documentation

> Remote configuration and documentation repository for SnapGen Flow Chrome Extension

[![Chrome Web Store](https://img.shields.io/badge/Chrome-Extension-brightgreen)](https://chrome.google.com/webstore)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## 📋 Overview

This repository hosts the remote configuration files and documentation for **SnapGen Flow**, a powerful Chrome extension for automating Google Veo Flow workflows.

## 🎯 What's Inside

- **`configs/banner-config.json`** - Dynamic configuration for extension banners and tools
- **`docs/`** - User guides, tutorials, and documentation
- **`images/`** - Screenshots and visual assets

## 🔧 Configuration Structure

The extension fetches configuration from `configs/banner-config.json` to dynamically update:

### Banner Content
- Promotional messages and links
- Support channels (Zalo, Telegram)
- Free tier information

### Tools List
- Dynamically add/remove tools
- Update tool descriptions and links
- Control visibility with enable/disable flags

## 📖 Documentation

- [Installation Guide](docs/installation.md) - How to install the extension
- [User Guide](docs/user-guide.md) - Complete usage instructions
- [Features](docs/features.md) - All features explained
- [FAQ](docs/faq.md) - Frequently asked questions

## 🚀 Quick Start

### For Users

1. Install SnapGen Flow from [Chrome Web Store](#)
2. Open any Google Veo Flow page
3. Click the extension icon to start automating

### For Developers

Configuration updates are automatic. The extension:
1. Caches config for 1 hour
2. Fetches fresh updates in background
3. Falls back to defaults if fetch fails

## 🔄 Updating Configuration

Edit `configs/banner-config.json` and commit changes. Extensions will auto-update within 1 hour.

### Example: Add a New Tool

```json
{
  "name": "My New Tool",
  "description": "Tool description here",
  "icon": "Sparkles",
  "color": "#8ab4f8",
  "link": "https://example.com/tool",
  "badge": "new",
  "enabled": true
}
```

### Example: Update Promo Banner

```json
{
  "banner": {
    "promo": {
      "marqueeText": "🎉 New Year Sale: 50% OFF All Tools!"
    }
  }
}
```

## 🛡️ Chrome Store Compliance

✅ **Fully Compliant:**
- Only fetches JSON data (no executable code)
- Works offline with fallback config
- Transparent configuration (public repo)
- No invasive tracking

## 📊 Features

- 🤖 **Automated Workflows** - One-click video generation
- 🎨 **Image Editing** - Built-in image editor
- 📝 **Smart Templates** - Reusable prompt templates
- 🌍 **Multi-language** - English & Vietnamese
- 🎨 **Themes** - Light, Dark, Auto modes
- 📊 **History Tracking** - View all generations

## 🔗 Links

- [Chrome Web Store](#) - Install extension
- [Official Website](https://snapgens.com) - Learn more
- [Support](https://snapgens.com/support) - Get help
- [Changelog](CHANGELOG.md) - Version history

## 💬 Support

Need help? Join our community:

- 💬 **Zalo Group:** [Join here](https://zalo.me/g/qrimzl692)
- 📱 **Telegram:** [Join here](https://t.me/+pob73D0nJ-QwMjhl)
- 📧 **Email:** support@snapgens.com
- 🌐 **Website:** [snapgens.com](https://snapgens.com)

## 📄 License

MIT License - See [LICENSE](LICENSE) file for details

## 🏢 About SnapGens

SnapGen Flow is developed by [SnapGens.com](https://snapgens.com), a platform dedicated to making AI tools more accessible and efficient.

---

**Made with ❤️ by SnapGens Team**
