#  Wireshark - Network Protocol Analyzer

Wireshark is a free, open-source tool used for capturing and analyzing network traffic in real time.  
This README covers the basics of what Wireshark is, how it works, and why it’s useful.


It’s widely used by:
- Network engineers (for troubleshooting)
- Security professionals (for intrusion detection)
- Students & researchers (for learning about protocols)

 Key Features
- Real-time packet capture and deep inspection
- Hundreds of supported protocols
- Powerful **display filters** for isolating traffic
- Color-coded packet listing for quick analysis
- Export captures in multiple formats (`.pcapng`, `.pcap`, `.txt`, etc.)

 Installation
 Windows
1. Download Wireshark from [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html)
2. Run the installer and follow the setup wizard.
3. Optionally install **Npcap** (required for packet capture).

 Linux
bash:
sudo apt update
sudo apt install wireshark

Wireshark uses Display Filters to help you find specific traffic.
| Filter Example         | Purpose                            |
| ---------------------- | ---------------------------------- |
| http                   | Show only HTTP traffic             |
| ip.addr == 192.168.1.1 | Show packets to/from an IP address |
| tcp.port == 443        | Show HTTPS traffic                 |
| dns                    | Show DNS queries and responses     |
| icmp                   | Show ping requests and replies     |

Practical Uses:
Troubleshooting: Identify slow or failed network connections
Security: Detect suspicious activity
Learning: Understand how protocols behave
Testing: Verify network configurations

Limitations:
Cannot capture encrypted payloads without the proper keys
Requires admin/root privileges for capturing live traffic
Large captures may use significant system resources
