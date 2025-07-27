# Day 4: Networks
## What is a network?
- It is a collection of devices which are connected to each other and share data to each other.They can be linked by wired or wireless connections.

##  Subnet
- Subnet masks are used to identify which part of the IP address refers to the network and which part refers to the host.
- Helps reduce network congestion by limiting broadcast domains.
- A subnet is a smaller part of network it exits so that we can divide a large network into manageable parts. 
- This is done to control traffic and improve performance.
- To even enhance security by isolating segments

## IP(Internet Protocol)
- Public vs. Private IP addresses: Public IPs are accessible over the internet; private IPs are used within local networks.
- IP addresses can be static or dynamic depending on how they’re assigned.
-It is a unique number label assigned to each device connected to the internet that uses ip for communication.
- It helps us to identify the device location in the network.
- It makes sure the data is sent to the right person.
- There are 2 types:-
  * IPv4
  * IPv6
## MAC ID
- It is also called MAC address which means Media Access Control Address
- It is the address of the hardware device. it is built into the device.
- It never changes.
- It is 6 pairs of hexadecimal numbers,seperated by **:** or **-**.

## IPv4 VS IPv6
- IPv4 and IPv6 are 2 versons of the IP which assigns address to devices so that they can communicate
  |     | IPv4 | IPv6 |
  |-----|------|------|
  | Created on | Older verson Created in 1980 | Newer verson  created in 1998 was created cause IPv4 ranout |
  | Size | 32bits | 128 bits |
  | Total address | Nearly 4.3 Billion(4.3 x 10<sup>9</sup>) | Nearly 340 undecillion(3.4x 10<sup>38</sup>) |
  | Format |	Numbers (0–255, four parts)| Hexadecimal, eight groups |
  | Speed| Slower| Faster|
  | Security| Optional | Built in |
  ## Staic and Dynamic IP address
  - Static IP address:
    * **Fixed:** Does not change once given.
    *  **Used for:** Servers,CCTV systems ,etc.
    *  Set manually by the user or admin.
  - Dynamic IP address:
    * Changes automatically Each time the device connects to a network,
    * Assigned by DHCP (Dynamic Host Configuration Protocol)
## TCP and UDP:
- TCP is used where reliability and order matter; UDP is used where speed is more critical than reliability.
- Common TCP ports: 80 (HTTP), 443 (HTTPS), 25 (SMTP). Common UDP ports: 53 (DNS), 67/68 (DHCP), 123 (NTP).
- **TCP (Transmission Control Protocol):**
  * Makes a reliable connection before sending data (handshake).
  * Ensures all packets arrive in the correct order with error checking.
- **UDP (User Datagram Protocol):**
  * Sends data without making a connection first.
  * no guarantee the data will arrive or arrive in order
  
  |  | TCP | UDP |
  |---------|-----|-----|
  | Connection | Connection-oriented (handshake) | Connectionless |
  | Reliability | Reliable, ensures delivery | Not reliable |
  | Speed | Slower | Faster |
  | Use cases | Web browsing, email, file transfer | Streaming, gaming, VoIP |
  | Complexity|Complex|Simple|

  ## UAC(User Access Control)
  - It is a windows security feature that helps prevent unauthorized changes to the computer.

## Reconnaissance:
- The process of gathering information about a target before the attack.
- There are two types:
  * **Active Reconnaissance:** Directly interacts with target system by sending packets scans portsbut is easier to detect
  * **Passive Reconnaissance:** No direct interaction with the target by collecting publicly available data the process is slower but it is harder to detect
  * We did passive reconnaissance using wayback machine

## Nmap
- Supports a scripting engine (NSE) for automated vulnerability detection.
- Useful in network inventory, service upgrade schedules, and monitoring host uptime.
- Used to scana nd gather information about networks,hosts and services
- What it does is it
  * finds live hosts on a network
  * Identifies open ports.
  * Detects services and versions running on those ports.
  * Can even guess the operating system.
  * Useful for security testing and reconnaissance.

| Flag         | Meaning                   | Purpose / When to Use                    |
| ------------ | ------------------------- | ---------------------------------------- |
| **-Pn**      | Skip host discovery       | Scan even if ping is blocked             |
| **-A**       | Aggressive scan           | Detect OS, versions, traceroute, scripts |
| **-sV**      | Service/version detection | Find software and version on ports       |
| **-O**       | OS detection              | Guess the target’s operating system      |
| **-oM**      | Machine-readable output   | Save results for automation              |
| **--script** | Run Nmap scripts (NSE)    | Check for vulnerabilities, extra info    |
| **-v / -vb** | Verbose / very verbose    | Show more details in scan output         |
| **-p**       | Specify port(s)           | Scan only chosen ports                   |
| **-sS**      | SYN (stealth) scan        | Faster, less detectable port scan        |
| **-sT**      | TCP connect scan          | Full handshake, reliable but noisy       |








  
