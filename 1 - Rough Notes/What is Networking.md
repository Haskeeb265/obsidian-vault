
2025-02-06 03:07

Status: #InProgress 

Tags: [[cybersecurity]] [[tryhackme]] [[networks]] 

# What is Networking

Internet is one giant network which consists of smaller networks
- Smaller networks are called private networks. 
- The networks connecting those smaller networks are called public networks
- A computer is identified by two means: **IP Address** and **Mac Address**
### IP ADDRESSES:
- Stands for Internet Protocol
- Same IP address can be associated to different device (but not at the same time)

This is the structure of an IP Address:
==192.168.1.1==
Where each subsection is an **octet**. In total there are 4 octets and can be in the range ==0-255==

- The IP Address is calculated through ==IP Addressing== and ==Subnetting==. IP can change from device to device but cannot be simultaneously active in the same network more than once.

- IP Addresses follows standards called Protocols.

- IPv4 is 2^32
- IPv6 is 2^128

![[Pasted image 20250206050135.png]]

### MAC ADDRESSES:

- Each hardware on the net is assigned a unique physical address in the factories they're build in. These are called MAC Addresses.
- MAC = Media Access Control
- A MAC consists of in total of 12 characters in hexadecimal divided into groups of 2.

This is what a MAC address looks like:
==a4:c3:f0:53:ac:2f==


-  MAC addresses can be "**Spoofed**". By spoofing we mean that they can be faked. 
- Spoofing happens when another device pretends to have another MAC Address over the network. 




#### References
[[What is Networking (TryHackMe)]]