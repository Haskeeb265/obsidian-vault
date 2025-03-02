
2025-03-02 03:26

Status: #InProgress 
 
Tags: [[CS50]] [[cybersecurity]] [[academia]] 

# Securing Systems (Introduction To CyberSecurity CS50)

- If you're only using HTTP, you're vulnerable to Machine-in-the-Middle Attacks
- The servers can read your actual information in HTTP protocol
- Packet Sniffing is basically peeking inside the packets that is being sent over the internet. Through packet sniffing the attacker can read your unencrypted data as well as modify your packet as well
- Cookies are basically used to remember the user who has once logged into a website. So instead of asking the user to login again and again, the server "remembers" the users by their cookies (sessions)
- Cookies save you from session hacking
- HTTPS keeps the content inside your packets encrypted
- TLS is a protocol used for HTTPS. It basically gives digital certificates to legitimate sites. It consists of a public key, name of the website, how long it is valid for
- TLS certificates are basically of type **X.509**

- In HTTPS, the browser first downloads the certificate and calculates it's hash value. 
- The browser then takes the signature on the certificate of the CA (Certified authority) as well as it's public key and runs it through an algorithm. The output should be the same as the hash value of the certificate if it's legit

- SSL Stripping is basically when you're using HTTP. The browser redirects you to a "safe" URL. That URL is generally sent back to you by a Man-in-the-Middle machine and is commonly the adversary's own website.
- You can use protocols like HSTS (HyperText Strict Transport Security). What it does is that it includes additional instructions to the packet header which solidifies the security futher. For example it can include in the server to only use HTTPS protocol for sub domains as well. 
- HSTS can also "preload" your websites into the browser's source code such that if you for example download chrome, it'll be in Chrome's source code to pair your website with HTTPS only.

- VPNs encrypt ALL your information between you and the VPN server
- SSH is about connecting to a remote server and executing commands on it. You can connect on another server and type commands on it while the entire interactions stays encrypted

- Ports tell the computer which packets offer which services. For example a packet destined for port 80 would be following HTTP protocol, a packet for port 443 would be following HTTPS and so on
- A threat to ports is a **PORT SCANNING** in which all the ports are scanned on a server between 0-65,000 to discover which ports are open to communication

- Firewalls are used to keep unintended internet traffic at bay.
- One of the ways the firewall blocks traffic is based on IP Addresses.
- Another way is Deep Packet Inspection. In this the firewall can actually see what's inside your packet. This way it can more effectively block bad traffic to your network or computer.
- Deep Packet Inspection can be implemented using Proxy servers which mimic a man-in-the-middle attack. 




#### References
[[Edx CS50 Securing Systems (Introduction To Cybersecurity)]]