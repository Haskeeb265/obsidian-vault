
2025-07-03 05:31

Status: #InProgress 

Tags:

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
	- First 6 bits = Differentiated Service Code Point




#### References
[[Network Layers and Protocols]]