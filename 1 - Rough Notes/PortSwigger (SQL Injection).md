
2025-07-25 23:43

Status: #InProgress 

Tags: [[cybersecurity]]

# PortSwigger (SQL Injection)

### WHAT IS SQL INJECTION:

- SQL injection is a web security vulnerability which allows an attacker to interfere with the queries that an application makes to its database.
- This can allow the user to make persistent changes to the database.
- A successful SQL injection can possibly lead to access to unauthorized information such as:
	- Passwords
	- Credit card details
	- Personal user information
- SQL injection can also allow an attacker to create a backdoor which would then allow them to have a persistent dormant access to the application which can go unnoticed and may takes eve YEARS to capture and deal with.

___

### WHERE SQL INJECTION IN A QUERY HAPPENS?

- Most commonly, SQL injection happens in **SELECT** and **WHERE**
- However, it can also happen in the following:
	- **UPDATE**
	- **INSERT**
	- **SELECT with ORDER BY**

- There are different types of SQL injections:
	1. Retrieving hidden data
	2. Altering application logic
	3. UNION attacks
	4. Blind SQL injections (output is not shown on the application interface)





#### References
[[SQL Injection (PortSwigger)]]