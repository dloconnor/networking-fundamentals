# Lab 02 — Capture Your First Packet

## Goal

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

<img width="1716" height="883" alt="image" src="https://github.com/user-attachments/assets/82dff694-be0a-4fb0-ae32-0fa57f8a6ad5" />


## 2. Capture Some Traffic

Double-click the interface.

Let Wireshark capture traffic for about 10 seconds.

Stop the capture.

Look at these columns:

Source
Destination
Protocol
Info

Source
Destination
Protocol
Info

## Observe

Can you find:

 -  Your own IP address?
 - Other IP addresses?
 - Protocols such as TCP, UDP, DNS or ARP?

Don't worry if you don't understand them yet.

3. Capture a Ping

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

You should see:

Echo request
Echo reply
Questions
What is the source IP of the Echo Request?
What is the destination IP?
What changes in the Echo Reply?
What would it mean if you saw requests but no replies?
Think About It

You have now seen traffic created by a command you ran yourself.

Networking is not just diagrams and theory.

You can observe what is actually happening.

What Happens to the Packet Next?

Your computer knows the IP address of the destination.

But on a local Ethernet network, it also needs a MAC address.

How does it find it?

We will get to that shortly.

## Observe

Can you find:

 -  Your own IP address?
 - Other IP addresses?
 - Protocols such as TCP, UDP, DNS or ARP?

Don't worry if you don't understand them yet.

3. Capture a Ping

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

You should see:

Echo request
Echo reply
Questions
What is the source IP of the Echo Request?
What is the destination IP?
What changes in the Echo Reply?
What would it mean if you saw requests but no replies?
Think About It

You have now seen traffic created by a command you ran yourself.

Networking is not just diagrams and theory.

You can observe what is actually happening.

What Happens to the Packet Next?

Your computer knows the IP address of the destination.

But on a local Ethernet network, it also needs a MAC address.

How does it find it?

We will get to that shortly.
