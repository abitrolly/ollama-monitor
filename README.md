<p align="center">
  <picture>
    <source srcset="./icons/icon.ico">
    <img src="./icons/icon.ico">
  </picture>
</p>
<div align="center">
  
# Ollama Monitor

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
- 🌐 Comprehensive proxy support with authentication
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
1. Go to [Releases](https://github.com/ysfemreAlbyrk/ollama-monitor/releases)
2. Download latest `OllamaMonitor.exe`
3. Run the executable

### Option 2: Run from Source
1. Clone the repository
```bash
git clone https://github.com/ysfemreAlbyrk/ollama-monitor.git
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Run directly
```bash
python ollama_monitor.py
```

### Option 3: Build from Source
1. Clone the repository and install dependencies (steps 1-2 above)

2. Build executable
```bash
python build.py
```
The executable will be created in the `dist` directory.

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

### I can't see the system tray icon 🤔
If the system tray icon is not visible, you may need to enable it in Windows settings:
1. Press right click on the taskbar and select `Taskbar Settings`
2. Click on `Select which icons appear on the taskbar`
3. Find `OllamaMonitor.exe` and make sure it's turned on

### Settings

To configure the application:
1. Right-click the tray icon
2. Select "Settings"
3. You can customize:
   - API URL (supports proxy with authentication)
   - Run at Windows startup
   - Start with Windows option

Example URLs:
- Direct connection: `http://localhost:11434`
- With proxy: `http://proxy.example.com:8080`
- With proxy auth: `http://username:password@proxy.example.com:8080`

### Logs

Application logs are stored in:
```
%APPDATA%/OllamaMonitor/logs/ollama_monitor_YYYYMMDD.log
```
Please send logs to [GitHub](https://github.com/ysfemreAlbyrk/ollama-monitor/issues) if you encounter any issues.

## 🔧 Development
### Version Management
The version information is centrally managed in `__version__.py`. To update the version:

1. Update the version in `__version__.py`
2. Run `python build.py` to rebuild the executable

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
