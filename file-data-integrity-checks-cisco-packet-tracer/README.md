# File and Data Integrity Checks

## Overview

This project demonstrates how file integrity can be verified after a cyber attack using Cisco Packet Tracer and Cisco Cybersecurity LabVM.

The lab simulates a ransomware attack where multiple client files must be recovered and verified using cryptographic hash functions and HMAC.

---

## Objectives

- Recover files after a cyber attack
- Verify integrity using MD5
- Detect modified files
- Recover files from FTP Backup Server
- Verify files using HMAC SHA-256
- Understand why HMAC is stronger than traditional hashing

---

## Technologies Used

- Cisco Packet Tracer
- Cisco Cybersecurity LabVM
- Ubuntu Linux
- OpenSSL
- FTP
- MD5
- SHA-256
- HMAC

---

## Skills Demonstrated

- Incident Response
- Digital Forensics
- File Integrity Verification
- FTP Operations
- Linux Commands
- Cryptographic Hashing
- HMAC Authentication

---

## Lab Workflow

```text
Cyber Attack
      │
      ▼
Download Hashes
      │
      ▼
Recover Files
      │
      ▼
Generate MD5
      │
      ▼
Compare Hashes
      │
      ▼
Find Modified File
      │
      ▼
Notify Supervisor
      │
      ▼
Recover File via FTP
      │
      ▼
Generate HMAC
      │
      ▼
Verify Integrity
```

---

## Commands Used

### FTP

```bash
ftp hq.corp
dir
get NEclients.txt
quit
```

### MD5

```bash
echo -n 'file contents' | md5sum
```

### HMAC

```bash
openssl dgst -sha256 -hmac cisco123 income.txt
```

---

## Concepts Learned

- File Integrity
- MD5 Hashing
- SHA-256
- HMAC
- FTP Recovery
- Incident Response
- Digital Forensics

---

## Screenshots

### Ransomware Page

<img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/bb8b221c-aeff-4daa-adab-0edadcc70f04" />
<img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/66f262bf-eff2-4dc8-a896-5af0d81b3a82" />



### Hash Verification

<img width="940" height="529" alt="image" src="https://github.com/user-attachments/assets/80df3f60-164a-4602-bcc2-ec1b8989c510" />


### FTP Recovery

<img width="940" height="961" alt="image" src="https://github.com/user-attachments/assets/76571c6f-6ffa-4542-8f83-ff0a45bdf793" />



### MD5 Verification

<img width="940" height="920" alt="image" src="https://github.com/user-attachments/assets/ddf48b13-2a4e-497f-98a7-0263ba2504c0" />


### HMAC Verification

<img width="940" height="464" alt="image" src="https://github.com/user-attachments/assets/1f7beb86-0d00-4ed2-bdcf-b79a35734874" />


---

## Outcome

Successfully recovered compromised files, detected unauthorized modifications using MD5, restored data from the FTP backup server, and verified integrity using HMAC-SHA256.
