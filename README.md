<p align="center"><img width=450 alt="RevShellRelay" src="https://github.com/vpanal/revshellrelay/blob/main/assets/revshellrelay.png"></p>

RevShellRelay is a Python script designed to handle communications between an attacker and a victim through sockets, allowing to stabilize a reverse shell to an interactive terminal.

## Features
- Sets up a remote shell with support for attacker reconnection.
- Custom configuration via arguments.

## Requirements
- Python 3.x
- Standard Python libraries: `socket`, `threading`, `argparse`, `sys`, `termios`, `tty`

## Installation
   ```bash
   git clone https://github.com/vpanal/revshellrelay.git
   cd revshellrelay
   ```

## Usage
### Basic example:
```bash
python3 revshellrelay.py --host 0.0.0.0 --port 4444 --host2 0.0.0.0 --port2 5000 -p 12345
```

### Arguments:
- `--host`: IP address of the server to receive the reverse shell (default: `0.0.0.0`).
- `--host2`: IP address for the attacker's client connection (default: `0.0.0.0`).
- `--port`: Port for the data connection (default: `4444`).
- `--port2`: Port for the shell connection (default: `5000`).
- `-p`: Password for authentication (default: `12345`).

### Example with custom parameters:
```bash
python3 revshellrelay.py --host 192.168.1.10 --port 5555 --host2 192.168.1.20 --port2 6000 -p 98765
```

## Demo

<p align="left"><img width=100% alt="Usage demonstration" src="https://github.com/vpanal/revshellrelay/blob/main/assets/demo.gif"></p>

## Security Notes
This script is designed for educational purposes and testing in controlled environments only. **Do not use it on systems without explicit authorization.**

## Contributions
If you want to contribute, fork the repository, make your changes, and send a pull request.

## License
This project is under the MIT License. See the `LICENSE` file for more details.

