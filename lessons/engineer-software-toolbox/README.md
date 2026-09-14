# Quick Lesson — Engineer's Software Toolkit

Every network engineer will have their own preferred software tools, but there are a few core utilities you'll use again and again.

## Connectivity Tools

### ping

`ping` is one of the simplest troubleshooting tools available.  It can help you check whether a destination is reachable and give you an indication of response time.

Example: ping 192.168.1.1

<img width="476" height="208" alt="image" src="https://github.com/user-attachments/assets/25870507-f619-4dd7-970c-613295d5c40d" />

A successful ping tells you that you received a response.

Remember though, No ping reply does not always mean the device is offline.  Firewalls and network devices can block ICMP traffic.

### traceroute / tracert

`traceroute` helps you see the path traffic takes towards a destination.

Windows: tracert 8.8.8.8

Linux/macOS: traceroute 8.8.8.8

This can be useful when trying to understand where traffic is stopping or taking an unexpected path.

## Device Access

### SSH

SSH stands for Secure Shell.  It is commonly used to remotely access routers, switches, firewalls and servers. SSH encrypts the connection, including usernames, passwords and commands. This should normally be your preferred remote access method.

## Network Information

### ipconfig

On Windows: `ipconfig`

or: ipconfig /all

This shows information such as:

- IP address
- Subnet mask
- Default gateway
- DNS servers

## DNS Tools

### nslookup

`nslookup` lets you query DNS.

Example: nslookup openai.com

Useful when trying to work out whether a problem is related to DNS.

### dig

`dig` provides more detailed DNS information and is commonly used on Linux and macOS.

Example: dig openai.com

## Testing Applications

### curl

`curl` allows you to test HTTP and HTTPS connections from the command line.

Example: curl https://example.com

This can help you determine whether a web service is responding without needing to open a browser.

### netstat / ss

These tools show network connections and listening ports on a computer.

Windows: netstat -an

Linux: ss -tuln

These can help answer questions such as:

Is the application listening?  Which port is it using?  Is there already a connection established?

## File Transfer

Network engineers often need to move configuration files, firmware or backups between devices. You may come across:

- SCP
- SFTP
- TFTP
- FTP

Where possible, prefer secure protocols such as SCP or SFTP.  TFTP and FTP are older protocols but are still commonly encountered on network equipment.
