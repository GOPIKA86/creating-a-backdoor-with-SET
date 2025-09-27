NAME: GOPIKA A

REG NO: 212224100017

# creating-a-backdoor-with-SET
creating a backdoor with SET - Ethical Hacking Techniques course

# AIM:
To Create a backdoor with Social Engineering Toolkit (SET)

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode


### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

### Architecture Diagram

```
+----------------+        +------------------------+        +----------------------+
| Attacker's PC  | -----> | SET (Credential        | -----> | Fake Login Page      |
| (Kali Linux)   |        | Harvester via Apache)  |        | (Hosted by SET)      |
+----------------+        +------------------------+        +----------------------+
       |                                                             |
       |                                                             v
       |   1. Configure SET with phishing site (e.g., Gmail clone)   |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Victim's Browser     |
       | <------------------------------------------------| Clicks Phishing Link|
       |                                                 +----------------------+
       |                                                             |
       |                                                             v
       |     2. Victim Enters Credentials → Sent to SET/Attacker    |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Credentials Captured |
       |                                                 | in Apache log/SET DB |
       |                                                 +----------------------+

```

## EXECUTION STEPS AND ITS OUTPUT:
Social Engineering attacks are the various cons used by the hackers to trick people into providing sensitive data to the attackers.

**Steps to Use SET for Phishing (Credential Harvester Attack Method)**

**1. Open terminal:**
```bash
sudo setoolkit
```

<img width="1251" height="869" alt="image" src="https://github.com/user-attachments/assets/abdb2a15-8286-44aa-9de9-83f142386e6b" />

**2. Navigate:**
```bash
1) Social-Engineering Attacks  
2) Website Attack Vectors  
3) Credential Harvester Attack Method
```
<img width="1236" height="705" alt="image" src="https://github.com/user-attachments/assets/e8b7703b-f97d-4176-907c-3dbfd22a24c5" />

**3. Enter your IP address as the attacker server.**

<img width="622" height="51" alt="image" src="https://github.com/user-attachments/assets/7920ea57-fce9-420c-b50f-1253db0f28d0" />

**4. Choose:**
```bash
2) Site Cloner
```
<img width="734" height="291" alt="image" src="https://github.com/user-attachments/assets/97fb8830-be82-4788-a26e-8d319c12deca" />

**5. Enter the URL of the legitimate site ```(e.g., https://accounts.google.com)```**
<img width="1042" height="678" alt="image" src="https://github.com/user-attachments/assets/b158cb16-fa2f-4028-8669-f00f08b90102" />

**6. Send the generated link to the victim.**
<img width="930" height="794" alt="image" src="https://github.com/user-attachments/assets/9e30e059-63d0-4885-9ff3-0f6ea0bdc29b" />

**7. Once the victim logs in → their credentials are stored in:**
```bash
/var/www/html/
```
<img width="739" height="189" alt="image" src="https://github.com/user-attachments/assets/cd62fc0c-b640-4d3e-a58d-1745069cac36" />



## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
