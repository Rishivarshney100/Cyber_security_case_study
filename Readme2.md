# Florida Water Treatment Facility Cyberattack - 2021

## Overview
This project provides an in-depth analysis of the cyberattack on the Oldsmar, Florida, water treatment facility, which occurred in February 2021. The attack targeted operational technology (OT) systems and posed significant risks to public safety. This README file outlines the incident, risk analysis, tactics, techniques, procedures (TTPs), post-incident measures, mitigation strategies, and improvements that can be made to prevent such attacks in the future.

---

## Table of Contents
- [Incident Overview](#incident-overview)
- [Risk, Vulnerability, and Threat](#risk-vulnerability-and-threat)
- [Tactics, Techniques, and Procedures (TTPs)](#tactics-techniques-and-procedures-ttps)
- [Post-Incident Measures](#post-incident-measures)
- [Mitigation Techniques](#mitigation-techniques)
- [Similar Incidents](#similar-incidents)
- [Categorization as Operational Attack](#categorization-as-operational-attack)
- [Compliance with CIA Triad](#compliance-with-cia-triad)
- [Improvements](#improvements)

---

## Incident Overview
- **Date**: February 5, 2021
- **Location**: Oldsmar, Florida, USA
- **Incident**: Cyberattack on the water treatment facility with the intent to alter water chemical levels.

---

## Risk, Vulnerability, and Threat
- **Risk**: Potential mass poisoning due to the increase of sodium hydroxide in the water supply.
- **Vulnerability**: Exploitation of weak password security and outdated systems, including TeamViewer remote access software.
- **Threat**: Unauthorized remote access by cyber actors aiming to manipulate water treatment chemical dosing.

---

## Tactics, Techniques, and Procedures (TTPs)
- **Initial Access**: Exploitation of remote desktop software (TeamViewer) with weak passwords.
- **Execution**: Manipulation of chemical dosing parameters, raising sodium hydroxide levels from 100 ppm to 11,100 ppm.
- **Persistence**: Potential watering hole attack via a contractor's website.
- **Defense Evasion**: Exploitation of vulnerabilities in operating systems and lack of security measures.
- **Impact**: Potential contamination of the water supply, which was detected and stopped before any damage occurred.

---

## Post-Incident Measures
- **Immediate Response**: Detection and reversal of unauthorized actions by the operator, preventing harm.
- **Investigation**: Involvement of federal agencies such as the FBI and Secret Service to investigate the attack.
- **Public Disclosure**: The City of Oldsmar disclosed the incident to maintain transparency and public trust.

---

## Mitigation Techniques
- **Enhanced Authentication**: Implementation of Multi-Factor Authentication (MFA) for remote access.
- **System Hardening**: Regular updates and patching of software to address known vulnerabilities.
- **Network Segmentation**: Isolation of OT networks from IT systems to minimize attack surface.
- **Access Controls**: Restricting remote access to authorized personnel and monitoring access logs.
- **Employee Training**: Educating staff on cybersecurity best practices and phishing awareness.

---

## Similar Incidents
- **Israel Water Sector Attacks (2020)**: Cyberattacks targeting agricultural water pumps, attempting to alter water flow and chemical levels.
- **Ukraine Power Grid Attack (2015)**: A cyberattack that caused power outages, revealing vulnerabilities in critical infrastructure.

---

## Categorization as Operational Attack
This attack falls under **Operational Attacks** as it targeted the operational technology systems of a critical infrastructure facility, seeking to disrupt essential public services.

---

## Compliance with CIA Triad
- **Confidentiality**: The attack did not compromise sensitive information but exposed the need for secure access controls.
- **Integrity**: The alteration of chemical dosing parameters threatened the integrity of the water supply.
- **Availability**: The swift response prevented the contamination of the water supply, maintaining its availability.

---

## Improvements
- **Advanced Threat Detection**: Implementing anomaly detection systems to identify abnormal activities in real-time.
- **Incident Response Planning**: Developing and testing incident response plans specifically for OT environments.
- **Third-Party Risk Management**: Assessing and securing third-party vendors and contractors with access to OT systems.
- **Regulatory Compliance**: Adhering to industry standards and regulations for OT cybersecurity.

---

## Conclusion
The Oldsmar water treatment facility cyberattack highlights the vulnerabilities within critical infrastructure systems, emphasizing the need for strong cybersecurity measures in operational technology environments. By implementing enhanced authentication, regular patching, and network segmentation, similar attacks can be mitigated in the future.
