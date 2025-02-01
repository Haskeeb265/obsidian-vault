
2025-01-16 16:35

Status: #Finished

Tags: [[cybersecurity]], [[offensive security]] [[tryhackme]]

# Offensive Security Intro

In offensive security, We simulate the a hacker's actions to find vulnerabilities in a system.

We used "GoBuster". It is a tool used to brute force:
- URIs (directories and files) in web sites.
- DNS subdomains (with wildcard support).
- Virtual Host names on target web servers.
- Open Amazon S3 buckets
- Open Google Cloud buckets
- TFTP servers

This is the command that is used to execute GoBuster:
	gobuster -u http://fakebank.thm -w wordlist.txt dir

- **-u** indicates the website that we wants to run GoBuster on
- **-w** is used to point to the file in which you have the words which you want to use in your bruteforce attack.
- **dir** refers to the mode of Gobuster. In the above command we'll be brute forcing directories and files

## CYBER SECURITY ROLES:
- ==Penetration Tester:== Responsible for finding vulnerabilities in technology products
- ==Red Teamer:== Plays the role of a threat and attacks an organization and then providing feedback from the perspective of an enemy
- ==Security Engineer:== Designs, maintains, and monitors security controls over the network to prevent any cyberattacks

#### References
[[Offensive Security Intro]] 