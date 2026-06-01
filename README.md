# Task-2: Phishing Email Analysis

## Objective
To analyze a sample phishing email by examining its header, identifying red flags, and documenting the findings.

## Files in this Repository
1. `sample_email.txt` - Contains full email header, body, and detailed analysis of why it's phishing
2. `Screenshot 2026-06-01 214152.png` - Header analysis showing SPF fail
3. `Screenshot 2026-06-01 214516.png` - Header analysis showing DKIM fail  
4. `Screenshot 2026-06-01 214812.png` - Summary of authentication results

## Key Findings
1. **Domain Spoofing**: Sender uses `security-update-paypal.com` instead of `paypal.com`
2. **SPF Failed**: Sending server IP not authorized for the domain
3. **DKIM Failed**: Email signature is invalid
4. **Social Engineering**: Uses urgency "24 hours" + threat "account suspended"
5. **Suspicious Link**: URL redirects to `verify-account.com`, not PayPal

**Conclusion**: The email is a phishing attempt and should be deleted.
