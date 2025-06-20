
2025-02-04 01:20

Status: #Started

Tags: [[cybersecurity]] [[algorithms]] 

# MD5 Message Digest Algorithm

- MD5 allows us to 128 bit compact outputs are created of messages of variable length.
- MD5 is generally used to create digital signatures, compress large file into more concise ones which can then me encrypted using public and secret keys
- MD5 can also be used to verify signatures and detect tempering in messages. It can also be used to generate and verify 128 bit cryptographic hashes.

However, MD5 has well documented flaws and weaknesses and hence this shouldn't be used for security purposes.

- MD5 was quickly recommended to be replaced by cryptographic functions like SHA-1. This was due to it's early "full collision" report
- Despite the flaws, it's still used even though alternates are available.
- In 2008, MD5 was declared "Cryptographically Broken"

**Full Collision:** Two distinct outputs producing the same hash value.
**Birthday Attack:** Exploiting the high probability of collisions using the "Birthday Paradox"

- The birthday paradox states that for n-bit hash, it only takes about 2^(n/2) attempts to find some collisions. In case of MD5 which supported 128 bit, This would be 2^64

==Here's how MD5 works:==
1. Let's assume that we have a message of length **n** and that we intend on finding it's digest message.  
2. Let's assume this is how the words are sequenced:
   m_0 m_1 ... m_{b-1}

Step #1:
Translate the message into bits

Step #2:
Add 1 bit into the original message

Step #3:
Add "k" number of 0s such that the length of the message becomes congruent to 448 mod 512

Step #4:
Append the message in a form of 64bit little endian integer.






#### References
[[MD5]]