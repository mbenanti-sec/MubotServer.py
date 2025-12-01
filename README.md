# MubotServer.py
Minimal TCP server using Python’s socketserver that prints what a client sends and replies with the same data in uppercase.

MubotServer is a minimal TCP server that demonstrates handling incoming
connections from simple "bots" using Python's socketserver framework.
When a client connects, the server prints the received data and responds with
the same data in uppercase.

Features

Listens on TCP port 8000 by default

Prints the client's IP address and raw data

Sends back the uppercase version of the received data

Requirements

Python 3 (standard library only, no external dependencies)

Install:

No extra installation required beyond Python 3.

Usage
python3 MubotServer.py

By default the script uses:

HOST, PORT = "", 8000


Example test with nc:

nc <server_ip> 8000
Hello from client


The server output:

Bot with IP 192.168.1.100 sent:
b'Hello from client'


The client receives:

HELLO FROM CLIENT


Disclaimer

This project is for educational purposes and to demonstrate basic
client–server communication in Python. It is not intended to be used as a
production server.
