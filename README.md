# CustomWin - Windows Customization Tool

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![PySide6](https://img.shields.io/badge/GUI-PySide6/Qt6-green)
![Windows](https://img.shields.io/badge/Platform-Windows%207|8|10|11-purple)
![Status](https://img.shields.io/badge/Status-Archived%20(2024)-lightgrey)

A modern Windows customization utility with PySide6 GUI, automatic dependency installation, and system tweaking capabilities.

## ✨ Features
- **Smart Installer**: Auto-detects system architecture and installs Python if needed
- **Modern GUI**: Frameless PySide6 interface designed in Qt Designer
- **Multi-Version Support**: Separate optimized versions for Windows 11 and legacy systems
- **System Integration**: Apply registry tweaks and customizations
- **Font Management**: Custom font packages for UI enhancement
- **Quick Launch**: Desktop shortcuts for easy access

## 🚀 Quick Start (Windows Only)
1. Download the repository
2. Run `install.bat` as **Administrator**
3. Follow the on-screen instructions:
   - Select system architecture (32-bit or 64-bit)
   - Choose your Windows version
4. Use the desktop shortcuts to launch the application

## 📁 Project Structure

```
customwin/
├── install.bat              # Smart installer with Python setup
├── SourceCodes/
│   ├── main11.py           # Windows 11 version (PySide6 + Qt Designer)
│   └── main7,8,10.py       # Windows 7/8/10 version
├── UI/
│   ├── Base11.ui           # Qt Designer interface for Windows 11
│   └── [other UI files]
├── Fonts/                  # Custom font packages (.ttf/.otf)
├── Asset/
│   └── A1.reg             # Test registry tweak (changes UI colors)
├── Shortcuts/             # Desktop shortcuts (.lnk files)
│   ├── CustomWin11.lnk    # Shortcut for Windows 11
│   └── CustomWin.lnk      # Shortcut for Windows 7/8/10
└── README.md              # This documentation
```

## 🛠️ For Developers

### Project Architecture
This project demonstrates:
- **PySide6 integration** with Qt Designer .ui files
- **System automation** via batch scripts and registry tweaks
- **Multi-version compatibility** handling
- **Self-contained installation** with dependency resolution

### Key Code Features (main11.py):
- Frameless window implementation
- Dynamic button actions with system integration
- Modular design for easy feature addition
- Safe testing approach with harmless registry tweaks

### Testing Strategy
The included `Asset/A1.reg` file serves as a **safe test case** to verify:
- Button functionality and system command execution
- Registry modification capabilities
- Administrator privilege requirements
- Modular architecture for future tweaks

## 📝 Development Notes
- **Created**: 2024
- **Original Platform**: Windows
- **Current Status**: Archived (project owner transitioned to Linux)
- **Potential**: Can be extended with additional system tweaks and UI enhancements

## 👨‍💻 Author
**sendisdewey** - Initial development and architecture design

---

> 💡 **Note**: This project is open for further development. Feel free to fork and add new features!
