# Electrobun Skills

A collection of specialized skills for building desktop applications with [Electrobun](https://blackboard.sh/electrobun/) — an ultra-fast TypeScript desktop app framework using Bun and native OS webviews.

## 🚀 Quick Start

Install any skill with a single command:

```bash
npx skills add rajavijayach/electrobun-skills/electrobun
```

Or install specific skills:

```bash
npx skills add rajavijayach/electrobun-skills/electrobun-rpc-patterns
npx skills add rajavijayach/electrobun-skills/electrobun-native-ui
```

## 📦 Available Skills

### Core

#### **electrobun**
Complete guide to building desktop apps with Electrobun. Covers project setup, BrowserWindow, RPC communication, and core APIs.

**Use when:** Starting a new Electrobun project, learning the basics, or need quick reference for core APIs.

```bash
npx skills add rajavijayach/electrobun-skills/electrobun
```

### Specialized Skills

#### **electrobun-window-management**
Advanced window and view management patterns including multi-window apps, BrowserView, window lifecycle, and orchestration.

**Use when:** Building multi-window applications, implementing tab systems, or managing complex window hierarchies.

```bash
npx skills add rajavijayach/electrobun-skills/electrobun-window-management
```

#### **electrobun-rpc-patterns**
Type-safe RPC patterns, bidirectional communication, error handling, and performance optimization for main↔webview communication.

**Use when:** Implementing complex main/webview communication, need type safety, or optimizing RPC performance.

```bash
npx skills add rajavijayach/electrobun-skills/electrobun-rpc-patterns
```

#### **electrobun-native-ui**
Native UI integration including ApplicationMenu, ContextMenu, Tray, native dialogs, and platform-specific patterns.

**Use when:** Adding native menus, system tray, context menus, or platform-specific UI elements.

```bash
npx skills add rajavijayach/electrobun-skills/electrobun-native-ui
```

#### **electrobun-distribution**
Packaging, code signing, auto-updates, notarization (macOS), and cross-platform distribution.

**Use when:** Preparing app for distribution, implementing auto-updates, or setting up code signing.

```bash
npx skills add rajavijayach/electrobun-skills/electrobun-distribution
```

#### **electrobun-debugging**
Development workflow, debugging main process and webview, profiling, and troubleshooting common errors.

**Use when:** Debugging build issues, runtime errors, or optimizing app performance.

```bash
npx skills add rajavijayach/electrobun-skills/electrobun-debugging
```

## 🎯 What are Skills?

Skills are reusable knowledge packages that enhance AI agents with specialized procedural knowledge. They transform general-purpose agents into domain experts.

Each skill contains:
- **SKILL.md**: Core workflows and patterns
- **references/**: Detailed API documentation and guides
- **scripts/**: Reusable code snippets and templates

## 🌟 Features

- ✅ Comprehensive coverage of Electrobun APIs
- ✅ Real-world code examples
- ✅ Progressive disclosure design (concise → detailed)
- ✅ Type-safe patterns and best practices
- ✅ Cross-platform considerations
- ✅ Production-ready patterns

## 📚 About Electrobun

Electrobun is a complete solution for building ultra-fast, tiny desktop applications:

- **TypeScript**: Write your entire app in TypeScript
- **Bun Runtime**: Fast startup (<50ms), small bundles (~14MB)
- **Native Webviews**: Use platform webviews (WKWebView, WebView2, WebKit2GTK)
- **Type-safe RPC**: Bidirectional communication between main and webview
- **Auto-updates**: Tiny delta updates (~14KB)
- **Cross-platform**: macOS, Windows, Linux

Learn more at [blackboard.sh/electrobun](https://blackboard.sh/electrobun/)

## 🤝 Contributing

Contributions are welcome! Please:

1. Follow the [skill-creator guidelines](https://skills.sh/anthropics/skills/skill-creator)
2. Keep SKILL.md concise (<500 lines)
3. Include real-world examples
4. Test skills with AI agents before submitting

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

## 🔗 Links

- [Electrobun Documentation](https://blackboard.sh/electrobun/)
- [Electrobun GitHub](https://github.com/blackboardsh/electrobun)
- [Skills.sh](https://skills.sh/)
- [Discord Community](https://discord.gg/ueKE4tjaCE)

---

Made with ❤️ for the Electrobun community
