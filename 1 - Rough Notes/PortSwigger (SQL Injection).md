
2025-07-25 23:43

Status: #InProgress 

Tags: [[cybersecurity]]

### WHAT IS SQL INJECTION:

- Web security vulnerability that allows an attacker to interfere with the queries made by the application to the database.
- Attackers can even obtain a persistent backdoor into applications through SQL injections which then allows them to stay dormant and perform malicious activities. Such backdoors go unnoticed for years even.

### DETECTING SQL INJECTION VULNERABILITIES:

- We can detect SQL injection vulnerabilities by following a set of tests against every entry point into the application.
- To get started with this we would typically start by submitting:
	- **'**: If the input is not properly validated, submitting a single **'** would give us an SQL error telling us that we can injection queries
	- **OR 1=1** or **OR 1=2**: Submitting this would interfere with the logica


#### References
[[SQL Injection (PortSwigger)]]