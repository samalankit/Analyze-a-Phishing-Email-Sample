Phishing Email Analysis (xIoTz Job Application)

This repo contains an analysis of a suspicious email allegedly from xIoTz thanking the recipient for applying to a job.

## Included Files

- `phishing_sample.txt`: Simulated email content
- `phishing_report.md`: Full analysis with phishing traits
- `header_analysis_result.txt`: Header breakdown via MxToolbox
- `email_comparison.md` : A comparison between a safe and a phishing email based on header analysis and content cues.
- `README.md`: Summary of task and learning

## Summary

Although the message looks professional and is SPF/DMARC compliant, it **fails DKIM checks** and uses unknown mail servers. The mismatch raises red flags that this may be a phishing attempt, especially if it contains links or downloads.
