
2024-11-01 16:00

Status: #Started

Tags:
[[cybersecurity]] [[computer security]]
# Introduction to Information Security

In the digital world, your data and your information is the most valuable asset. Hence that's why it should be your utmost priority to keep it safe and secure from attackers and potential threats. 

Information doesn't need to be secure only when it's **stored**. Rather it should also be kept safe when it's **transmitting and processed**.

Information security is basically protection of **Confidentiality, Integrity, and Availability** of our digital assets. This can be done via the implementation of **technology, policy, education, training, and awareness**.


> [!IMP] According to EC-Council
>> Information Security is in the state of well-being of **information** and **infrastructure** in which possibility of theft, tampering, or disruption of information and services is **kept low** or **tolerable**.
>
	The above definition implies that it's not possible to 100% remove the threat of an attack from a system

When we talk about **Security** in information security, we use that term in the sense of **minimizing** the **vulnerabilities**. 

Vulnerability is basically ANY weakness that can be **exploited** by an attacker.

Just like information security, Network and Internet security means to **detect, deter, and correct** any flaws in the TRANSMISSION of information.

We need to rely on cyber security because:
1. Evolution of tech
2. Computers involved in too many of our daily tasks
3. More networks = More area to be exploited

Following are the few impacts of the security breaches of your system:
1. Loss of reputation
2. Low client loyalty
3. Low investor confidence
4. Legal action
5. Monetary loss

---

# Database Security
Another sub domain of Information Security is **Data Security**. It is responsible for the safe keeping of our information. The value of our data motivates the attacker to steal, sabotage, or corrupt it.

*Maintaining CIA triad of our data in the **DBMS** is called Database security.*

Database security can be implemented by with the help of **control approaches**.
These are:
1. Managerial Controls => Policy implementation and Governance. 
2. Physical Controls => Isolating the servers on a room with locked doors and other necessary physical security requirements 
3. Technical Controls => Access control, backup, authentication.

---

# CIA Triad
The CIA Triad is the goals which we need to upheld and look after whenever we're implementing security. Following are the goals that are in CIA triad:
1. **Confidentiality** = Maintaining data secret such that only the intended parties can read it
2. **Integrity** = Keeping the data sent and received authentic without any modification or destruction
3. **Availability** = Timely access to the entities (services) when needed


> [!NOTE] Nonrepudiation
> When a Sender sends a message and then denies it or when a receiver receives a message and then denies it. Nonrepudiation protects both parties in this case. It helps with **authenticity and accountability** (additional security goals)

---

# Classification of Attacks
There are 2 methods of attacking.
## Method #1:
**Passive Attacks**:
- The attacker doesn't directly interact with the parties involved
- Attacker attempts to intercept the **transmitted** message.
- Methods of passive attacks are **spoofing and eavesdropping**
- Passive attacks are almost impossible to detect since neither the sender nor the receiver knows that their message is being interrupted. Hence this is why messages are sent **encrypted**. When dealing with passive attacks, emphasis on **prevention** rather than **detection**
**Active Attacks**:
- Attacker directly interacts with the machine. There are 4 types of active attacks
	1. **Masquerade**: Masquerading is when the attacker impersonates someone to get information out of you through social engineering.
	2. **Replay**: Replay is when the attacker resends a captured packet with the intention of producing an unauthorized effect to the system
	3. **Modification**: Modification is when a message, a part of the message is either altered, reordered, or delayed to produce an unauthorized effect
	4. **DOS**: Denial Of Service prevents the legitimate users from accessing a service. Attackers achieve this by bombarding the servers with GB/s of requests continuously.

Active attacks are hard to **prevents** because there are so many vulnerabilities. That's why we **detect** active attacks and then minimize the disruptions caused by it.

## Method #2:
**Direct Attacks**









#### References
[[Bahria University 7th Semester Lecture 1 Information Security.pdf]]