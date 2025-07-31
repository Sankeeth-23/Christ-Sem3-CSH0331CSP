# ✅ Check Internet Exposure via Shodan

## 🎯 Objective  
Perform a personal security audit by checking what information is publicly visible about your internet connection — from an attacker’s perspective.

---

## 📋 Scenario  
You're assessing your network's exposure using Shodan to discover what services and data are accessible to the public internet. This helps identify security risks and apply proper defenses.

---

## 🔍 Steps Taken  

1. **Public IP Discovery**  
   - Identified the public IP address using a service like [whatismyipaddress.com](https://whatismyipaddress.com)  
   - *(IP masked for privacy: `XXX.XXX.XXX.XXX`)*

2. **Shodan Lookup** *(Simulated Results)*  
   - Entered the IP into [Shodan.io](https://shodan.io)  
   - Found the following open ports and services:

     | Port | Service      | Notes                                      |
     |------|--------------|--------------------------------------------|
     | 80   | HTTP         | Apache 2.4.29 – exposed web server         |
     | 443  | HTTPS        | Secure web interface active                |
     | 22   | SSH          | OpenSSH 7.6p1 – could allow remote access  |
     | 7547 | TR-069       | ISP modem management – potential risk      |

   - **Exposed Metadata**: ISP name, reverse DNS, geolocation (city-level), and device fingerprinting.

---

## ⚠️ Security Risks Identified  

- **Open SSH Port (22)**: Susceptible to brute-force login attacks.
- **TR-069**: A protocol often misconfigured by ISPs, exploitable by attackers.
- **Web Services**: Public-facing HTTP/HTTPS services may leak headers or run outdated software.
- **Device Information Exposure**: Revealing router model and firmware can aid targeted attacks.

---

## 🔐 Recommendations  

- 🔒 Close all unused ports via your router/firewall settings.  
- 🚫 Disable remote access features (SSH, TR-069) unless absolutely needed.  
- 🔑 Change default passwords on all devices, especially routers and cameras.  
- 🔄 Keep router and firmware/software fully updated.  
- 🌐 Use a VPN to hide your real IP address.  
- 📊 Set up traffic alerts or intrusion detection (if supported).

---

## ✅ Conclusion  

Understanding what your network exposes to the internet is the first step in securing it. Tools like Shodan help reveal what attackers can see — use this knowledge to proactively protect your systems.
