# Phishing Email Analysis Report – xIoTz Job Application

## 1. Sender Analysis
- **Display Name:** xIoTz
- **Actual Email:** Not shown directly in the screenshot, but the suspicious behavior is analyzed in the headers.
- Sender uses a legitimate-looking job-related subject line to appear trustworthy.
- The authenticity of the domain should be checked manually if it doesn't match official job domains (e.g., careers.xiotz.com).

## 2. Header Analysis (via MXToolbox):
❌ DMARC Compliant
❌ SPF Alignment Failed
✅ SPF Authenticated
✅ DKIM Alignment
❌ DKIM Authentication Failed

⚠️ DKIM failed – which may indicate the message was **forged** or altered during transit.

## 3. Language and Tone
- Professional tone, uses the subject “Thanks for submitting your application…” to gain trust.
- This is a **social engineering technique** to avoid suspicion.

## 4. Relay Information
- Email was relayed through: `srv1642.main-hosting.eu` and `relay.mailchannels.net`
- These are not known official email servers of `xIoTz`, raising doubt about authenticity.

## 5. Link and Attachment Check
- Not shown in the header result, but if the original email contained any links or attachments, they should be checked for:
  - Misspelled domains (e.g., `xIoTz-career.net` instead of `xiotz.com`)
  - Suspicious redirect URLs
  - File attachments pretending to be PDFs or job offers

## 6. Conclusion
Although the SPF and DMARC passed, **DKIM failure and unknown relay servers** raise concerns about this email's legitimacy. If the domain and content do not match official xIoTz communication channels, this may be a **phishing attempt targeting job seekers**.

➡️ Always verify job application emails directly from the company website or HR contacts.
