---
layout: default
title: "🛡️ Endpoint Threat Detection & Response with Splunk + Windows Defender"
---

# 🛡️ Endpoint Threat Detection & Response with Splunk + Windows Defender

## 🧠 Project Overview

This project demonstrates how Splunk + Windows Defender can be used to build an **EDR (Endpoint Detection & Response)** monitoring solution in a home lab environment.

We built:

- A real-time Splunk dashboard
- Mapped MITRE ATT&CK threat detections (PowerShell, Brute-force, Registry tampering)
- Custom alerts with hourly scheduling
- Documentation of the detection & response lifecycle

---

## 🧩 MITRE Mapping

- **T1059.001** – PowerShell Execution
- **T1110.001** – Brute-force Logins
- **T1112** – Registry Modification

---

## ⚡ PowerShell Abuse Detection (T1059.001)

### 🔍 Raw Logs:
![PowerShell Logs](images/Powershell%20log%20results.png)

### 📊 Dashboard Panel:
![PowerShell Dashboard](images/Powershell%20Dashboard%20Panel.png)

---

## 🚨 Brute-force Detection (T1110.001)

### 🔍 Failed Logins:
![Failed Logins](images/failed-login-screen.png)

### 📊 Dashboard Panel:
![Brute-force Panel](images/brute-force-dashboard-panel.png)

### ⚙️ Alert Setup:
![Brute-force Alert Config](images/Brute%20force%20alert%20config.png)

---

## 🛠️ Registry Modification Detection (T1112)

### 🔍 Registry Log Output:
![Registry Mod](images/Registry%20modification%20query%20results.png)

---

## 📊 Final EDR Dashboard

Real-time dashboard with all threat detections mapped to MITRE techniques:

![EDR Dashboard](images/Final_EDR_Dashboard_Screenshot.png)

---

## 🧠 Key Learnings

- Set up a Universal Forwarder to ingest Windows logs into Splunk
- Built detection logic using `EventCode` and `sourcetype` filtering
- Scheduled alerts for brute-force behavior
- Mapped detection panels to real-world adversarial techniques (MITRE)
- Documented end-to-end defensive lifecycle from logging to alerting

---

## 🔗 Connect With Me

Let’s connect and collaborate on more real-world security engineering projects:

[📎 My LinkedIn](https://www.linkedin.com/in/suraj-k-3bb9a0190)

---
