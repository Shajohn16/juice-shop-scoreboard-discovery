# OWASP Juice Shop - Score Board Discovery

## Challenge
You successfully solved the challenge: **Score Board** — Find the carefully hidden 'Score Board' page.

## Summary
This project explains how I discovered the hidden scoreboard URL and accessed it using multiple techniques including BurpSuite and browser path guessing.

## Exploitation Flow
1. Access the Juice Shop app on localhost (Docker).
2. Brute-force common paths or use `robots.txt`, `sitemap.xml`, or page source.
3. Discovered `/score-board` path.
4. Accessed it to unlock the challenge.

## Tools Used
- BurpSuite
- OWASP Juice Shop (Docker)
- Browser DevTools

## Flags Solved
✅ Score Board route discovered

## Notes
No dependencies on this host system. This write-up is fully portable.

for clarity -----------------

# Juice Shop Challenge: Score Board Discovery

## 🧠 Challenge Description
This project solves the OWASP Juice Shop challenge: **Score Board**  
> "Find the carefully hidden 'Score Board' page."

## 💡 Objective
By analyzing the app structure and hidden endpoints, we discovered the `/score-board` page using Burp Suite and browser inspection.

## 🛠️ Tools Used
- Burp Suite
- Browser DevTools
- OWASP Juice Shop (Docker)
- Linux Terminal (Kali)

## 🔓 Solution Strategy
1. Launched Juice Shop on Docker locally.
2. Explored site and used Burp Suite to look for hidden endpoints.
3. Found `/score-board` and navigated manually to it.
4. Successfully solved the challenge.

## 🚩 Result
Challenge was marked as solved. 🟢

## 📁 Structure
- `README.md`: This file
- `screenshot.png`: Proof of solution (optional)

## 🗃️ Tags
`OWASP Juice Shop` `BurpSuite` `Bug Bounty` `Pentesting` `Scoreboard`

---------------- BETTER AND DETIALED REAMDE FOR CLARITY ----------------

# 🍊 OWASP Juice Shop - Scoreboard Discovery (Challenge Walkthrough)

## 🔍 Challenge: Scoreboard Discovery
**Category**: Information Disclosure  
**Objective**: Find and access the hidden Score Board page of OWASP Juice Shop.

---

## 🧠 What I Learned
As an Offensive Security Researcher, this challenge reinforced critical techniques in:
- **Client-side enumeration** for hidden endpoints
- **JavaScript reverse engineering**
- **Application structure mapping**
- Avoiding red herrings through logic-based validation of paths

---

## 🛠️ Tools & Techniques Used
- **Burp Suite (Community Edition)**: Intercept traffic, map app structure, and test hidden routes.
- **Browser DevTools (Firefox)**: Locate obfuscated JavaScript files.
- **JS Beautifier & Source Analysis**: Read through minified files to extract clues.
- **Directory Brute-forcing** (if applicable): For endpoint discovery using tools like `ffuf` or `dirsearch`.

---

## 🧪 Methodology (Step-by-Step)
1. **Load the App** → Visited `http://localhost:3000` in browser.
2. **Check for robots.txt** → No public disallowed paths.
3. **Inspected JavaScript** → Located hints to `/score-board` in obfuscated files.
4. **Used Burp** → Verified existence of `/score-board` path via Repeater.
5. **Accessed Scoreboard** → Challenge solved.

---

## 📸 Screenshots
*(Replace with actual screenshots or link to webhook logs/console output if needed)*

---

## 🧵 What is Score Board Discovery?
The Score Board is a **secret page** within the Juice Shop application that lists all possible challenges and their completion status. It's intentionally hidden to simulate real-world **security by obscurity** flaws.

> Accessing this page demonstrates the importance of properly securing internal endpoints, as attackers can reveal sensitive app mechanics if exposed.

---

## ⚙️ Relevance in Real-World Pentesting
- **OSINT & Recon Phase**: Finding unlinked paths in the frontend source is a common and essential skill.
- **Bypassing Security Through Obscurity**: Scoreboards, dashboards, and admin panels often lack proper authentication in poorly designed systems.
- **Obfuscated JS Analysis**: Key in CTFs and red-team engagements for buried endpoints.

---

## ✅ Challenge Completed

# juice-shop-scoreboard-discovery
