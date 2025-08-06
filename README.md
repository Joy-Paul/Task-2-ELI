# Task-2-ELI

Task: Analyze a phishing email to identify potential indicators of malicious intent.
Objective: Recognize and document phishing characteristics based on industry best practices.

📧 1. Email Sample Overview
Subject Line: "URGENT: Your Account Has Been Suspended!"
Sender Address: support@paypalsecure.com
Email Body Preview:

Dear Customer,
We noticed unusual activity on your PayPal account. For your security, your account has been temporarily suspended.
Please login now to restore access: Click Here
Failure to respond within 24 hours will result in permanent suspension.

🕵️ 2. Phishing Indicators Found
✅ 1. Suspicious Sender Address (Spoofing)
Claimed to be from PayPal, but the domain @paypalsecure.com is not an official PayPal domain.

Legitimate emails from PayPal would come from @paypal.com.

✅ 2. Email Header Analysis
Return-Path does not match sender domain.

Reply-To address redirects to a completely unrelated domain.

SPF/DKIM validation failed (checked using MXToolbox or similar header analyzer).

✅ 3. Suspicious Link
Hyperlink text shows "Click Here", but when hovered, it points to:
http://paypal-verification123.com/login

The domain is unrelated to PayPal and is clearly fraudulent.

✅ 4. Urgency and Threatening Language
"URGENT", "Account Suspended", "Failure to respond within 24 hours..." are pressure tactics.

Creates fear to push users to act impulsively.

✅ 5. Spelling/Grammar Errors
Sentence structure is awkward:
"Please login now to restore access" → "log in" should be two words.
Minor grammatical inconsistencies throughout the email.

✅ 6. Unusual Attachment or Link
Contains a clickable link instead of directing users to manually visit the official website.

Potential malware or credential harvesting site.

🧠 3. Summary of Phishing Traits
#	Phishing Indicator	Description
1	Fake sender address	Domain spoofing or domain lookalike (paypalsecure.com)
2	Header manipulation	Reply-to/Return-path mismatch, failed SPF
3	Malicious URL	Mismatched anchor and real URL
4	Urgent tone	Fear-based language pushing immediate action
5	Spelling/grammar issues	Minor errors reduce credibility
6	Link to non-official domain	Redirects to phishing site pretending to be PayPal
