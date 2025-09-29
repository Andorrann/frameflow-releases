# 📋 Frameflow Changelog

---

## [1.8.2] - 2025-09-28

### 🆕 Added
- **Automatic update system** with GitHub Releases integration
- **Help → Check for Updates** menu for manual update checking
- **Automatic update check** at application startup (5-second delay)
- **Smart version comparison** supporting semantic versioning
- **Update notification dialogs** with changelog preview
- **Background update checking** using separate threads
- **Direct download links** to latest installer from GitHub

### ⚡ Improved
- **Enhanced build system** with `requests` library integration
- **Professional update workflow** with user-friendly notifications
- **Non-intrusive startup checks** with configurable delays
- **Error handling** for network connectivity issues
- **Logging system** for update check activities

### 🔧 Technical
- Added `UpdateService` and `UpdateChecker` classes
- Integrated GitHub API for release information
- Added `requests>=2.28.0` dependency
- Updated PyInstaller configuration for new dependencies
- Enhanced error handling and logging for update operations

---

## [1.8.1] - 2025-09-27

### 🆕 Added
- **Complete diagnostic system** with system info export for technical support
- **Help → Diagnostic Information** menu for troubleshooting
- **Export diagnostic data** as text file or ZIP archive
- **Auto-update system preparation** with GitHub Releases integration
- **Professional build system** with organized scripts and clear structure
- **Automated installer creation** with Inno Setup integration

### 🐛 Fixed
- **Major theme switching bug** - all UI elements now update correctly
- **Step list consistency** during theme changes
- **Complete CSS styles** for light theme with explicit colors
- **Forced widget updates** during theme switching
- **Error handling** improvements across all components
- **Icon path issues** in build system (now uses correct `logo_exe.ico`)

### ⚡ Improved
- **Build system reorganization** - scripts moved to `scripts_build/` directory
- **Clear output directories** - `executable/` and `installer/` instead of `dist/`
- **Menu-driven build process** with options for different build types
- **Professional installer** with proper English localization
- **Enhanced stability** across all modules
- **Performance optimizations** throughout the application
- **Better error messages** and user feedback

### 🔧 Technical
- Refactored theme system architecture
- Enhanced error handling and logging
- Optimized UI component updates
- Prepared infrastructure for automatic updates
- Improved build scripts organization
- Updated Inno Setup configuration

---

## [1.8.0] - 2025-09-20

### 🆕 Added
- **Redesigned Markdown generation** with improved professional format
- **Centralized markdown generator** with hierarchical structure
- **Professional format** compatible with Wiki.js
- **Automatic numbered lists** (1. 2. 3.) for step descriptions
- **Auto-maximize mode** for image editor window

### 🐛 Fixed
- **Button order** corrected in image editor (Cancel → Validate)
- **Coordinate system** reliability with normalized coordinates
- **Capture mode label** color now adapts to theme

### ⚡ Improved
- **Professional tutorial format** following Wiki.js standards
- **Robust window maximization** with fallback geometry
- **Enhanced step descriptions** with numbered list placeholders

### 🧹 Maintenance
- Cleaned up development/test files
- Organized project structure

---

## [1.7.0] - 2025-09-15

### 🆕 Added
- **Modern MVC architecture** with adapters
- **Refactored effect zones management** - simplified and streamlined
- **Robust JSON metadata system**
- **Drag & drop step reordering** with visual feedback
- **Complete context menu** for step management

### ⚡ Improved
- **Modern PyQt6 interface**
- **Tutorial persistence** for work in progress
- **Overall performance** optimizations

---

## [1.6.0] - 2025-09-10

### 🆕 Added
- **Automatic/manual screenshot capture** with F9 hotkey
- **Window detection and selection** with thumbnail previews
- **Image editing tools** (blur, highlight)
- **Automatic markdown generation**
- **Dark/Light theme support**

### 🐛 Fixed
- General stability improvements
- Memory management optimizations

---

## [1.5.0] - 2025-09-05

### 🆕 Added
- Modern PyQt6 interface
- Basic screenshot capture system
- Basic markdown export

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

**Frameflow** - Tutorial Creator  
Developed with ❤️ by Andorrann