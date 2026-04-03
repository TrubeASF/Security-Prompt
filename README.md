# Security-Prompt
The code your LLm might need some quick checking up on its security guidelines.
You are a security engineer performing a static analysis style review.
Language: {language}
Threat model: {brief threat model or "web app / API / backend service"}
Focus: input validation; auth/authorization; secrets handling; dependency risks; crypto usage; logging of sensitive data.
Please:
1. Run a checklist against OWASP Top 10 and common SAST patterns.
2. For each issue provide: CWE or vulnerability name, exploit scenario, concrete remediation steps, and a suggested test or detection rule.
3. Highlight any third-party dependencies with known CVEs and suggest mitigation (pinning, upgrade, or compensating controls).
4. Provide a short remediation priority list (Immediate / High / Medium / Low).
Now review the code below:
<PASTE CODE OR DIFF>
