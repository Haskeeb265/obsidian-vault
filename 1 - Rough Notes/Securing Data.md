
2025-02-01 18:31

Status: #InProgress

Tags: [[cybersecurity]] [[CS50]]
# Securing Data

## Hashing:
Process of taking an input and storing/converting it into a "hash".
- A Hash is basically a value that is the result of a mathematical algorithm. 

- On server side what happens is that whenever a user signs up, the password's hash value is saved in the database. Next time the user puts in his password to login, the hash of the input password is compared to the stored hash. (The password itself is never compared

- Rainbow tables are CSV files or other files in which the hacker has already stored the hashes of most passwords. With the help of Rainbow table, the adversary would only have to compare his hashes to the hashes of a breached database.  

- Unless there's some randomness in the hashing function, the hash of a 2 same inputs would be the same

- **Salting** is a process in which we give our hash function another input including the data. It's called "Salt". The purpose of salting is to ensure that the same input has different hash value.
- According to NIST, stored passwords should be salted and hashed in a form that is resistant to offline attacks. They should be salted and hashed using a **one way** key derivation function.





#### References
[[Edx CS50 Securing Data (Introduction to Cybersecurity)]]