# Task 3 — Vulnerability Scan on Localhost

## 🎯 Objective
Perform a vulnerability scan on the local system using Nessus Essentials, identify critical issues, and document recommended fixes.

---

## 🛠 Environment
- **Tool Used:** Nessus Essentials (macOS)
- **Target:** `127.0.0.1` (localhost)
- **Scan Type:** Basic Network Scan

---

## 📊 Scan Results Summary
The scan identified **4 distinct vulnerabilities** of Medium and High severity.

| # | Vulnerability | Severity | Plugin ID | Port/Service | Risk / Impact |
|---|---------------|----------|-----------|--------------|---------------|
| 1 | c-ares `< 1.34.5` Use After Free | **High** | 234803 | 0/general | Memory corruption that could allow a crash or possible remote exploitation. |
| 2 | Ruby REXML `< 3.3.6` DoS | **High** | 242630 | 0/general | XML parsing flaw may allow DoS when handling malicious XML. |
| 3 | Ruby WEBrick `< 1.8.2` HTTP Request Smuggling | Medium | 240854 | 0/general | Inconsistent parsing may allow attackers to smuggle HTTP requests. |
| 4 | SSL Certificate Cannot Be Trusted | Medium | 51192 | 8834/www | The web interface certificate is self-signed, not trusted by browsers or clients. |

---

## 🔎 Vulnerability Details & Fixes

### 1. c-ares `< 1.34.5` — Use After Free
- **Severity:** High  
- **Description:** A flaw in `read_answers()` may lead to use-after-free, exploitable under specific network conditions.  
- **Fix:**  
  ```bash
  brew update && brew upgrade c-ares
  softwareupdate --install --all   # Ensure macOS patches are applied