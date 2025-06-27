
2025-06-28 00:35

Status: #InProgress

Tags: [[cybersecurity]]

# Port Scanning

- Ports are used to exchange information 
- Port range = 0 - 65,535
- Ports from 0 - 1023 are called "well-known" ports which are reserved for internet usage. They can also have specialized purposes.
- Ports are managed by TCP and UDP.

Most used and commonly known ports and their purpose:

1. Port 20 (UDP): Used for transferring data (FTP)
2. Port 22 (TCP): SSH used to secure login, FTP and port forwarding
3. Port 23 (TCP): Used to unencrypted communications
4. Port 53 (UDP): DNS which translates DNS names into machine readable IP addresses
5. Port 80 (TCP): Used by HTTP


### Port Scanning Techniques:
1. Ping Scans: Simplest port scanning technique. Also known as ICMP requests. Several ICMP requests are sent to multiple servers in hopes of getting a response.
2. Vanilla Scan: Attempts to connect to all 65,535 ports at the same time. Sends a synchronized SYN flag. It receives an ACK response in back. Easily detectable by firewall
3. SYN Scan: Also known as "half-open scan". Sends an SYN flag and waits for SYN-ACK response. In case of a response from the port, the scanner does not respond back meaning no TCP connection is establis


#### References
