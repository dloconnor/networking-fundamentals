# Quick Lesson — The Network Engineer's Toolkit

You do not need expensive equipment to start learning networking.  A good network engineer mainly needs tools to:

- Observe
- Test
- Connect
- Troubleshoot

---

## Essential Command-Line Tools

You will use these regularly:

- ping        Test basic reachability
- traceroute  See the path traffic takes
- ipconfig    View network settings on Windows
- ip          View network settings on Linux
- arp         View IP-to-MAC mappings
- nslookup    Test DNS
- dig         Query DNS in more detail
- netstat     View network connections
- ss          Modern Linux alternative to netstat
- curl        Test websites and APIs

You do not need to memorise every option.

Learn what question each tool helps you answer.

Packet Analysis
Wireshark

One of the most useful tools you can learn.

Wireshark lets you inspect network traffic and see protocols such as:

ARP
DNS
ICMP
TCP
UDP
HTTP
TLS
tcpdump

A command-line packet capture tool commonly used on Linux servers.

Connecting to Network Devices
SSH

Used to securely connect to routers, switches, firewalls and servers.

Example:

ssh admin@192.168.1.1
Console Cable

Sometimes a device has no working network connection.

A console cable lets you connect directly to it.

This is especially useful when configuring or recovering network equipment.

Building Practice Networks

You do not need a cupboard full of routers and switches.

Network simulators allow you to practise on your computer.

Popular options include:

Cisco Packet Tracer
GNS3
EVE-NG

We will introduce these when we start building larger networks.

Physical Tools

If you eventually work with physical networks, useful tools include:

Laptop
Console cable
Ethernet cables
USB-to-Ethernet adapter
Cable tester
Label maker
Small screwdriver set

More advanced engineers may also use fibre testers and other specialist equipment.

You do not need these to start learning.

The Most Important Tool

The most valuable tool a network engineer has is not hardware or software.

It is a methodical troubleshooting process.

Instead of guessing:

What do I know?

What should be happening?

What is actually happening?

Where does the behaviour change?

What can I test next?

Tools help you collect evidence.

Your job is to interpret it.

Key Takeaway

You do not need dozens of tools.

Start with:

Terminal
ping
traceroute
ipconfig / ip
nslookup / dig
arp
Wireshark
SSH
