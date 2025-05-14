
#  Cyberattack on New York Dam (Bowman Avenue Dam) - Research Summary

This repository provides a detailed overview of the cyberattack on the Bowman Avenue Dam in New York. The attack, carried out in 2013 and disclosed publicly in 2015, was an example of an operational cyberattack targeting critical infrastructure. This document outlines the technical, operational, and strategic aspects of the incident.

---

##  1. Year of Incident
- **Year:** 2013  
- **Public Disclosure:** December 2015

---

##  2. Risk, Vulnerability, and Threat

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

##  3. Tactics, Techniques, and Procedures (TTPs) Used

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

##  4. Post-Measures Taken

- FBI and DHS launched forensic investigations.
- Dam’s system was disconnected from the internet.
- U.S. DOJ indicted **seven Iranian hackers** in 2016.
- Public attribution increased awareness and policy review.

---

##  5. Mitigation Techniques Used

- Network segmentation and firewall implementation.
- Secure VPNs and multi-factor authentication (MFA).
- Regular patching and software updates.
- Cybersecurity training for operators.
- Deployment of IDS and SIEM systems.

---

##  6. Similar Past Incidents

### A. Ukraine Power Grid Attack (2015)
- Disrupted power to 230,000+ citizens using **BlackEnergy** malware.

### B. Stuxnet Worm (2010)
- Sabotaged Iran's nuclear centrifuges using advanced ICS malware.

### C. Maroochy Shire Sewage Spill (2000)
- Insider exploited wireless access to release raw sewage into public areas.

---

##  7. CIA Triad Compliance

- **Confidentiality:** Breached – Unauthorized access to critical systems.
- **Integrity:** Threatened – Potential control over dam operations.
- **Availability:** Preserved – No outage occurred (gate offline).

---

##  8. Recommendations for Future Improvements

- Adopt **Zero Trust Architecture**.
- Use **AI/ML for anomaly detection** in ICS.
- Enable **Cyber Range training** for operational staff.
- Increase **funding and support** for small utilities.
- Secure **supply chains** for hardware/software procurement.
- Conduct **regular red team exercises**.

---
