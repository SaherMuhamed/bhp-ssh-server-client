# SSH Server & Client

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)  ![Kali](https://img.shields.io/badge/Kali-268BEE?style=for-the-badge&logo=kalilinux&logoColor=white)  ![Windows](https://img.shields.io/badge/Windows-0078D4.svg?style=for-the-badge&logo=Windows&logoColor=white)  ![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)

This repository contains two Python scripts for implementing a simple SSH server and client using Paramiko library.

## SSH Server

### Overview

The SSH server script (`ssh_server.py`) sets up a basic SSH server that listens for incoming connections, authenticates clients, and executes commands sent by the client.

### Usage

1. Ensure you have Python 3.x installed on your system.
2. Install the required dependencies using `pip install paramiko`.
3. Generate an RSA key pair for server authentication (`test_rsa.key`) or modify the `HOSTKEY` variable to point to an existing RSA key.
4. Run the script (`ssh_server.py`).

## SSH Client

### Overview

The SSH client script (`ssh_rcmd.py`) establishes a connection to the SSH server, prompts the user for commands, sends them to the server, and displays the output received from the server.

### Usage

1. Ensure you have Python 3.x installed on your system.
2. Install the required dependencies using `pip install paramiko`.
3. Run the script (`ssh_rcmd.py`).
4. Enter the server IP address, port (or press Enter for default), username, and password when prompted.
5. Once connected, you can enter commands to execute on the server. Type `exit` to disconnect from the server.

## Screenshot
![](https://github.com/SaherMuhamed/bhp-ssh-server-client/blob/main/screenshot/Screenshot_2024-04-25.png)

## Security Considerations

1. **Authentication:** The server script currently uses simple password authentication. Consider implementing stronger authentication methods such as SSH keys.
2. **Encryption:** SSH communications are encrypted, but ensure proper key management and encryption practices are followed for increased security.


## Acknowledgement
**This python script provided by Black Hat Python - 2nd Edition book for self learning**

## Disclaimer

These scripts provide basic functionality and are intended for educational purposes. They may not be suitable for production environments without further security hardening and testing.
