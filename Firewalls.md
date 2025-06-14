# Firewall Report

## 1. Introduction
- A **firewall** is a security device or software that controls traffic between networks.
- It acts as a barrier between a trusted internal network and untrusted external networks.

## 2. Purpose of Firewalls
- Prevent unauthorized access.
- Block malicious traffic.
- Monitor and log network activity.
- Enforce organizational security policies.

## 3. Types of Firewalls

### a. Packet-Filtering Firewall
- Inspects headers of packets (IP, port, protocol).
- Fast and simple.
- Works at the **network layer**.
- Limited in deep traffic inspection.

### b. Stateful Inspection Firewall
- Tracks the state of active connections.
- Allows packets that match known sessions.
- More secure than packet-filtering firewalls.

### c. Proxy Firewall
- Intermediary between client and server.
- Operates at the **application layer**.
- Inspects content of packets.
- Adds latency but provides better filtering.

### d. Next-Generation Firewall (NGFW)
- Combines traditional firewall features with:
  - Deep Packet Inspection (DPI)
  - Intrusion Prevention Systems (IPS)
  - Application-level awareness
- Can detect modern threats like malware and exploits.

### e. Software vs. Hardware Firewalls
- **Software Firewall**: Runs on individual devices (e.g., Windows Firewall).
- **Hardware Firewall**: Dedicated appliance for network protection (e.g., Cisco ASA).

## 4. Firewall Rules
- Define allow/deny conditions based on:
  - IP addresses
  - Ports
  - Protocols
  - Applications
- Evaluated in sequence (top-down order).

## 5. How Firewalls Work
- Intercept data packets entering/leaving a network.
- Apply filtering rules.
- Log and monitor decisions.
- Can be placed at network perimeter or between segments.

## 6. Firewall Architectures

### a. Bastion Host
- Hardened device placed outside the internal firewall.
- Exposes limited services to the public (e.g., web server).

### b. DMZ (Demilitarized Zone)
- Buffer zone between internal network and the internet.
- Hosts public-facing services (e.g., mail, DNS).

### c. Dual-Homed Host
- Two network interfaces for separating internal and external traffic.
- Can be used for traffic inspection and control.

## 7. Limitations of Firewalls
- Cannot protect against:
  - Insider threats
  - Phishing attacks
  - Social engineering
- May be bypassed by encrypted traffic (e.g., VPNs, HTTPS).
- Require regular updates and monitoring.

## 8. Use Cases
- **Enterprise Networks**: Control and secure internal and external access.
- **Home Networks**: Protect devices from internet-based threats.
- **Cloud Environments**: Use virtual firewalls to protect cloud resources.

## 9. Popular Firewall Solutions

### Software:
- Windows Defender Firewall
- iptables (Linux)
- pfSense

### Hardware:
- Cisco ASA
- Palo Alto Networks
- Fortinet FortiGate
- Sophos XG

## 10. Conclusion
- Firewalls are critical for maintaining network security.
- They should be part of a multi-layered defense strategy.
- Regular updates, monitoring, and integration with other security tools enhance their effectiveness.


## 11. References
Stallings, W. (2017). Network Security Essentials: Applications and Standards (6th ed.). Pearson.
Comprehensive resource on firewalls, network architectures, and security principles.

National Institute of Standards and Technology (NIST). (2009). Guide to Firewalls and Firewall Policy (SP 800-41 Rev. 1).
https://csrc.nist.gov/publications/detail/sp/800-41/rev-1/final

Fortinet. (n.d.). Firewall Security Explained
Definitions, use cases, and architecture examples from a popular firewall vendor.

Sophos. (n.d.). Sophos XG Firewall Overview
Details on Sophos’ NGFW features and network deployment options.
