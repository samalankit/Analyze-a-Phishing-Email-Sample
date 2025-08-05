# 📧 Email Safety Comparison Report

## 1. Purpose

This report compares a **safe (legitimate)** email and an **unsafe (phishing)** email based on **content cues** and **email header analysis results** using MXToolbox.

---

## 2. Summary Table

| Criteria                         | Safe Email                                   | Unsafe Email                                          |
|----------------------------------|----------------------------------------------|-------------------------------------------------------|
| Subject                          | Employee Referral for a position at Firstsource Solutions | 🧠 Some handy resources to get started! |
| DMARC Compliant                  | ✅ Yes                                      | ❌ No                                                 |
| SPF Alignment                    | ✅ Passed                                   | ❌ Failed                                             |
| SPF Authenticated                | ✅ Passed                                   | ✅ Passed                                             |
| DKIM Alignment                   | ✅ Passed                                   | ✅ Passed                                             |
| DKIM Authenticated               | ✅ Passed                                   | ❌ Failed                                             |
| Relay Delay                      | 1 second                                    | 0 seconds                                              |
| Tone and Language                | Professional, Formal                        | Generic, Urgent, “Free” Offer                          |
| Links Present                    | No suspicious links                         | ✅ Contains suspicious link                           |
| Branding                         | Consistent with company (Firstsource)       | ❌ No clear branding                                  |

---

## 3. Legitimate Email Analysis

### 🟢 Safe Email

- **Subject:** Employee Referral for a position at Firstsource Solutions
- **Source Domain:** firstsource.com
- **Header Analysis (via MXToolbox):**
  - ✅ DMARC Compliant
  - ✅ SPF Alignment & Authentication
  - ✅ DKIM Alignment & Authentication

<img width="1919" height="975" alt="image" src="https://github.com/user-attachments/assets/faf1170c-827e-4081-887a-248c8429aa40" />

**Conclusion:**  
This email passed all necessary validation checks, and came from a verifiable corporate domain. The header analysis confirms that it is **authentic**.

---

## 4. Phishing Email Analysis

### 🔴 Unsafe Email

- **Subject:** 🧠 Some handy resources to get started!
- **Source Domain:** Suspect or unknown
- **Header Analysis (via MXToolbox):**
  - ❌ DMARC Compliant
  - ❌ SPF Alignment Failed
  - ✅ SPF Authenticated
  - ✅ DKIM Alignment
  - ❌ DKIM Authentication Failed

<img width="1919" height="968" alt="image" src="https://github.com/user-attachments/assets/d64e8912-250f-47c2-8c70-a918f9a9ce7a" />

**Conclusion:**  
This email failed multiple authentication protocols such as **DMARC** and **DKIM**, indicating a **high probability of spoofing**. Combined with suspicious content and urgency-based manipulation, it is flagged as **phishing**.

---

## 5. Key Takeaways

- **SPF**, **DKIM**, and **DMARC** validation are crucial in identifying email authenticity.
- Even if SPF or DKIM is partially passed, failure in DMARC often indicates spoofing.
- Always verify:
  - Sender's domain
  - Tone of the message
  - Presence of unusual links
  - Email header using tools like [MXToolbox](https://mxtoolbox.com/EmailHeaders.aspx)

---

## 6. Tools Used

- [MXToolbox - Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- Screenshots of header analysis from both emails
