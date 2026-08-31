# Node.js Event Logger

A simple event-driven logging system built with Node.js using the built-in `EventEmitter`, `fs`, and `os` modules.

## Features

- Custom event handling with `EventEmitter`
- Timestamped application logs
- Logs stored in a text file
- System memory monitoring
- Automatic memory logging every 3 seconds
- File-based logging using Node.js `fs` module

## How It Works

The application uses an event-driven approach:

```text
logger.log()
     ↓
EventEmitter emits "message"
     ↓
Event listener receives the event
     ↓
logToFile()
     ↓
Timestamp + message
     ↓
eventlog.txt

## How To Run

1. git clone <https://github.com/devgurveer/node-event-logger.git>

2.cd node-event-logger

3.node logger.js

4.eventlog.txt