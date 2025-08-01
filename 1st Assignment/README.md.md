# 🔎 Check Internet Exposure via Shodan

## 🎯 Objective  
Conduct a personal network security audit to determine what information is publicly visible about your internet connection using Shodan.

## 📋 Scenario  
You're simulating an attacker's view of your home network by analyzing exposed services and potential vulnerabilities. This helps identify weak points and guides system hardening.

## 🔧 Steps Followed  
1. **Found Public IP** using [whatismyipaddress.com](https://whatismyipaddress.com) — *masked as* `XXX.XXX.XXX.XXX`  
2. **Searched on Shodan** at [shodan.io](https://shodan.io)  
3. **Observed Exposed Services**:

| Port | Service | Description                            |
|------|---------|----------------------------------------|
| 80   | HTTP    | Apache 2.4.29 web server                |
| 443  | HTTPS   | Secure web interface                   |
| 22   | SSH     | OpenSSH 7.6p1 – potential brute force  |
| 7547 | TR-069  | ISP router mgmt – remotely accessible  |

## ⚠️ Security Risks  
- **Open SSH Port (22):** Vulnerable to brute-force login attempts.  
- **TR-069:** Common target in ISP routers with outdated firmware.  
- **Device Details:** Attackers can fingerprint router models and software versions.  
- **Outdated Web Services:** Exposed HTTP servers may reveal sensitive info.

## 🔐 Recommendations  
- 🔒 Close unused ports via firewall/router settings.  
- 🚫 Disable remote access protocols unless required.  
- 🔑 Change all default device/router credentials.  
- 🔄 Update firmware regularly.  
- 🌐 Use a VPN to hide your public IP.  
- 📈 Enable logging or alerts for suspicious activity.

## ✅ Conclusion  
Shodan helps visualize what attackers see. Regular audits, proper configuration, and minimizing public exposure can dramatically improve home network security.
