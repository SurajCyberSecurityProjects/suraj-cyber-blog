---
layout: home
title: "Suraj's Cybersecurity Projects Blog"
excerpt: "Hands-on defensive security projects using Splunk, MITRE ATT&CK, and more."
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.3"
  overlay_image: /assets/images/blog-header.jpg
  caption: "Real-world Detection & Response Projects"
---

Welcome to my cybersecurity blog. Explore hands-on detection and response labs using MITRE ATT&CK, Splunk, Windows Defender, and more.


# 🛡️ Endpoint Threat Detection & Response with Splunk + Windows Defender

A hands-on, real-world project that combines **Splunk (Free version)** and **Windows Defender** to simulate and detect attacker behavior using **MITRE ATT&CK techniques**. Built for home lab environments and focused on **EDR (Endpoint Detection & Response)** visibility.

---

## 🧠 Project Overview

This project demonstrates how to detect, visualize, and alert on endpoint-level threats using native Windows logging + Splunk dashboards.

🔍 Core Outcomes:

- Created MITRE-mapped detections  
- Simulated real-world threats (PowerShell, Brute-force, Registry changes)  
- Built a live Splunk dashboard  
- Created custom alerts and documented detection-to-response flow

---

## 🌿 MITRE ATT&CK Mapping

| Technique    | Name                          | Description                             |
|-------------|-------------------------------|-----------------------------------------|
| T1059.001   | PowerShell Execution           | Detects suspicious PowerShell usage     |
| T1110.001   | Brute-force Login Attempts     | Identifies multiple failed logins       |
| T1112       | Registry Modification          | Flags unauthorized registry changes     |

---

## ⚡ PowerShell Abuse Detection (T1059.001)

### 🔍 Raw Log Sample

![PowerShell Logs](/assets/images/Powershell%20log%20results.png)

We ran recon commands (e.g., `whoami`, `Get-Process`) to simulate attacker behavior. These generated logs were ingested into Splunk.

### 📊 Dashboard Panel

![PowerShell Dashboard](/assets/images/Powershell%20Dashboard%20Panel.png)

---

## 🚨 Brute-force Detection (T1110.001)

### 🔍 Failed Login Attempts

![Failed Logins](/assets/images/failed-login-screen.png)

This detection captured multiple invalid RDP/console login attempts from the same source within a short time window.

### 📊 Brute-force Dashboard

![Brute-force Panel](/assets/images/brute-force-dashboard-panel.png)

---

## 🛠️ Registry Modification Detection (T1112)

### 🔍 Raw Registry Log

![Registry Log](/assets/images/Registry%20modification%20query%20results.png)

Changes to sensitive registry keys (such as `Run` and `RunOnce`) were captured and visualized.

---

## 📊 Final EDR Dashboard

![EDR Dashboard](/assets/images/Final_EDR_Dashboard_Screenshot.png)

---

## 📌 Key Learnings

- Splunk Universal Forwarder setup on Windows VM  
- Ingested Event Logs + Defender Logs  
- Used MITRE ATT&CK to structure detection logic  
- Simulated threats to test EDR visibility  
- Built real-time dashboards and alerts  

---

## 💬 Let’s Connect

Want to discuss more about SOC, EDR, or threat detection?

👉 [Connect with me on LinkedIn](https://www.linkedin.com/in/suraj-k-3bb9a0190)

---

**Built with ❤️ by Suraj**  
