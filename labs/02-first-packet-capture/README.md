# Lab 02 — Capture Your First Packet

## Objective

Use Wireshark to capture and inspect traffic from your own computer.

By the end of this lab, you should be able to:

- Start and stop a packet capture
- Identify basic source and destination information
- Use a simple Wireshark filter

## What You Need

- A computer with internet access
- Wireshark installed
- Download Wireshark from https://www.wireshark.org/download.html

---

## 1. Choose Your Network Interface

Open Wireshark.

Select the interface you are currently using:

- Wi-Fi if connected wirelessly
- Ethernet if connected by cable

You should normally see activity beside the active interface.

<img width="1712" height="873" alt="image" src="https://github.com/user-attachments/assets/43f2c506-807f-4c8d-8cd8-1d9288c9a14a" />

## 2. Capture Some Traffic

Double-click the interface.

Let Wireshark capture traffic for about 10 seconds.

Stop the capture.

Look at these columns:

- Source
- Destination
- Protocol
- Info

<img width="2226" height="1633" alt="image" src="https://github.com/user-attachments/assets/8e0f3e4b-a5e5-4cca-9b06-bc556f6d5b9b" />

## Observe

Can you find:

 - Your own IP address?
 - Other IP addresses?
 - Protocols such as TCP, UDP, DNS or ARP?

Don't worry if you don't understand them yet.

## Capture a Ping

Start a new capture.

Open a terminal and ping your default gateway.

- Windows
ping 192.168.1.1

- Linux/macOS
ping -c 4 192.168.1.1

Replace 192.168.1.1 with your own default gateway.

Stop the capture.

In Wireshark, enter this display filter:

icmp

<img width="919" height="599" alt="image" src="https://github.com/user-attachments/assets/21a55a79-e665-4e31-b88a-3147f1817fbc" />

You should see:

- Echo request
- Echo reply
  
## Questions

- What is the source IP of the Echo Request?
- What is the destination IP?
- What changes in the Echo Reply?
- What would it mean if you saw requests but no replies?


You have now seen traffic created by a command you ran yourself.

Networking is not just diagrams and theory.  You can observe what is actually happening.

What Happens to the Packet Next?

Your computer knows the IP address of the destination.  But on a local Ethernet network, it also needs a MAC address. How does it find it? We will get to that shortly.
