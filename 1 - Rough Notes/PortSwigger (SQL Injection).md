
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
	- **OR 1=1** or **OR 1=2**: Submitting this would interfere with the logic of the SQL. Through these phrases you can tell the database to validate something as "True" which isn't necessarily true.
	- **Time based Payloads:** We can submit time delay/based SQL queries which basically tells the application to give response in X amount of seconds or minutes. If the response is given in that time then that means that your query was interpreted as an SQL query. If not then there's no vulnerability.
	- **OAST Payloads:** Special payloads submitted that causes the database to make network requests like DNS or HTTP. If the network request is hit then that means that a vulnerability exists in the application

### WHERE SQL INJECTIONS HAPPEN (IN QUERIES):
- Most commonly SQL injection happens in the **WHERE** clause of a **SELECT** query.
- However, it also happens in the following:
	- In the **UPDATE** statements or the **WHERE** clause of the UPDATE.
	- In **INSERT** statements

### COMMON SQL INJECTION EXAMPLES:
#### Retrieving Hidden Data:
- In this SQL injection we modify the SQL query to return additional results. This is often done by the **' --** or the **OR 1=1**. We should be careful when using OR 1=1 because sometimes it can be used by the application in different contexts like **UPDATE** or **DELETE** causing accidental data loss.
#### Subverting Application Logic:
- Subverting application logic is basically manipulating the query in such a way that it asks for something eg: ==username and password== but you only give it a ==username== by completely bypassing the password field making you login as any user.
#### Retrieving Data from Other Database Tables:
- If SQL injection is possible, an attacker can use that to get data from other tables of the database as well.
- This is done by using a **UNION** with your original query and appending another **SELECT** statement to that query.
- **Original Query:** `SELECT name, description FROM products WHERE category = 'Gifts'
- ==Modified Query:== `SELECT name, description FROM products WHERE category = 'Gifts'' UNION SELECT username, password FROM users--` (This query would return all of the username and passwords from the user table as well)

___

### SQL INJECTION UNION ATTACKS:
- You can use **UNION** when the application is vulnerable to SQL injection + it returns the results directly into the application

# GLOSSARY:
1. **OAST:** Out-of-Band Application Security Testing



#### References
[[SQL Injection (PortSwigger)]]