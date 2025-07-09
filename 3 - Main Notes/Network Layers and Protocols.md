
2025-07-03 05:31

Status: #Finished 

Tags: [[networks]]

# Network Layers and Protocols

### NETWORKING MODELS:

- There are multiple networking model. Each model has a certain number of vertical layers.

- Arpanet Reference Model = 3 layers
- OSI Model = 7 layers
- Andrew Tanenbaum Model = 5 layers

1. Physical
2. Data
3. Network
4. Transport
5. Application

- Data travels from Application layer of the sender to the Physical layer of the receiver.

- Focusing more on Network and Transport layer

### MOST PROMINENT PROTOCOLS IN NETWORK AND TRANSPORT LAYER:
##### Internet Protocol (IP):

- IP delivers packets from host to destination on the basis of IP address in the packet header.
- It is connectionless; errors like data corruption, packet loss or duplication might occur.
- Packets of connectionless protocols are also called datagrams. 
- IP protocol has 2 variants:
	- IPv4
	- IPv6

###### IPv4 Header:
![[Pasted image 20250703054836.png]]

1. ==(4-bit) Version:== Indicates protocol being used.
2. ==(4-bit) IHL:== (IP Header Length). This is length of the header in 32 bit words. Minimum is 5 words. Maximum is 15 words. Therefore maximum header length = 32x15 = 480bit or 60 bytes.
3. ==(8-bit) Type of Service:== Used to quality of service. Also known as Differentiated Services. 
	- First 6 bits = Differentiated Service Code Point (DSCP)
	- Last 2 bits = Explicit Congestion Notification (ECN); Used to notify the receiver incase of a network congestion.

4. ==(16-bit) Total Length:== Indicates total length of the packet in bytes. Maximum packet length  = 65,535 bytes.
5. ==(16-bit) Identification:== All fragments of the packet have the same Identification number. This allows the receiver to assemble fragmented packets.
6. ==(3-bit) Flags:== First bit is unused. Other 2 bits are DF (Don't Fragment) and MF (More Fragment) bits. DF indicates to the router to not fragment the packet. MF signals that more fragments are about to come. All fragments have MF except for the last one indicating that it's the last fragment.
7. ==(13-bit) Fragment Offset:== Indicates where in the packet this fragment belongs to. Together with MF, this helps in assembling of packets.
8. ==(8-bit) Time to Live:== A counter which limits the life of a packet. Each router decreases this. When it hits 0, the router discards the packets and sends an ICMP error.
9. ==(8-bit) Protocol:== Indicates "next level protocol" being used in the data portion of the packet.
10. ==(16-bit) Header Checksum:== Checksum only on the header only. This is to verify the changing values like Time to Live for example.
11. ==(32-bit Source Address):== Source IP Address
12. ==(32-bit Destination Address):== Destination IP Address
13. ==(variable) Options:== Not used commonly. Only used to flexibly configure your packet. It allows control over how your packet is handled.
14. ==(variable) Data:== Payload of the packet. Data is not part of the header and hence it's not included in the Header Checksum.

______


#### References
[[Network Layers and Protocols]]