# Cloud Attack Surface Scanner

A lightweight cloud security tool designed to simulate **attack surface reconnaissance in AWS environments** from a Red Team perspective.

---

## 🧠 Overview

This project demonstrates how an attacker or security engineer can map exposed cloud resources and identify potential misconfigurations in AWS infrastructure.

The focus is not exploitation, but **security validation and risk visibility**.

---

## 🎯 Objectives

- Simulate cloud attack surface discovery
- Identify exposed cloud resources (S3, Security Groups)
- Generate structured security reports
- Support security validation and risk assessment workflows

---

## ⚙️ Architecture

The tool is structured in a modular format:

- `core/` → execution logic and orchestration
- `aws/` → AWS service interaction modules
- `outputs/` → generated reports (JSON format)

---

## ☁️ What It Checks

### S3 Buckets
- Lists buckets (simulated or real AWS integration-ready)
- Designed for future detection of public exposure

### Security Groups
- Designed to identify open network exposure (0.0.0.0/0 scenarios)
- Baseline for network attack surface analysis

---

## 📊 Output Example

```json
{
  "s3": {
    "buckets": []
  },
  "security_groups": {
    "rules": []
  }
}
🚀 How to Run
python3 core/scanner.py
🎯 Security Perspective

This tool simulates the initial phase of a Red Team engagement, focusing on:

Attack surface mapping
Cloud misconfiguration discovery
Exposure validation

It aligns with modern cloud security practices such as:

MITRE ATT&CK (Reconnaissance phase)
Cloud Security Posture Management (CSPM)
Threat modeling in cloud environments
⚠️ Disclaimer

This tool is intended for educational and defensive security purposes only.
It should only be used in environments where you have authorization.

👤 Author

Marcos Caron
Cloud Security & Offensive Security Practitioner

