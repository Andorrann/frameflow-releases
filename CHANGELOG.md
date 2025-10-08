# 📋 Frameflow Changelog

---

## [1.8.3-3] - 2025-10-07

### ✨ Features
- **Modern UI Theme System** - Complete light/dark theme implementation with soft colors
- **Improved Step Visualization** - Steps now feature blue accent bars for better separation
- **Adaptive Borders** - Ultra-discrete borders that adapt to the selected theme
- **Undo/Redo in Image Editor** - Full undo/redo support with keyboard shortcuts (Ctrl+Z / Ctrl+Y)
- **Zone Re-editing** - Edit zones multiple times before tutorial finalization without displacement

### 🐛 Fixed
- **Theme Application** - Theme now correctly applies on startup
- **Dark Theme Borders** - Fixed overly bright borders in dark mode
- **Zone Displacement Bug** - Zones no longer shift when reopening the image editor

### 🔄 Rework
- **UI Spacing & Layout** - Optimized component spacing for better visual hierarchy
- **Step List Design** - Redesigned step items with modern styling and hover effects
- **Image Editor Controls** - Modern undo/redo buttons with visual feedback

---

## [1.8.3-2] - 2025-10-06 (Hotfix)

### 🆕 Added
- **Integrated changelog** - Recent updates now displayed directly in "Check for Updates" dialog
- **Smart display** - Shows last 3 versions automatically with proper styling

### ♻️ Changed
- **Removed standalone changelog menu** - Changelog now integrated with update checker for cleaner UX

---

## [1.8.3-1] - 2025-10-06 (Hotfix)

### 🐛 Fixed
- **Fixed blur/highlight/crop zones shifting** when reopening image editor or finalizing tutorial
- **Added changelog viewer** in Help menu for easy access to release notes

---

## [1.8.3] - 2025-09-29

### 🌐 Added
- **Wiki.js integration** - Publish tutorials directly to your Wiki.js instance
- **Automatic image upload** with seamless link replacement
- **One-click publishing** from tutorial completion dialog

---

## [1.8.2] - 2025-09-28

### 🆕 Added
- **Automatic update system** - Check for new versions from Help menu
- **Auto-update check** at startup with notifications
- **Direct download links** to latest installer

---

## [1.8.1] - 2025-09-27

### 🆕 Added
- **Diagnostic system** - Export system info for troubleshooting (Help menu)

### 🐛 Fixed
- **Theme switching bug** - All UI elements now update correctly when changing themes

---

## [1.8.0] - 2025-09-20

### 🆕 Added
- **Improved Markdown generation** with professional format compatible with Wiki.js
- **Auto-maximize mode** for image editor window

### 🐛 Fixed
- **Button order** in image editor (Cancel → Validate)
- **Capture mode label** color adaptation to theme

---

## [1.7.0] - 2025-09-15

### 🆕 Added
- **Drag & drop step reordering** with visual feedback
- **Context menu** for step management
- **Tutorial persistence** - Save and resume work in progress

---

## [1.6.0] - 2025-09-10

### 🆕 Added
- **Screenshot capture** with F9 hotkey (automatic/manual modes)
- **Window selection** with thumbnail previews
- **Image editing tools** - Blur and highlight areas
- **Markdown generation** for tutorials
- **Dark/Light theme** support

---

## [1.5.0] - 2025-09-05

### 🆕 Added
- Initial release with PyQt6 interface
- Screenshot capture
- Markdown export

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
