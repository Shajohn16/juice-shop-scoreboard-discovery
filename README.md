<<<<<<< HEAD
# juice-shop-scoreboard-discovery
# Juice Shop Scoreboard Discovery (OWASP Juice Shop)

## 🎯 Challenge
> Find the carefully hidden 'Score Board' page.

## 🧠 Description
This project documents the complete exploitation of the **Score Board discovery** challenge in OWASP Juice Shop. The goal was to locate the hidden route `/#/score-board` and demonstrate it using BurpSuite and manual testing.

## 🔧 Tools Used
- Docker
- Burp Suite (Community)
- OWASP Juice Shop (local instance)
- Kali Linux

## 📁 Project Structure
- `setup/`: Container setup and environment details
- `burp/`: BurpSuite config files and request analysis
- `screenshots/`: Visual proof of challenge completion
- `writeup/`: Step-by-step attack documentation

## 🐳 Docker Setup
```bash
docker run --rm -d -p 3000:3000 bkimminich/juice-shop


🛡️ Exploit Summary
Visit hidden route: http://localhost:3000/#/score-board

Observe 200 OK response

Log completion on screen

yaml
Copy code

---

### 2. `setup/docker-start-command.txt`
docker run --rm -d -p 3000:3000 bkimminich/juice-shop

yaml
Copy code

---

### 3. `setup/environment-notes.md`
```markdown
# Environment Notes

- **OS**: Kali Linux (VM on Oracle VirtualBox)
- **Network**: Host-only + NAT Adapter
- **Docker**: Preinstalled
- **Port**: Juice Shop exposed on localhost:3000
4. burp/repeater-request.txt
http
Copy code
GET /#/score-board HTTP/1.1
Host: localhost:3000
User-Agent: Mozilla/5.0
Accept: text/html
Connection: close
5. writeup/scoreboard-discovery-walkthrough.md
markdown
Copy code
# Walkthrough: Scoreboard Discovery Challenge

## Step 1: Start Juice Shop
```bash
docker run --rm -d -p 3000:3000 bkimminich/juice-shop
=======
# juice shop scoreboard discovery
>>>>>>> d4fff1d69989e41b73f92fc46800f3d023feee52
