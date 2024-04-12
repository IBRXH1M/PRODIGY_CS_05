# Packet Sniffer Tool

The Packet Sniffer Tool is a Python script that captures and analyzes network packets, displaying relevant information such as source and destination IP addresses, protocols, and payload data.

## Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/IBRXH1M/PRODIGY_CS_05.git
    ```

2. Install Python 3.x if you haven't already.

3. Install the required dependencies using pip:

    ```bash
    pip install scapy
    ```

## Usage

1. Open a terminal or command prompt and navigate to the directory containing the `packet_sniffer.py` script.

2. Run the script with administrator privileges:

    ```bash
    python network-packet-analyzer.py
    ```

3. The script will automatically fetch your IP configuration using the `ipconfig` command and start capturing packets on the default interface.

4. Press `Ctrl+C` to stop the packet sniffer.

## Example Output

```
My IP Configuration:
Interface: Ethernet
IPv4 Address: 192.168.1.108
Subnet Mask: 255.265.256.0
Default Gateway: 192.168.0.1
==================================================

Starting packet sniffer...

Ethernet Frame:
Destination MAC: 00:00:5e:00:00:01, Source MAC: 00:00:00:00:00:00, Protocol: 2048
IPv4 Packet:
  Version: 4, Header Length: 20, TTL: 128
  Protocol: 6, Source IP: 192.168.1.1, Destination IP: 192.168.1.104
TCP Segment:
  Source Port: 448, Destination Port: 65127
  Sequence: 1999243897, Acknowledgment: 2700604634
Flags:
  URG: 0, ACK: 1, PSH: 0, RST: 0, SYN: 0, FIN: 0
Data:
b'HTTP/1.1 200 OK\r\nDate: Tue, 13 Apr 2024 00:00:00 GMT\r\nServer: Apache\r\nContent-Length: 15\r\nConnection: close\r\nContent-Type: text/html\r\n\r\nHello, World!\n'
==================================================
```

## Notes

- Running the script requires administrator privileges for raw socket access.
- Use this tool responsibly and ethically. Ensure that you have proper authorization before capturing network packets.
