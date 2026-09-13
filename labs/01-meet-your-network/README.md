#Lab 01 — Meet Your Network

##Objective - Understand the basic network information configured on your computer.

What You Will Learn
By the end of this lab, you should be able to identify:

1.Your IP address
2.Your subnet mask
3.Your default gateway
4.Your DNS servers
5.Your MAC address
6.Your active network interface

Before You Start
You only need:

A Windows, macOS, or Linux computer
An internet connection
A terminal or command prompt
Scenario
Your laptop is connected to a network and can access the internet.

But what information does your computer actually need in order to communicate?

In this lab, we are going to investigate the network configuration your computer is already using.

##Part 1 — Find Your Network Configuration

##Windows
Open Command Prompt and run:

ipconfig /all

##Linux

Run:

ip addr

Then:

ip route

##macOS

Run:

ifconfig

and:

route -n get default
Questions

Find and write down:

1.What is your IP address?
2.What is your subnet mask?
3.What is your default gateway?
4.What DNS servers are configured?
5.What is your MAC address?
6.Are you connected using Ethernet or Wi-Fi?

Think About It

Your computer has an IP address. But your router also has an IP address. Why does your computer need to know the router's address?

##Challenge

Disconnect from your network.

Run the commands again.

Reconnect.

What changed?

What Happens to the Packet Next?

Imagine you open a browser and try to reach a website.

Your computer now knows its own IP address, subnet mask, default gateway and DNS server.

But before it can send anything...

How does it decide whether the destination is on the local network or somewhere else?

That is what we will investigate next.
