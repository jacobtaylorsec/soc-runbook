# SOC Incident Response Runbook

## Overview
This repository contains a collection of **SOC analyst incident response playbooks**, each designed and executed in a controlled lab environment.  
Every playbook demonstrates end-to-end handling of security incidents — from **detection and alerting** through **containment, recovery, and executive reporting**.  

The goal is to provide practical, hands-on examples of **security monitoring and incident response workflows** across multiple domains:  
- **Endpoint Security:** SSH brute force, Windows malware execution  
- **Email Security:** Phishing and credential harvesting  
- **Cloud Security:** AWS IAM / CloudTrail / CloudWatch login abuse  

All screenshots were generated in lab environments I configured (Splunk, Windows Defender, AWS CloudTrail/CloudWatch).  
Each playbook now includes **metrics (MTTD/MTTR), SOC tickets, knowledge base entries, and leadership-ready executive summaries**.

---

## Table of Contents

| Playbook | Description |
|----------|-------------|
| [SSH Brute Force](playbooks/ssh_bruteforce.md) | Detection and response to SSH brute force attempts using Splunk and UFW |
| [Phishing](playbooks/phishing.md) | Analysis and containment of a phishing campaign with header review and user communication templates |
| [Malware](playbooks/malware.md) | Investigation of malware execution on a Windows endpoint using Defender AV/EDR |
| [Cloud / AWS Security](playbooks/cloud.md) | Detection and containment of suspicious AWS console login attempts with CloudTrail and CloudWatch |

---

## Key Features
- **Detection & Alerting:** SIEM searches, log analysis, dashboards, and automated alerts  
- **Containment & Recovery:** UFW rules, IAM access restriction, endpoint isolation, MFA enforcement  
- **SOC Process Layers:**  
  - Tier-1 analyst **decision flowcharts**  
  - **User communication templates** for awareness and response  
  - **Metrics tracking (MTTD/MTTR, user reporting rate, impacted users)**  
  - **SOC tickets** with timelines, indicators, impact, and actions  
  - **Knowledge base entries** for training and repeatability  
  - **Executive summaries** for leadership reporting  

---

## Why This Project Matters
- Demonstrates **real SOC workflows** across multiple threat vectors  
- Shows experience with **Splunk, AWS CloudTrail/CloudWatch, Windows Defender, IAM security controls, and phishing analysis**  
- Organized in a **professional, audit-ready format** aligned with NIST 800-61 and SOC best practices  
- Designed to serve as both a **portfolio project for recruiters/hiring managers** and a **training resource for SOC analysts**  

---

## Repository Structure

```
soc-runbook/
├── playbooks/             # Markdown playbooks
│   ├── ssh_bruteforce.md
│   ├── phishing.md
│   ├── malware.md
│   └── cloud.md
├── screenshots/           # Supporting images for playbooks
│   ├── ssh_bruteforce/
│   ├── phishing/
│   ├── malware/
│   └── cloud/
└── README.md              # Main repository overview
```

---

## References
- [NIST 800-61: Computer Security Incident Handling Guide](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf)  
- [Splunk Documentation](https://docs.splunk.com/)  
- [AWS IAM Security Best Practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)  
- [Microsoft Security Documentation](https://learn.microsoft.com/en-us/windows/security/threat-protection/)  
- [CISA Phishing Guidance](https://www.cisa.gov/news-events/news/avoiding-social-engineering-and-phishing-attacks)  

