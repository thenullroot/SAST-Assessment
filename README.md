# Vulnerable Flask App – SAST Assessment

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.10%2B-blue.svg)
![Flask](https://img.shields.io/badge/flask-vulnerable-red.svg)
![Semgrep](https://img.shields.io/badge/SAST-Semgrep-orange.svg)
![Stars](https://img.shields.io/github/stars/thenullroot/SAST-Assessment?style=social)
![Forks](https://img.shields.io/github/forks/thenullroot/SAST-Assessment?style=social)
[![LinkedIn](https://img.shields.io/badge/Author-Aniket%20Nayak-blue)](https://www.linkedin.com/in/aniket-nayak-634495317/)

## 📌 Project Overview
This repository contains a deliberately insecure Flask application designed for penetration testing practice.  
The project demonstrates how to perform **Static Application Security Testing (SAST)** using **Semgrep** with multiple rulesets:
- Baseline ruleset
- OWASP Top 10 (2025) ruleset
- Python language‑specific ruleset

The goal is to identify vulnerabilities, map them to **OWASP Top 10 categories**, and provide professional remediation guidance.

---

## 🛠 Tools Used
- **Semgrep** – static analysis engine
- **Python / Flask** – vulnerable application framework
- **OWASP Top 10 (2025)** – vulnerability classification
- **Linux environment** – for running scans and evidence collection

---

## 📂 Repository Structure
- **SAST-Assessment/** (root folder)
  - **evidence/**
    - **final_report/** → Consolidated_SAST_Report_Vulnerable_Flask_App.txt  
    - **screenshots/** → baseline_scan.png, owasp_top_ten_scan.png, python_scan.png  
    - **semgrep/** → baseline_scan.txt, owasp_top_ten_scan.txt, python_scan.txt  
  - **scope.txt** → Defines the scope of the assessment  
  - **Vulnerable-Flask-App/** → Source code of the intentionally vulnerable Flask application  


---

## 📑 Key Deliverable
- **[Consolidated SAST Report](evidence/final_report/Consolidated_SAST_Report_Vulnerable_Flask_App.txt)**  
  A professional, detailed report consolidating findings from all three scans, mapped to OWASP Top 10 categories, with remediation recommendations.

---

## 🚀 How to Reproduce
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/SAST-Assessment.git
   cd SAST-Assessment/Vulnerable-Flask-App

2. Set up a Python virtual environment and install dependencies:

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

3. Run the vulnerable Flask app:

python vulnerable-flask-app-linux.py

4. Execute Semgrep scans:

semgrep --config=auto vulnerable-flask-app-linux.py
semgrep --config=owasp-top-ten vulnerable-flask-app-linux.py
semgrep --config=p/python vulnerable-flask-app-linux.py

👨‍💻 Author
Aniket Nayak – Aspiring Penetration Tester

⚠️ Disclaimer
This project is for educational and training purposes only.
Do not deploy the vulnerable Flask app in production environments.

