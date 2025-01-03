# AgentSmith

Network packet analyzer for Closers game, supporting TCP/UDP traffic inspection and custom packet definitions.

## Features

- TCP/UDP packet capture and analysis
- Custom packet definition format (.yuil)
- Packet capture saving/loading
- GUI built with Gioui
- Real-time packet inspection

## Installation

```bash
go get github.com/yuilmuil/agentsmith
```

## Requirements

- Go 1.20 or higher
- Gioui library
- libpcap/npcap (for packet capture)

## Usage

```bash
./agentsmith
```

The GUI will launch, allowing you to:
- Select network interface
- Start/stop packet capture
- View packet details
- Save/load packet definitions

## Packet Definitions

AgentSmith uses .yuil files to store packet definitions. Example format:

```yuil
packet:
  name: "LoginRequest"
  id: 1001
  fields:
    - name: "username"
      type: "string"
      length: 32
    - name: "password"
      type: "string"
      length: 64
```

## Current Status

This project is in early early early development. Features and APIs may change significantly.

## License

GNU GENERAL PUBLIC LICENSE

## Contributing

Pull requests welcome. Please see CONTRIBUTING.md for guidelines.
