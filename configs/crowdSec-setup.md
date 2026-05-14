# CrowdSec Setup

## Purpose

CrowdSec is used to monitor suspicious activity and improve the overall security of the homelab environment through automated protection and threat detection

One of the main reasons for adding CrowdSec was to gain more hands-on experience with security monitoring and understand how detection systems behave in a real Linux server environment

---

## Deployment

CrowdSec was configured alongside the Ubuntu Server environment to monitor system activity and improve overall visibility into potentially suspicious behavior

The setup process included:-
- Installing CrowdSec on Ubuntu Server
- Configuring basic monitoring functionality
- Testing detection behavior
- Reviewing generated alerts and decisions
- Adjusting configurations during testing

---

## Features Used

Current CrowdSec functionality includes:-
- Threat detection
- Monitoring suspicious access attempts
- Community-driven threat intelligence
- Automated decision and protection system
- Basic monitoring of local server activity

---

## Custom Configuration

During testing, some trusted local services and normal activity generated unnecessary alerts and monitoring noise

To improve stability and reduce interference, basic custom whitelist configurations were added for trusted local services such as:-
- Pi-hole
- Tailscale-related activity
- Trusted local devices

This helped improve:-
- Detection accuracy
- Stability for trusted systems
- Reduction of false positives
- Overall usability of the security stack

---

## Lessons During Setup

Working with CrowdSec highlighted how security monitoring can sometimes interfere with legitimate activity if not configured carefully

The setup process helped improve understanding of:-
- False positives
- Whitelisting concepts
- Monitoring behavior
- Service interaction inside a Linux environment

---

## Notes

Sensitive logs, identifiers, and configuration details have been removed from public documentation
