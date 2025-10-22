# 📋 Frameflow Changelog

All notable changes to Frameflow will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.8.4-1] - 2025-10-22

### ✨ Features
- **Markdown Editor (in-app):** A built-in, split-view Markdown Editor is now available to preview and modify the generated tutorial Markdown directly within the application.
  - Live preview styled like WikiJS (theme-aware: light/dark)
  - Toolbar for common formatting (headers, bold/italic/code, lists)
  - Support for task lists and WikiJS special notes (info/success/warning/danger)
  - Image path resolution so tutorial images render in the preview
  - Changes are saved and used during tutorial finalization

### 🐛 Fixed
- **"Failed to load Python DLL" error:** Fixed first-launch DLL loading error by using permanent runtime directory instead of temporary folder
  - Runtime files now extracted to `%LOCALAPPDATA%\Frameflow\Runtime` (persistent)
  - Disabled UPX compression to reduce antivirus false positives
  - Added runtime directory check on startup
  - See [Troubleshooting Guide](docs/TROUBLESHOOTING_DLL_ERROR.md) for details

---

## [1.8.4] - 2025-10-19

### 🐛 Bug Fixes
- **Fixed:** Screenshots are no longer lost when closing the application  
- **Fixed:** Tutorial recovery now works correctly after unexpected app closure  
- **Fixed:** Work folder is properly preserved for incomplete tutorials  
- **Fixed:** Watermark now applying correctly to images

### 🔧 Improvements
- Tutorials are now **automatically saved after every change**  
- Users can now **load previously created tutorials** directly within the software  
- Enhanced stability for tutorial save/load operations  
- Better error handling during tutorial finalization  


---

## [1.8.3-5] - 2025-10-15

### ✨ Features
- **Watermark Size Control** - Added slider to adjust watermark size (10% to 200%)
- **Structured Logging System** - Centralized logging with diagnostic export and automatic rotation

### 🐛 Fixed
- **Python DLL Error** - Fixed "Failed to load Python DLL" on Windows installation
- **Update Dialogs Dark Theme** - All update dialogs now support dark theme
- **WikiJS Integration Dialog** - Dark theme support
- **Step Deletion Crash** - Fixed undefined error when deleting steps
- **Watermark Position Drift** - Fixed watermark not returning to original position when resizing

---

## [1.8.3-4] - 2025-10-11

### ✨ Features
- **Wiki.js Publication Dialog** - Modern interface to publish tutorials directly to Wiki.js
- **Wiki.js Progress Dialog** - Real-time publication progress with visual feedback
- **Tutorial Persistence** - Tutorial stays loaded after finalization
- **Watermark System** - Add custom watermarks with position and opacity controls

### 🐛 Fixed
- **Watermark Persistence** - Settings now saved when editing images
- **Tutorial Reset** - No longer auto-resets after finalization
- **Wiki.js Image Upload** - Fixed markdown image URLs


---

## [1.8.3-3] - 2025-10-07

### ✨ Features
- **Modern UI Theme System** - Complete light/dark theme implementation
- **Undo/Redo in Image Editor** - Full undo/redo support (Ctrl+Z / Ctrl+Y)

### 🐛 Fixed
- **Zone Displacement Bug** - Zones no longer shift when reopening the image editor

---

## [1.8.3-2] - 2025-10-06

### ✨ Features
- **Integrated changelog** - Recent updates displayed in "Check for Updates" dialog

---

## [1.8.3-1] - 2025-10-06

### 🐛 Fixed
- **Zones shifting** - Fixed blur/highlight/crop zones when reopening editor

---

## [1.8.3] - 2025-09-29

### ✨ Features
- **Wiki.js integration** - Publish tutorials directly to your Wiki.js instance

---

## [1.8.2] - 2025-09-28

### ✨ Features
- **Automatic update system** - Check for new versions with notifications

---

## [1.8.1] - 2025-09-27

### ✨ Features
- **Diagnostic system** - Export system info for troubleshooting

### 🐛 Fixed
- **Theme switching bug** - Fixed UI elements update when changing themes

---

## [1.8.0] - 2025-09-20

### ✨ Features
- **Improved Markdown generation** - Professional format for Wiki.js
- **Auto-maximize mode** for image editor

### 🐛 Fixed
- **Button order** in image editor
- **Capture mode label** color adaptation

---

## [1.7.0] - 2025-09-15

### ✨ Features
- **Drag & drop step reordering** with visual feedback
- **Tutorial persistence** - Save and resume work

---

## [1.6.0] - 2025-09-10

### ✨ Features
- **Screenshot capture** with F9 hotkey
- **Window selection** with thumbnails
- **Image editing tools** - Blur and highlight
- **Dark/Light theme** support

---

## [1.5.0] - 2025-09-05

### ✨ Features
- Initial release with PyQt6

---

## 📝 Version Numbering

Frameflow uses [Semantic Versioning](https://semver.org/):

- **MAJOR** (X.0.0): Breaking changes
- **MINOR** (0.X.0): New features (backward compatible)
- **PATCH** (0.0.X): Bug fixes (backward compatible)

### Version Tags
- **Alpha**: Internal development version
- **Beta**: Public testing version
- **RC**: Release Candidate (pre-release)
- **Stable**: Production version

---

## 🐛 Reporting Issues

To report bugs or request features:

1. Use **Help → Diagnostic Information** to export system info
2. Create a detailed report with reproduction steps
3. Include your Frameflow version and Windows version
4. Attach diagnostic export if applicable

---

## 🏢 About

**Frameflow** - Professional Tutorial Creator  
Developed with ❤️ by Andorrann

Create professional screenshot-based tutorials with automatic markdown generation for Wiki.js and other documentation platforms.
