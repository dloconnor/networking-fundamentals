# Lab 01 — Meet Your Network

## Objective - Understand the basic network information configured on your computer.

### What You Will Learn
By the end of this lab, you should be able to identify your:

- IP address
- Subnet mask
- Default gateway
- DNS servers
- MAC address
- Active network interface

Before You Start
You only need:

- A Windows, macOS, or Linux computer
- An internet connection
- A terminal or command prompt
  
## Scenario
Your laptop is connected to a network and can access the internet.  But what information does your computer actually need in order to communicate?

In this lab, we are going to investigate the network configuration your computer is already using.

## Part 1 — Find Your Network Configuration

## Windows
Open Command Prompt and run:

ipconfig /all

## Linux

Run:

ip addr

Then:

ip route

## macOS

Run:

ifconfig

and:

route -n get default

## Questions

Find and write down:

- What is your IP address?
- What is your subnet mask?
- What is your default gateway?
- What DNS servers are configured?
- What is your MAC address?
- Are you connected using Ethernet or Wi-Fi?
- Your computer has an IP address. But your router also has an IP address. Why does your computer need to know the router's address?

## Challenge

Disconnect from your network.

Run the commands again.

Reconnect.

What changed?
