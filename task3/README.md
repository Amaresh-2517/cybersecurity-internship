# Task 3 – Basic Vulnerability Scan on Your PC Using Nessus Essentials

## Objective
Use Nessus Essentials, a free vulnerability scanner, to identify and assess common security vulnerabilities on your computer.

## Tools Used
- Nessus Essentials

## Steps Performed
1. Installed Nessus Essentials on the computer.
2. Configured the scan target as the local machine IP (127.0.0.1).
3. Conducted a full vulnerability scan which took approximately 30-60 minutes.
4. Reviewed the scan report focusing on High and Medium severity vulnerabilities.
5. Analyzed each vulnerability's details including description, risk factor, and potential impact.
6. Documented remediation steps for each identified vulnerability.
7. Took screenshots and compiled a detailed report of findings.

## Summary of Findings
- Several medium and high severity vulnerabilities were discovered.
- Medium severity issues include untrusted SSL certificates and outdated software components (e.g., Ruby WEBrick HTTP request smuggling).
- High severity vulnerabilities include DoS vulnerabilities in Ruby REXML library and use-after-free issues in c-ares library on macOS.
- Each vulnerability includes a risk synopsis and recommended remediation actions such as software upgrades or configuration changes.

## Deliverables
- Detailed vulnerability scan report (this document).
- Documentation of critical vulnerabilities and suggested fixes.
- Screenshots of scanned results.

## Outcome
This task provided practical exposure to vulnerability scanning and enhanced understanding of security risks in software and system configurations commonly found on personal computers.

## Interview Questions to Prepare
- What is vulnerability scanning and how does it differ from penetration testing?
- What are some common vulnerabilities discovered in this scan?
- How does Nessus identify vulnerabilities?
- What are the impacts of untrusted SSL certificates?
- Explain the significance of CVSS (Common Vulnerability Scoring System).
- Why is it important to update software and libraries frequently?
- How do you prioritize remediation of vulnerabilities?
- What are false positives in vulnerability scanning?

## Submission
Upload your entire task3 folder including this README.md and your detailed Nessus report to your GitHub repository.

