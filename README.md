# c-209 — IP Messenger

A classic local-network messenger with a Python socket server and a Tkinter GUI client, supporting a live user list and chat.

## Features
- TCP socket server that accepts multiple clients concurrently (threading).
- Client GUI to enter your name, view active users, and refresh the list.
- On-demand server command `show list` to enumerate connected users.
- Centralized chat window with message delivery and device-specific buffer sizing.

## Tech Stack
- Python 3
- Standard library: `socket`, `threading`, `tkinter`, `ttk`

## Project Structure
```
PRO-C209-Student-BoilerPlate-main/
├── server.py   # socket server + client handling
└── client.py   # Tkinter messenger client
```

## Installation
- Uses only the Python standard library; no dependencies to install.

## Usage
```bash
# Terminal 1 — start the server
python server.py

# Terminal 2+ — start clients
python client.py
```
1. Enter your name and click "Connect to Chat Server".
2. Use **Refresh** to list users (server sends `show list` data).
3. Type messages in the chat window and send.