# SOC Incident Response Runbook

## Overview
This repository is a collection of **SOC analyst incident response playbooks** built and documented in a controlled lab environment.  
Each playbook demonstrates end-to-end handling of common security incidents — from detection and alerting, to containment, recovery, and lessons learned.  

The goal is to provide practical, hands-on examples of **security monitoring and incident response** across multiple domains:  
- **Endpoint security (SSH brute force, Malware)**
- **Email security (Phishing)**
- **Cloud security (AWS IAM/CloudTrail/CloudWatch)**

All screenshots were generated in lab environments I configured (Splunk, Windows Defender, AWS CloudTrail/CloudWatch).

---

## Table of Contents

| Playbook | Description |
|----------|-------------|
| [SSH Brute Force Playbook](playbooks/ssh_bruteforce.md) | Detection and response to SSH brute force attempts using Splunk and UFW |
| [Phishing Playbook](playbooks/phishing.md) | Analysis and containment of a phishing email with header review and SOC ticketing |
| [Malware Playbook](playbooks/malware.md) | Investigation of malware execution on a Windows endpoint using Defender AV/EDR |
| [Cloud / AWS Security Playbook](playbooks/cloud.md) | Detection and containment of suspicious AWS Console login attempts with CloudTrail and CloudWatch |

---

## Key Features
- **Detection**: Queries, log analysis, dashboards, and alert configurations  
- **Alerting**: Real-time alerts (Splunk, CloudWatch, Defender AV) with email notifications  
- **Containment**: Firewall rules, IAM access restriction, endpoint isolation  
- **Recovery**: System scans, credential resets, MFA enforcement  
- **Lessons Learned**: Playbook notes, tuning recommendations, and hardening guidance  

---

## Why This Project Matters
- Demonstrates **real SOC workflows** across multiple threat vectors  
- Shows experience with **Splunk, AWS CloudTrail/CloudWatch, Windows Defender, and IAM security controls**  
- Organized in a **professional, audit-ready format** suitable for recruiters, mentors, and hiring managers  

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
- [AWS Security Best Practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)  
- [Microsoft Security Documentation](https://learn.microsoft.com/en-us/windows/security/threat-protection/)  
