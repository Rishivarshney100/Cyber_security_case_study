
# 📄 Cyberattack on New York Dam (Bowman Avenue Dam) - Research Summary

This repository provides a detailed overview of the cyberattack on the Bowman Avenue Dam in New York. The attack, carried out in 2013 and disclosed publicly in 2015, was an example of an operational cyberattack targeting critical infrastructure. This document outlines the technical, operational, and strategic aspects of the incident.

---

## 🗓️ 1. Year of Incident
- **Year:** 2013  
- **Public Disclosure:** December 2015

---

## ⚠️ 2. Risk, Vulnerability, and Threat

### Risk
- Unauthorized access to critical infrastructure.
- Potential manipulation of industrial control systems (ICS).
- Physical disruption to water management.

### Vulnerability
- Internet-connected control systems without adequate protection.
- Weak authentication and lack of encryption.
- No proper network segmentation.

### Threat
- Attributed to a **state-sponsored group from Iran**.
- Aimed to identify and exploit vulnerabilities in U.S. infrastructure.

---

## 🧰 3. Tactics, Techniques, and Procedures (TTPs) Used

- **Reconnaissance:** Scanned public IPs and used platforms like Shodan.
- **Initial Access:** Exploited remote portals with weak/default credentials.
- **Execution:** Attempted interaction with gate control software.
- **Command & Control (C2):** Maintained remote visibility (gate offline at time).

---

## 🔧 4. Post-Measures Taken

- FBI and DHS launched forensic investigations.
- Dam’s system was disconnected from the internet.
- U.S. DOJ indicted **seven Iranian hackers** in 2016.
- Public attribution increased awareness and policy review.

---

## 🛡️ 5. Mitigation Techniques Used

- Network segmentation and firewall implementation.
- Secure VPNs and multi-factor authentication (MFA).
- Regular patching and software updates.
- Cybersecurity training for operators.
- Deployment of IDS and SIEM systems.

---

## 🧾 6. Similar Past Incidents

### A. Ukraine Power Grid Attack (2015)
- Disrupted power to 230,000+ citizens using **BlackEnergy** malware.

### B. Stuxnet Worm (2010)
- Sabotaged Iran's nuclear centrifuges using advanced ICS malware.

### C. Maroochy Shire Sewage Spill (2000)
- Insider exploited wireless access to release raw sewage into public areas.

---

## 🔒 7. CIA Triad Compliance

- **Confidentiality:** Breached – Unauthorized access to critical systems.
- **Integrity:** Threatened – Potential control over dam operations.
- **Availability:** Preserved – No outage occurred (gate offline).

---

## 🚀 8. Recommendations for Future Improvements

- Adopt **Zero Trust Architecture**.
- Use **AI/ML for anomaly detection** in ICS.
- Enable **Cyber Range training** for operational staff.
- Increase **funding and support** for small utilities.
- Secure **supply chains** for hardware/software procurement.
- Conduct **regular red team exercises**.

---

## 📁 File Contents

- `Cyberattack_on_New_York_Dam_Report.docx`: Full research report on the cyberattack.
- `README.md`: Summary and structured documentation.

---

## 🧠 Author Notes

This document was compiled as part of a research project on **operational cyberattacks** and critical infrastructure protection. The case study demonstrates the importance of proactive cybersecurity in ICS environments.

