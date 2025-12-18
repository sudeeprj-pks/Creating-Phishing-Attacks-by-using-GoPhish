# Phishing Simulation Using GoPhish (Kali Linux)

## 📘 Project Overview

This project demonstrates how to **simulate phishing campaigns using GoPhish** on **Kali Linux** for **security awareness training, red-team labs, and defensive analysis**. The objective is to understand how phishing attacks are created, launched, and analyzed so organizations can **improve detection, user awareness, and email security controls**.

> ⚠️ **Ethical & Legal Notice**
> This project is strictly for **educational purposes** and **authorized environments only** (labs, test domains, or with written permission). Do **NOT** conduct phishing against real users or organizations without consent.

---

## 🎯 Learning Objectives

* Understand phishing attack components (email, landing page, tracking)
* Configure and run GoPhish on Kali Linux
* Launch a controlled phishing simulation
* Analyze results to identify security gaps
* Learn **phishing defense and mitigation strategies**

---

## 🧠 Prerequisites

* Basic understanding of email and web technologies
* Familiarity with the Linux command line (CLI)
* Basic knowledge of social engineering principles

---

## 🛠️ Tools & Technologies

* **Kali Linux** – Penetration testing and security lab OS
* **GoPhish** – Open-source phishing simulation framework
* **Email Account** – For sending test emails (authorized)
* **Web Server** – For hosting landing pages (Apache or equivalent)

---

## 📦 Installation – GoPhish

1️⃣ Download the latest GoPhish release from the official repository:

* [https://github.com/gophish/gophish/releases](https://github.com/gophish/gophish/releases)

2️⃣ Extract the archive:

```bash
tar -xvzf gophish-vX.X.X-linux-64bit.tar.gz
```

3️⃣ Start GoPhish:

```bash
cd gophish
sudo ./gophish
```

4️⃣ Access the admin interface:

* URL: [https://localhost:3333](https://localhost:3333)
* Default credentials:

  * **Username:** admin
  * **Password:** gophish

---

## 🧪 Lab Tasks

### Task 1: Set Up the Phishing Campaign

Steps:

* Open the GoPhish web interface at `https://localhost:3333`
* Create a **User Group** with authorized test email addresses
* Create an **Email Template** for the phishing message
* Configure a **Landing Page** to capture inputs (test data only)
* Create a **Campaign** using the user group, template, and landing page

**Expected Output:**
A fully configured phishing campaign ready for controlled execution.

---

### Task 2: Launch the Phishing Campaign

Create an email template with the following example (lab use only):

* **Subject:** Urgent suspicious activity on your Microsoft account
* **From:** [support@yourcompany.com](mailto:support@yourcompany.com)
* **Body (HTML):**

```html
<html>
  <body>
    <h2>Dear User,</h2>
    <p>We have noticed suspicious activity on your account. Please verify your account information by clicking the link below:</p>
    <p><a href="http://192.168.1.100:8080/verify">Verify Account</a></p>
    <p>If you do not verify your account within 24 hours, your account will be locked.</p>
    <p>Thank you,<br>Your Company Support Team</p>
  </body>
</html>
```

**Expected Output:**
A convincing phishing email template designed for awareness testing.

---

### Task 3: Analyze Phishing Results

* Monitor campaign results in the GoPhish dashboard
* Review metrics such as:

  * Email opened
  * Link clicked
  * Credentials submitted (test data)
* Identify users who interacted with the phishing content

**Expected Output:**
A detailed report highlighting user behavior and security weaknesses.

---

## 📊 Reporting & Analysis

Key metrics to include in your report:

* Email delivery success rate
* Click-through rate (CTR)
* Credential submission rate
* Time to first click

Use findings to recommend:

* User awareness training
* Email filtering improvements
* MFA enforcement
* URL filtering and sandboxing

---

## 🛡️ Phishing Defense Guide (Recommendations)

* Conduct regular security awareness training
* Enable **Multi-Factor Authentication (MFA)**
* Implement email security gateways
* Use SPF, DKIM, and DMARC
* Train users to identify suspicious emails and URLs
* Monitor and block malicious domains

---

## ⚠️ Disclaimer

This project must only be executed in **controlled lab environments** or with **explicit authorization**. Any misuse of phishing tools is unethical and may be illegal.

---

## 📄 License

This project documentation is provided for **educational and training purposes** only.

---

**Project Title:** Phishing Simulation Using GoPhish
**Domain:** Cybersecurity • Social Engineering Awareness
**Platform:** Kali Linux
**Author:** Sudeep
