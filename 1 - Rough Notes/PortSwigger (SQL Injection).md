
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

___

### SQL INJECTION EXAMPLES:

- **Original Query:** SELECT * FROM users WHERE username = "haseeb" AND password = "123";
- **Modified Query:** SELECT * FROM users WHERE username = "haseeb" -- ==(This query would let me login to "haseeb" without having to insert any password)==


### BLIND SQL INJECTION:

- Blind SQL injection doesn't return anything in the application. However it can still be used to get access to unauthorized data like passwords.
	- You can trigger out-of-band network interaction using OAST techniques. This is very powerful and works when other techniques fail...(But what is it?)

### SECOND ORDER SQL INJECTIONS:r

- SQL injections which are not executed immediately and stored in the database,
- A reaction from an authorized person later triggers these queries/payload.

___

- It is important to examine the database that you're attacking. SQL is implemented similarly throughout multiple databases however there are a few domains where SQL is changed. For example:
	- String concatenation
	- Comments
	- Error messages

- An SQL injection vulnerability is often useful to find information about the database. The info of database can help you better exploit that vulnerability.
- It is not always necessary that you will be able to find or exploit straightforward SQL vulnerabilities. In most cases nowadays inputs are stored in the form of XML or JSON. However you can still exploit this by encoding your queries in special characters within those XML/JSON responses.


#### References
[[SQL Injection (PortSwigger)]]