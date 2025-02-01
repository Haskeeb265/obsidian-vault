
2025-01-27 16:21

Status: #Finished 

Tags: [[cybersecurity]] [[CS50]] 

# Securing Accounts (Introduction To Cybersecurity EDX)

## Building Blocks of Security:

1. **Authentication**: Authentication refers to "Who you are". For example, let's say you're Haseeb. Just because you're Haseeb, it doesn't necessarily mean you'd have access to everywhere you go. These are usually IDs, Emails, and Usernames.
2. **Authorization**: Authorization is the process of "Whether you should have access or not". Once a person has authenticated his/her identity, now they would have to give their proof of authorization. This can be anything from passwords to biometrics and so on.

## Some Common Attacks

1. **Dictionary Attack:** A dictionary attack is basically an attacker collecting information on you, storing it into a computer file and then using that file to brute-force your password.
2. **Brute-Force Attacks**: A Brute-Force attack is basically trying all possible combinations in the hope of that one combination will break the password. Passwords of shorter length are more vulnerable to brute-force attack compared to password of longer lengths

------------------------------------------------------------------------


- We have to balance between choosing a password which we can remember easily (usability) and making it hard for the adversary to crack the code (security).
- **NIST** is an organization which standardize cybersecurity including other things.
  - According to NIST, the smallest number of characters in a password should be 8 and the longest should be 64
  - The developers should compare the password of the user to check if it's a commonly compromised password. If it is, give user an alert to choose a better password.
  - Developers should also not give a hint to the user or an unauthorized person. For example: "What's the name of your pet?"
  - After a certain number, the user would be locked out of the device or account

- 2FA revolves around:
  1. Knowledge: Something you can remember
  2. Possession: Something you possess like a security card
  3. Inherence: Something that's part of you like your fingerprint

- **Keylogging** is the process of recording the keystrokes of a person's computer. It is done by first installing a keylogger into the persons' PC which then records and sends the keystrokes back to the adversary's server/PC
- **Credential Stuffing** trying the usernames and passwords that has been breached on another website(S) in hope that the victim is using the same username and password
- **Phishing** is basically doing social engineering but in a more technical way.
- **Machine-in-the-Middle** is basically being vary of machines in the internet such as routers, switches, etc. which might harm you when your information goes through them

---
## Some Security Solutions:

### Single Sign-On (SSO):
It is basically signing up with another account on another website or app such as "Sign in with Google" or "Sign in with Facebook". The presumption here is that since accounts like Google and Facebook are dear to you, chances are you've already set 2FA and secure passwords on them. Since we meet the security criteria, why not just log in with those accounts directly instead of creating or registering a new account.

### Password Managers
Password managers not only save passwords for you but they also create them for you too as well as automatically log you in on legit URLs or the URLs on which you created a password using the password manager. This practice saves us from Phishing attacks as well




#### References
[[Edx CS50 Introduction to CyberSecurity (Securing Accounts)]]