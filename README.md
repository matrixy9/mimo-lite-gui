# MiMo Lite GUI

A lightweight local browser GUI for MiMo Code/OpenCode-compatible APIs.

## Download

Download the latest release:

https://github.com/matrixy9/mimo-lite-gui/releases/latest

## Requirements

- Node.js 18+
- MiMo CLI installed and configured
- Your own MiMo/API/model credentials

This project does not include API keys, sessions, logs, caches, or model credentials.

## Quick Start

Download `mimo-lite-gui.zip` from Releases, then:

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

## Use An Existing Backend

If you already started MiMo backend:

```bash
mimo web --port 30142 --hostname 127.0.0.1
```

Run the GUI only:

```bash
MIMO_PROJECT_DIR="/path/to/your/project" MIMO_GUI_START_BACKEND=0 npm start
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
