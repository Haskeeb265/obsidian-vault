
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

- One way hash functions turn string values of arbitrary length into a fixed length. This means that no matter how short or long a password is, the Hash would always be of the same length. 
- You **CANNOT** reverse one-way hash functions. 


## Cryptographic Hash Functions:
Cryptography is all about securing data. Whether it's in transit or at rest.

- Encoding/Encrypt = plaintext -> codetext
- Decoding/Decrypt = codetext -> plaintext

Ciphers are algorithmic in nature.

- Cyphers are well documented and mostly public. The algorithms are out in the open for everyone to see. 
- To keep these ciphers specific to each users, we have a secret piece of information called a **key**
- To establish communication between two connections, the sender as well as the recipient should know each other's keys
- Keys in nature as basically very huge numbers

There are many different types of encryptions.
### Secret-Key Cryptography
- The security of your data relies on the secrecy of your key
- The presumption is that if A wants to send a message to B, then A and B must keep secret whatever key they're using
- This is also known as **Symmetric-Key Encryption**. This means that both A and B will use the same key to decrypt and encrypt
- For B to read A's message, B must know the algorithm as well as the key A used 

## Public Key Cryptography
- Also known as Asymmetric Key Cryptography
- RSA, Diffie-Hellman, MQV 

- Instead of one key, you use 2 keys. Public key and Private key. 
- Anyone over the internet can encrypt a message using YOUR public key. Only YOUR secret key can decrypt a message encrypted by YOUR public key
### RSA:
- Relies on really big prime numbers where **p** * **q** = **n** and p and q are really big prime numbers. This is done so that no one can know what the original p and q were

**To Encrypt**: ==cipher text = m^e mod n== (e = public key)
**To Decrypt:** ==message = m^d mod n== (d = secret key) 
### Key Exchange:

1. Diffie-Hellman: Algorithm for sharing a key. This is how it works
	- ==A = g^a mod p== where   a = private key, g = any number called the generator, p = prime number
	- ==B = g^b mod p== where   a = private key, g = any number called the generator, p = prime number

The values A and B are sent across the internet. Then this formula is applied:
- **s = B^a mod p**
- **s = A^b mod p.**

The above formula gives both parties the same public key

### Digital Signatures:
- DSA, ECDSA, RSA allows you to sign documents digitally (including many more)
-   







#### References
[[Edx CS50 Securing Data (Introduction to Cybersecurity)]]