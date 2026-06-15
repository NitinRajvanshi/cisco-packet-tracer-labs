# Investigate a Threat Landscape

## Objective

This Cisco Packet Tracer lab demonstrates how attackers exploit common cybersecurity vulnerabilities including:

- Network Misconfiguration
- Phishing Attacks
- Ransomware
- Rogue Wireless Access Points
- DNS Hijacking

---

## Part 1: Network Configuration Vulnerability

### Findings

- Guest network was enabled.
- Guests could access internal devices.
- Webcam discovered at IP address 192.168.100.101.
- Router used default admin credentials.
- Guest network security was disabled.

### Risk

Attackers could gain access to devices inside the home network and compromise privacy.

### Mitigation

- Disable guest access to local network.
- Enable WPA2/WPA3 security.
- Change default router credentials.
- Use strong passwords.

---

## Part 2: Phishing Malware Vulnerability

### Phishing Email

Subject:
Urgent - Account Verification Required

The phishing email instructed users to visit:

pix.example.com

### Result

Victims were redirected to a malicious website that launched ransomware.

### Impact

- File encryption
- Data loss
- Operational disruption
- Financial damage

### Mitigation

- Security awareness training
- Email filtering
- Anti-malware solutions
- Regular backups

---

## Part 3: Wireless Network and DNS Vulnerability

### Attack Overview

A rogue wireless network named:

Cafe_WIFI_FAST

was used to lure victims.

### DNS Hijacking

DNS records redirected:

friends.example.com

to the same malicious server used in the phishing attack.

### Attack Flow

1. Victim connects to rogue Wi-Fi.
2. Attacker-controlled DHCP assigns malicious DNS server.
3. DNS requests are redirected.
4. Victim accesses malware website.
5. Ransomware infection occurs.

### Mitigation

- Verify wireless networks before connecting.
- Use trusted DNS services.
- Employ VPN protection.
- Monitor DNS traffic.

---

## Skills Learned

- Vulnerability Assessment
- Wireless Security
- Phishing Analysis
- DNS Security
- Network Hardening
- Cybersecurity Incident Investigation

---

## Tools Used

- Cisco Packet Tracer
- DHCP
- DNS
- Wireless Networks
- Web Browser Simulation
- Email Simulation
