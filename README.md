# DNS-ICMP-Traffic-Analysis__Cybersecurity-Incident-Report

## Description
This project is part of the **Google Cybersecurity Certificate course**, where I worked as a beginner analyst investigating a network issue reported by clients.  
The main task was to analyze **DNS and ICMP traffic logs** captured with `tcpdump` and identify which protocol and service were impacted.  

The issue revolved around users being unable to access the website `www.yummyrecipesforme.com`. My role was to simulate an investigation and write a **Cybersecurity Incident Report** that explains the findings, root cause, and next steps.

---

## Key Features
- Simulation of real-world SOC analyst workflow: **incident detection, investigation, and reporting**.
- Hands-on analysis of **DNS queries** and **ICMP error messages**.
- Identification of **network service disruption** (UDP/DNS – port 53).
- Structured **incident reporting** with timestamps, protocols, and error details.

---

## Tools & Environment
- **tcpdump**
- **Linux CLI**
- **WPS Office**  
- Environment: Course-provided lab environment (simulated traffic capture)

---

## 🚀 Usage
To replicate the analysis:
```bash
# Run tcpdump to capture DNS/ICMP traffic
sudo tcpdump -n -vv -i eth0 port 53 or icmp

# Save capture to a file
sudo tcpdump -n -vv -i eth0 port 53 or icmp -w capture.log

# View logs
less capture.log
