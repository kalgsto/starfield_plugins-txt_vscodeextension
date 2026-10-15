# Starfield Plugins Highlighter for VS Code

[![Visual Studio Code](https://img.shields.io/badge/VS%20Code-Extension-007ACC?logo=visualstudiocode)](https://code.visualstudio.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/kalgsto/starfield-plugins/releases)

A dedicated, high-visibility syntax highlighter and load order helper for Bethesda Starfield's `plugins.txt` file.

Designed specifically for modders and players managing their plugins in:
`%LOCALAPPDATA%\Starfield\plugins.txt` (or `%APPDATA%\Local\Starfield\Plugins.txt`).

---
<img width="1161" height="437" alt="image" src="https://github.com/user-attachments/assets/dcdbd8fa-c84c-4cb8-8985-66c92dec1b7e" />

## 🎨 Visual Color-Coding

Instantly tell what is active, what is disabled, and how your load order sections are organized:

| Element | Example | Default Color | Description |
|---|---|---|---|
| **Enabled Mod** | `*sfbgs019.esm` | **Teal / Cyan (`#4EC9B0`)** | Active plugin loaded into Starfield |
| **Disabled Mod** | `Reaper_Action_Hub.esm` | **Red (`#F44747`)** | Inactive / disabled plugin without leading asterisk |
| **Section Dividers** | `_____-added-quests-_____.esm` | **Bold Gold (`#DCDCAA`)** | Category headers and organizer dummy ESMs |
| **Comments** | `# Please do not modify this file.` | **Italic Green (`#6A9955`)** | Comment and note lines |

*(Built-in TextMate scope defaults ensure these colors show up accurately regardless of what color theme you are using).*

---

## ⚡ Features & Productivity Commands

### 1. One-Click File Opener
Never dig through Windows Explorer's hidden AppData folders again!
- Press `Ctrl + Shift + P`
- Select **`Starfield: Open plugins.txt (%LOCALAPPDATA%\Starfield)`**
- Opens your active plugins file instantly in VS Code.

### 2. Fast Mod State Toggle (`Alt + X`)
Enable or disable mods in seconds without manually typing or deleting asterisks:
- Place your cursor on any plugin line (or highlight multiple lines).
- Press **`Alt + X`** (or right-click & choose **Starfield: Toggle Plugin Active State**).
- Toggles between `*Mod.esm` (Active Teal) and `Mod.esm` (Inactive Red).
- Safely skips comment lines and section headers.

### 3. Real-Time Status Bar & Breakdown Statistics
- Displays a live active plugin counter at the bottom of VS Code whenever you view `plugins.txt`.
- Click the counter or run **`Starfield: Show Load Order Statistics`** to view a full breakdown:
  - Active (Enabled) Plugins
  - Inactive (Disabled) Plugins
  - Category Separators
  - Comment Lines
  - Total Load Order Plugins

---

## 💻 Keyboard Shortcuts

| Shortcut | Command | When |
|---|---|---|
| `Alt + X` | Toggle Plugin Active State (`*` on/off) | While editing `plugins.txt` |
| `Ctrl + /` | Toggle Comment (`#`) | While editing `plugins.txt` |

---

## 📦 How to Install

### Method 1: Install via VS Code VSIX (Recommended)
1. Download **`starfield-plugins-1.0.0.vsix`** from the [Releases](https://github.com/kalgsto/starfield-plugins/releases) page.
2. In VS Code, press `Ctrl + Shift + P`.
3. Type and select **`Extensions: Install from VSIX...`**.
4. Choose the downloaded `.vsix` file.

### Method 2: Manual Install
Copy the extension folder into your VS Code extensions folder:
`%USERPROFILE%\.vscode\extensions\fearthereaper.starfield-plugins-1.0.0`

---

## 📄 License

This extension is licensed under the [MIT License](LICENSE).
Created by **fearthereaper** (@kalgsto).
```
