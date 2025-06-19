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

