
#  Cyberattack on New York Dam (Bowman Avenue Dam) - Research Summary

This repository provides a detailed overview of the cyberattack on the Bowman Avenue Dam in New York. The attack, carried out in 2013 and disclosed publicly in 2015, was an example of an operational cyberattack targeting critical infrastructure. This document outlines the technical, operational, and strategic aspects of the incident.

##  Category: Operational Technology
---

## Table of Contents

1. [Year of Incident](#year-of-incident)
2. [Risk, Vulnerability, and Threat](#risk-vulnerability-and-threat)
3. [Tactics, Techniques, and Procedures (TTPs) Used](#tactics-techniques-and-procedures-ttps-used)
4. [Post-Measures Taken](#post-measures-taken)
5. [Mitigation Techniques Used](#mitigation-techniques-used)
6. [Similar Past Incidents](#similar-past-incidents)
7. [CIA Triad Compliance](#cia-triad-compliance)
8. [Recommendations for Future Improvements](#recommendations-for-future-improvements)
---

##   Year of Incident
- **Year:** 2013  
- **Public Disclosure:** December 2015

---

##   Risk, Vulnerability, and Threat

### Risk
- Unauthorized access to critical infrastructure.
- Potential manipulation of industrial control systems (ICS).
- Physical disruption to the water management system.

### Vulnerability
- Internet-connected control systems without adequate protection.
- Weak authentication and lack of encryption.
- No proper network segmentation.

### Threat
- A **state-sponsored group from Iran comprising 7 hackers**.
- They were trying to identify and exploit vulnerabilities in U.S. infrastructure.

---

##   Tactics, Techniques, and Procedures (TTPs) Used

| Tactic  (Why)                 | Goal                                                                       |
| ------------------------ | -------------------------------------------------------------------------- |
| **Initial Access**       | Gain entry into the dam's network/control system.                          |
| **Discovery**            | Understand the system layout, control interfaces, and possible weaknesses. |
| **Persistence**          | Maintain long-term access without being detected.                          |
| **Collection**           | Gather intelligence about system configurations and capabilities.          |
| **Impact** *(Attempted)* | Try to manipulate the dam's physical operations (e.g., control the gate).  |


| Technique (how)                             | Description                                                                                              |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **Network Scanning (Reconnaissance)** | Used tools like Shodan to find publicly exposed ICS devices.                                             |
| **Remote Access via Unsecured Ports** | Connected to control systems over the internet using default credentials or weak authentication.         |
| **Credential Guessing / Brute Force** | Attempted to guess usernames and passwords.                                                              |
| **Manual System Inspection**          | Looked around inside the system to understand how controls and sensors work.                             |
| **ICS/SCADA Access Interface**        | Tried to access Human-Machine Interfaces (HMIs) that control physical components (like the sluice gate). |

## Procedure:
1. Use Shodan or similar tools to locate internet-exposed ICS systems.
2. Identify a target with minimal authentication or outdated software.
3. Attempt login with default credentials (e.g., admin/admin).
4. Upon successful login, explore interface panels to learn about dam operations.
5. Maintain a connection to monitor or potentially manipulate the system.
6. Exit quietly without making changes (in this case, the dam gate was offline, preventing action).

---

##   Post-Measures Taken

- FBI and DHS launched forensic investigations.
- Dam’s system was disconnected from the internet.
- Public attribution increased awareness and policy review.

---

##   Mitigation Techniques Used

| **Category**                  | **Mitigation Technique**          | **Description / Action**                                       |
| ----------------------------- | --------------------------------- | -------------------------------------------------------------- |
|  **Network Security**       | Disconnection from Internet       | Air-gapped the dam’s control system to block remote access.    |
|                               | Network Segmentation              | Separated OT and IT networks using firewalls and DMZs.         |
|  **Access Control**         | Strong Password Policies          | Replaced default credentials and enforced password complexity. |
|                               | Multi-Factor Authentication (MFA) | Implemented MFA for accessing sensitive systems.               |
|  **System Hardening**      | Security Patching                 | Updated outdated firmware/software to close vulnerabilities.   |
|  **Monitoring & Detection** | Basic Logging & Alerting          | Introduced basic logging and monitoring mechanisms.            |
|  **Incident Response**      | Incident Response Plan            | Created protocols to respond to future cyber threats.          |
|  **Training & Awareness**   | Initial Awareness Campaigns       | Educated staff on cyber hygiene and attack reporting.          |

---

##   Similar Past Incidents

### A. Ukraine Power Grid Attack (2015)
- Disrupted power to 230,000+ citizens using **BlackEnergy** malware.

### B. Stuxnet Worm (2010)
- Sabotaged Iran's nuclear centrifuges using advanced ICS malware.

### C. Maroochy Shire Sewage Spill (2000)
- Insider exploited wireless access to release raw sewage into public areas.

---

##   CIA Triad Compliance

- **Confidentiality:** Breached – Unauthorized access to critical systems.
- **Integrity:** Threatened – Potential control over dam operations.
- **Availability:** Preserved – No outage occurred (gate offline).

---

##   Recommendations for Future Improvements

| **Category**                  | **Mitigation Technique**                | **Description / Action**                                                                   |
| ----------------------------- | --------------------------------------- | ------------------------------------------------------------------------------------------ |
|  **Network Security**       | Secure Protocols                        | Disable unused ports; enforce secure communication protocols (e.g., SSH, HTTPS).           |
|  **Access Control**         | Least Privilege Principle               | Users only get access to what they need — nothing more.                                    |
|  **System Hardening**      | Disable Unused Services                 | Reduce attack surface by turning off unnecessary system services.                          |
|                               | Secure Configuration                    | Harden device settings according to ICS security standards.                                |
|  **Monitoring & Detection** | Intrusion Detection System (IDS)        | Monitor traffic for suspicious patterns in real time.                                      |
|                               | SIEM (Security Info & Event Management) | Log and analyze events for quicker threat detection.                                       |
|                               | Anomaly Detection (AI/ML)               | Use behavior analysis to detect unusual activity.                                          |
|  **Incident Response**     | Red Team / Blue Team Exercises          | Simulate attack/defense to improve preparedness.                                           |
|  **Training & Awareness**   | ICS Cybersecurity Training              | Educate operators on phishing, malware, and system hygiene.                                |
|                               | Awareness Campaigns                     | Encourage secure behavior and rapid threat reporting.                                      |
|  **Advanced Architecture**  | Zero Trust Architecture                 | Assume no one is trusted — verify everything internally and externally.                    |
|                               | Secure by Design                        | Build ICS (Industrial Control Systems) systems with embedded security controls.           |
|  **Governance & Policy**      | Supply Chain Vetting                    | Ensure third-party vendors follow cybersecurity best practices.                            |
|                               | Threat Intelligence Sharing             | Collaborate across industries to share attack indicators.                                  |

---
