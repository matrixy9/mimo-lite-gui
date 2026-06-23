# MiMo Lite GUI

A lightweight local browser GUI for MiMo Code/OpenCode-compatible APIs.

## Download

Download the latest release:

https://github.com/matrixy9/mimo-lite-gui/releases/latest

Download the file named:

```text
mimo-lite-gui.zip
```

Do not use GitHub's green `Code -> Download ZIP` button. That only downloads the repository README, not the GUI release package.

## Requirements

- Node.js 18+
- MiMo CLI installed and configured
- Your own MiMo/API/model credentials

This project does not include API keys, sessions, logs, caches, or model credentials.

## macOS / Linux

Download and unzip `mimo-lite-gui.zip`, then run:

```bash
unzip mimo-lite-gui.zip
cd mimo-lite-gui
npm install
MIMO_PROJECT_DIR="/path/to/your/project" npm start
```

Open:

```text
http://127.0.0.1:30143
```

`MIMO_PROJECT_DIR` should point to the project you want MiMo Code to work on, not the GUI folder.

## Windows

PowerShell:

```powershell
Expand-Archive .\mimo-lite-gui.zip
cd .\mimo-lite-gui
npm install
$env:MIMO_PROJECT_DIR="C:\Users\YourName\Projects\your-project"; npm start
```

Open:

```text
http://127.0.0.1:30143
```

`MIMO_PROJECT_DIR` should point to the project you want MiMo Code to work on, not the GUI folder.

## API / Model Credentials

This GUI does not include or store API keys, sessions, logs, caches, or model credentials.

Configure your API keys and model provider in MiMo CLI first. After MiMo CLI works from your terminal, start this GUI from the same terminal environment.

If your MiMo setup uses environment variables for credentials, set them in the same terminal before running `npm start`.

## Use An Existing Backend

If you already started MiMo backend:

```bash
mimo web --port 30142 --hostname 127.0.0.1
```

Run the GUI only:

```bash
MIMO_PROJECT_DIR="/path/to/your/project" MIMO_GUI_START_BACKEND=0 npm start
```

On Windows PowerShell:

```powershell
$env:MIMO_PROJECT_DIR="C:\Users\YourName\Projects\your-project"; $env:MIMO_GUI_START_BACKEND="0"; npm start
```

## Configuration

Optional environment variables:

```bash
MIMO_PROJECT_DIR=/path/to/project
MIMO_GUI_PORT=30143
MIMO_BACKEND_PORT=30142
MIMO_BIN=/path/to/mimo
```

## Safety

This release does not include:

- API keys
- Personal sessions
- Logs or caches
- Model credentials
- Native macOS app bundle
- MiMo project history
