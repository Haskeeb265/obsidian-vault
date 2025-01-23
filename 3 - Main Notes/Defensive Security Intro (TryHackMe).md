
2025-01-18 17:54

Status: #Finished 

Tags: [[defensive security]] [[cybersecurity]]

# Defensive Security Intro (TryHackMe)

Defensive security mainly covers these 2 tasks:
1. Preventing intrusions from occurring
2. Detecting intrusions when they occur and respond properly

Defensive security is handled by Blue Teams

Defensive Security responsibilities includes:
- Training users and spreading awareness about cybersecurity.
- Documenting and managing assets: This includes the devices that we need to manage and protect adequately
- Updating and patching any vulnerabilities
- Setting up preventive security devices such as firewalls
- Setting up logging and monitoring devices.


## Security Operations Center (SOC)

A SOC is a team of cybersecurity specialists which monitor the network to see any malicious activities.

SOC's areas of interests are:
- Vulnerabilities
- Network intrusions
- Unauthorized activity
- Policy violations

SOC covers various tasks to ensure security. One such task is **Threat Intelligence**:
### Threat Intelligence:

- Intelligence refers to the information you gather about actual and potential enemies. A threat is any actions which can negatively affect the system.
- Threat intelligence helps companies better understand how to deal with their adversaries. Each company has different type of adversaries.
- Intelligence needs data. Data is collected from local sources such as network logs and public sources such as forums. This data needs to be collected, processed, and analyzed. The analysis phase seeks to find more information about the enemy. It helps create a list of recommendation and actionable steps

### Digital Forensics And Incident Response (DIFR):

In DIFR, we cover:
- Digital Forensics
- Incident Response
- Malware Analysis

#### Digital Forensics:

Digital forensics is the process of investigating crimes and establish facts while preparing evidences which are presentable in court.

In defensive security, the focus of forensics is evidence after an attack. It focuses on different areas such as:

1. File System: Analyzing low level copy (image) of a system.
2. System Memory
3. System logs
4. Network Logs

### Incident Response:

Incident response is the methodology which is to be followed when an *incident* occurs. The aim is to reduce the damage and recover in as little time as possible.

Here are the 4 major phases of incident response:
1. Preparation
2. Detection and Analysis
3. Containment, Eradication, and Recovery
4. Post-Incident Activity

## Malware:

Malware is malicious software. It can be anything such as software, files, and documents that are saved on your hard disk and can be shared over the network. There are different types of malware:

-  **Virus:** A program attached to a file. It's purpose is to make the computer slow till its unusable. It is designed to spread from one computer to another. It works by overwriting, deleting, and altering the files on the infested PC
- **Trojan Horse:** Usually attached to a usable software such as video player or editor. Underneath which dangerous code lurks. Once the program is installed, the malware is also installed in your PC
- **Ransomware:** Encrypts the files of the victim and asked for money in return for the key of the encrypted files.

> [!NOTE] IP Address
> 	An IP address is like a home address for your computer on the PC. Your IP address tells the other computers where to send the information that you request.
> New or Unknown IP Address's mean someone suspicious or new to the network is trying to get access

#### References
[[Defensive Security Intro]]