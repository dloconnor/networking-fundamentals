# Lab 03 — ARP: Who Has This IP?

## Goal

See how your computer discovers the MAC address of another device on the local network.

You will learn:

- What ARP does
- The difference between an IP address and a MAC address
- How ARP requests and replies work

---

## 1. View Your ARP Table

### Windows

arp -a

### Linux
ip neigh

### macOS
arp -a

Look for the IP address of your default gateway.

Can you see a MAC address beside it?

## 2. Capture ARP Traffic

Open Wireshark and start a capture.

Use this display filter:

arp

<img width="850" height="304" alt="image" src="https://github.com/user-attachments/assets/79bf0159-7ac6-4b9f-a3a7-14b94f172eca" />


Now ping your default gateway.

You may see something like:

Who has 192.168.1.1?
Tell 192.168.1.20

followed by:

192.168.1.1 is at aa:bb:cc:dd:ee:ff

## Questions
- What IP address is your computer looking for?
- Who sends the ARP request?
- Who replies?
- What information does the reply contain?

Your computer already knew the gateway's IP address.  So why did it need to discover its MAC address?

Because on the local network:

- IP identifies the destination logically.
- MAC identifies where the Ethernet frame should be delivered.

## Key Takeaway

ARP answers a simple question:

- I know the IP address. What is the MAC address?


