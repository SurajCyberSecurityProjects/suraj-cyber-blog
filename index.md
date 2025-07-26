---
layout: single
title: "Suraj's Cybersecurity Projects Blog"
excerpt: "Hands-on defensive security projects using Splunk, MITRE ATT&CK, and more."
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.3"
  overlay_image: /assets/images/blog-header.jpg
  caption: "Real-world Detection & Response Projects"
---

# 🛡️ Endpoint Threat Detection & Response with Splunk + Windows Defender

A hands-on, real-world project that combines **Splunk (Free version)** and **Windows Defender** to simulate and detect attacker behavior using **MITRE ATT&CK techniques**.  
Built for home lab environments and focused on **EDR (Endpoint Detection & Response)** visibility.

---

## 🧠 Project Overview

This project demonstrates how to detect, visualize, and alert on endpoint-level threats using native Windows logging + Splunk dashboards.

🔍 Core Outcomes:

- Created MITRE-mapped detections  
- Simulated real-world threats (PowerShell, Brute-force, Registry changes)  
- Built a live Splunk dashboard  
- Created custom alerts and documented detection-to-response flow  

---

## ✳️ MITRE ATT&CK Mapping

Mapped techniques to real-world adversary behaviors using MITRE's ATT&CK framework for detection planning:

| Attack Type          | MITRE Technique         |
|----------------------|-------------------------|
| Brute Force          | T1110                   |
| PowerShell Execution | T1059.001               |
| Registry Mod         | T1112                   |

---

## 📜 Log Data Collection (Windows Logs)

Collected endpoint logs using native tools (Event Viewer, Sysmon) and sent them to Splunk:

- Security logs for brute-force and failed login
- PowerShell logs for execution tracking
- Sysmon logs for process, registry, and file events

🖼️ **Failed Login Attempt:**

![Failed login screen](/images/failed-login.png)

🖼️ **PowerShell Log Results:**

![PowerShell log results](/images/powershell-log-results.png)

🖼️ **Registry Modification Detected:**

![Registry modification query results](/images/registry-modification-query.png)


---

## 📊 Custom Dashboards (Splunk)

Interactive dashboards were built in Splunk to visualize attacker behavior in real time.

🖼️ **PowerShell Dashboard Panel:**

![PowerShell Dashboard Panel](/images/powershell-dashboard.png)

🖼️ **Brute-force Dashboard Panel:**

![Brute-force Dashboard Panel](/images/brute-force-dashboard.png)

🖼️ **Final EDR Summary Dashboard:**

![Final EDR Dashboard Screenshot](/images/final-edr-dashboard.png)

---

## 🚨 Custom Alerts & Detection Response Flow

Created Splunk alerts to detect critical behavior such as:

- Repeated failed logins (brute force)  
- Suspicious PowerShell use  
- Registry tampering

Each alert triggered custom actions and was mapped back to MITRE techniques.

🖼️ **Brute Force Alert Configuration:**

![Brute-force Alert Config](/images/brute-force-alert-config.png)

---

## 🔁 Detection to Response Flow (Summary)

1. Simulated attacker behavior on endpoint (PowerShell, failed logins)  
2. Collected logs → Sent to Splunk → Parsed into dashboards  
3. Triggered alerts based on thresholds or suspicious behavior  
4. Documented mapping from threat to detection to analyst action

---

## ✅ Key Takeaways

- Engineered a complete endpoint detection stack using free enterprise-grade tools  
- Enabled real-time threat visibility via MITRE-mapped detections in Splunk  
- Built custom correlation rules for credential access, PowerShell misuse, and persistence threats  
- Simulated realistic attacker behavior to validate detection logic  


---

> 🧠 **Pro Tip**: Want to try this yourself? Spin up a Windows VM, install Splunk Free, simulate basic threats, and watch the logs come alive.

---


