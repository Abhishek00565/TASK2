#  Cyber Security Internship – Task 2: Phishing Email Analysis

##  Objective

Analyze a phishing email sample to identify suspicious indicators like spoofed email addresses, misleading links, social engineering tactics, and email header manipulation.

---

##  Tools Used

- Plain text email sample (`phishing_email_sample.txt`)
- [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- Screenshot evidence of email and header analysis

---

##  Step-by-Step Analysis

 1. Phishing Email Sample

A spoofed email pretending to be from **PayPal Security** was used as the phishing sample.  
The email falsely claimed the recipient's account had been limited due to suspicious activity.

 File: `phishing_email_sample.txt`  
 Screenshot: `screenshots/phishing_mail.png`

---

###  2. Phishing Indicators Identified

| Indicator | Description |
|----------|-------------|
|  **Spoofed sender email** | `service.epayipal@outlook.com` mimics a PayPal domain |
|  **Fake links** | “Log in” and “Resolution Center” likely redirect to a phishing site |
|  **Urgent tone** | “Your account is still temporarily limited…” creates pressure |
|  **Generic greeting** | No personal name, just “Dear Customer” |
|  **Social engineering** | Uses fear and authority to provoke response |

---

###  3. Email Header Analysis

A simulated header was analyzed using MXToolbox.  
Screenshot: `screenshots/header_analysis.png`

#### Key Findings:
- Header shows the message came from **203.0.113.123**, an unknown source.
- The domain used is **mail-fake.paypal.com**, which is not a legitimate PayPal server.
- The **From**, **Reply-To**, and **Return-Path** addresses all match a spoofed Outlook address:  
  `service.epayipal@outlook.com`

---

##  Interview Questions & Answers

**1. What is phishing?**  
A type of cyberattack where attackers impersonate trusted entities to steal sensitive information like passwords or credit card numbers.

**2. How to identify a phishing email?**  
Check for suspicious sender emails, grammar errors, fake links, urgent or threatening language, and unexpected attachments.

**3. What is email spoofing?**  
Email spoofing is when an attacker forges the sender's address to make it look like it came from someone trusted (e.g., PayPal).

**4. Why are phishing emails dangerous?**  
They can trick users into revealing confidential info or downloading malware, leading to identity theft or system compromise.

**5. How can you verify the sender’s authenticity?**  
Check domain spelling, email headers, SPF/DKIM verification, and contact the organization through official channels.

**6. What tools can analyze email headers?**  
- [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)  
- [Google Admin Toolbox](https://toolbox.googleapps.com/apps/messageheader/)

**7. What actions should be taken on suspected phishing emails?**  
- Do not click links or download attachments  
- Report to IT/security team  
- Block sender  
- Delete the email

**8. How do attackers use social engineering in phishing?**  
They manipulate emotions like fear or urgency to get the victim to act without thinking — for example, threatening account suspension.

---



