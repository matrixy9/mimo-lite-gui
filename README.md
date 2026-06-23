# MiMo Lite GUI

A lightweight local browser GUI for MiMo Code/OpenCode-compatible APIs.

## Download

Download the latest release:

https://github.com/matrixy9/mimo-lite-gui/releases/latest

Choose the package for your system:

- macOS: `mimo-lite-gui-macos.zip`
- Windows: `mimo-lite-gui-windows.zip`
- Linux: `mimo-lite-gui-linux.zip`

Do not use GitHub's green `Code -> Download ZIP` button. That only downloads the repository README, not the GUI release package.

## Requirements

- Node.js 18+
- MiMo CLI installed and configured
- Your own MiMo/API/model credentials

This project does not include API keys, sessions, logs, caches, or model credentials.

## macOS

1. Download `mimo-lite-gui-macos.zip`.
2. Unzip it.
3. Double-click `Open MiMo Lite GUI.command`.
4. Choose the code project folder that MiMo Code should work on.
5. Open `http://127.0.0.1:30143` if the browser does not open automatically.

## Windows

1. Download `mimo-lite-gui-windows.zip`.
2. Unzip it.
3. Double-click `Open MiMo Lite GUI.cmd`.
4. Choose the code project folder that MiMo Code should work on.
5. Open `http://127.0.0.1:30143` if the browser does not open automatically.

## Linux

1. Download `mimo-lite-gui-linux.zip`.
2. Unzip it.
3. Run:

```bash
chmod +x ./open-mimo-lite-gui.sh
./open-mimo-lite-gui.sh
```

4. Choose the code project folder that MiMo Code should work on.
5. Open `http://127.0.0.1:30143` if the browser does not open automatically.

## What Is The Project Folder?

The project folder is the codebase you want MiMo Code to read, edit, and run commands inside. It is not the GUI folder.

The launcher remembers your selected project folder. Delete `.mimo-lite-gui-project` or `.mimo-lite-gui-project.txt` inside the GUI folder if you want to choose a different project next time.

## API / Model Credentials

This GUI does not include or store API keys, sessions, logs, caches, or model credentials.

Configure your API keys and model provider in MiMo CLI first. After MiMo CLI works from your terminal, start this GUI.

## Safety

This release does not include:

- API keys
- Personal sessions
- Logs or caches
- Model credentials
- Native macOS app bundle
- MiMo project history
