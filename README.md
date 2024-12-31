# Tor Iptables Manager

This script configures and manages iptables rules to route network traffic through the Tor network, providing a level of anonymity. It includes options to load, flush, refresh, or check the public IP address.

## Features

- Load iptables rules to route traffic through Tor.
- Flush iptables rules to default.
- Refresh the Tor circuit to get a new IP address.
- Check the current public IP address.

## Installation
Clone the repository:
```sh
git clone https://github.com/yourusername/tortables.git
cd tortables
```
Install dependencies:
```sh
pip install -r requirements.txt
```

## Usage
Load iptables rules:
```sh
sudo ./tortables.py -l
```
Flush iptables rules:
```sh
sudo ./tortables.py -f
```
Refresh the Tor circuit and get a new IP:
```sh
sudo ./tortables.py -r
```
Check the current public IP address:
```sh
sudo ./tortables.py -i
```
Help:
```sh
sudo ./tortables.py -h
```

## Security Considerations
The script requires superuser privileges to modify iptables rules.
It assumes the presence of the Tor service and the iptables command on the system.
Use with caution and a good understanding of iptables and Tor configuration.

## Contributing
Contributions are welcome! Just submit a pull request.

## License
This project is licensed under the MIT License.
