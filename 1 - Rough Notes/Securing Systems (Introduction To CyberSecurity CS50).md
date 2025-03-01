
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

- SSL Stripping 





#### References
[[Edx CS50 Securing Systems (Introduction To Cybersecurity)]]