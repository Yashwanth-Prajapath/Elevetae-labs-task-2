# Elevetae-labs-task-2
Repo for Task 2 of the internship I'm currently doing at Elevate labs
# Analyzing a Phishing Email Sample

This repository documents a phishing email analysis conducted as part of a cybersecurity training task.

---

##  Objective

To analyze a suspicious email and identify signs of phishing by examining email headers, sender spoofing, links, attachments, and authentication mechanisms.

---

##  Sample Phishing Email

### ⚠ Email Details:
- **From:** `security-update@micros0ft-support.com`
- **To:** `victim@example.com`

###  Observations:
- The sender uses **typosquatting** — `"micros0ft"` instead of `"microsoft"` (uses zero `0` instead of letter `o`).
- The domain name is **not** owned or operated by Microsoft.
- Email appears to be impersonating Microsoft support.
- May include a **malicious link** disguised as a Microsoft login/update page.
- Possibly contains a **dangerous attachment** (`.zip`) that could deploy malware upon opening.

---

##  Email Header Analysis (MXToolbox)

### 🔧 Tool Used:
- [MXToolbox Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)

###  Results Summary:
- **SPF / DKIM:** No records found → sender is **unauthenticated**.
- **Relay Delay:** 0 seconds (insignificant for trust assessment).
- **Spoofed From Address:** `security-update@micros0ft-support.com`
- **Suspicious Domain:** Not a verified Microsoft domain.

---

## 🖼Full Email Body (Visual Reference)

To maintain formatting integrity, the phishing email body is provided below as an image:

- `Microsoft Phishing Email Example.png` — Displays the complete body of the phishing email for visual analysis.

---

## Phishing Indicators Found

| Indicator Type              | Description |
|-----------------------------|-------------|
|  **Typosquatted Domain**     | `micros0ft-support.com` mimics Microsoft |
|  **Spoofed Sender**          | Impersonates Microsoft support |
|  **No SPF/DKIM Auth**        | Cannot verify sender authenticity |
|  **Mismatched Domain**       | Domain name doesn’t belong to Microsoft |
|  **Suspicious Link**         | Likely redirects to phishing or credential harvesting page |
|  **Potential Attachment**    | Possible malware in attached file (e.g., disguised executable) |
|  **Urgent Language (Implied)** | Phishing often uses urgent tone to provoke action |

---

## Conclusion

This email exhibits **classic phishing traits**, including spoofed domains, suspicious sender details, likely malicious links/attachments, and lack of proper authentication (SPF/DKIM). Such emails are designed to steal credentials or install malware and should be reported and deleted immediately.

---

## Author

**Darsh Chatrani**  
🔗 [LinkedIn](https://www.linkedin.com/in/yashwanth-prajapath-90a065303/)  
📞 Contact: +91 73958 52057

---
