# Ollama Monitor

<div align="center">

[![Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Windows](https://img.shields.io/badge/Platform-Windows-blue.svg)](https://www.microsoft.com/windows)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A lightweight system tray application to monitor Ollama AI models with real-time status updates.

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Contributing](#-contributing) • [License](#-license)

</div>

## ✨ Features

- 🔄 Real-time monitoring of Ollama model status
- 🔔 Clean and minimal notifications
- 🚀 Windows startup configuration
- ⚙️ Customizable API connection settings
- 🎯 Color-coded status indicators:
  - 🟢 Green: Model active and running
  - 🔵 Blue: No model running
  - 🔴 Red: Ollama service not running

## 📋 Requirements

- 💻 Windows 10/11
- 🐍 Python 3.8+
- 🤖 [Ollama](https://github.com/jmorganca/ollama) installed and configured

## 🚀 Installation
You need to have [Ollama](https://github.com/jmorganca/ollama) installed and configured 😊
### Option 1: Download Executable
1. Go to [Releases](https://github.com/ysfemreAlbyrk/ollama-monitor)
2. Download `OllamaMonitor.exe`
3. Run the executable

### Option 2: Run from Source
1. Clone the repository
```bash
git clone https://github.com/ysfemreAlbyrk/ollama-monitor
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Run the application
```bash
python ollama_monitor.py
```

### Option 3: Build Executable from Source
1. Clone the repository and install dependencies (follow Option 2 steps)
2. Install PyInstaller
```bash
pip install pyinstaller
```
3. Create executable
```bash
pyinstaller --clean --noconsole --icon=icons/icon.ico --add-data "icons/*.png;icons" --add-data "settings.json;." ollama_monitor.py
```
4. Find the executable in `dist/ollama_monitor` directory

## 📖 Usage

1. Make sure Ollama is installed and running on your system
2. Launch OllamaMonitor
3. The app will appear in your system tray with a color-coded status icon:
   - 🟢 Green: Model active and running
   - 🔵 Blue: No model loaded
   - 🔴 Red: Ollama not running
4. Right-click the tray icon to:
   - View current model status
   - Open settings
   - Exit the application

### Settings

To configure the application:
1. Right-click the tray icon
2. Select "Settings"
3. You can customize:
   - API Host (default: localhost)
   - API Port (default: 11434)
   - Start with Windows option

## 📜 Changelog

See [CHANGELOG.md](CHANGELOG.md) for a list of changes.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- 🚀 [Ollama](https://github.com/jmorganca/ollama) for the amazing AI model runtime
- 🖥️ [pystray](https://github.com/moses-palmer/pystray) for the system tray implementation

---

<div align="center">
Made with ❤️ by Yusuf Emre ALBAYRAK
</div>