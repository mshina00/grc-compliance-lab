# Lab 07: Network Traffic Analysis with Wireshark (Security and Compliance Focus)

**Time:** 3-4 hours | **Tools:** Wireshark | **Frameworks:** ISO 27001 A.8.20, A.8.24; PCI DSS Req. 4; HIPAA 164.312(e); NIST CSF PR.DS, DE.CM

> **Ethics and legality:** Capture only on your own network and devices, or use public sample capture files. Never capture other people's traffic without written authorization.

## Objectives
- Capture and read network traffic.
- Show why encryption in transit matters, and connect findings to compliance controls.
- Recognize suspicious patterns that feed risk assessment and monitoring.

## Setup
1. Install Wireshark from wireshark.org.
2. Choose your Wi-Fi or Ethernet interface and start a capture.
3. Alternatively, download sample `.pcap` files from the official Wireshark sample captures page.

## Part A: Basics (30 min)
1. Capture 2 minutes of normal browsing, then stop.
2. Open **Statistics → Protocol Hierarchy** and note which protocols appear.
3. Open **Statistics → Conversations** and identify the top talkers.

## Part B: DNS and TCP (45 min)
| Goal | Display filter |
|---|---|
| View DNS queries | `dns` |
| TCP connection starts (SYN) | `tcp.flags.syn == 1 && tcp.flags.ack == 0` |
| Retransmissions (possible network trouble) | `tcp.analysis.retransmission` |
| One host only | `ip.addr == <address>` |

Tasks: follow one TCP three-way handshake (SYN, SYN-ACK, ACK) and record the packet numbers. List five domains your device looked up.

## Part C: Encrypted vs Unencrypted Traffic (60 min)
| Goal | Display filter |
|---|---|
| Unencrypted web requests | `http` |
| Form submissions | `http.request.method == "POST"` |
| TLS handshakes | `tls.handshake.type == 1` |

Tasks:
1. Using a **sample capture** (or a test page you control), find HTTP traffic and show that content is readable.
2. Find TLS traffic and show that the payload is not readable.
3. Right-click a packet → **Follow → TCP Stream** and compare both cases.
4. Write the compliance impact: which requirements would unencrypted transmission of sensitive data violate?

## Part D: Spotting Suspicious Patterns (60 min)
Using a public sample capture that contains scanning or ARP activity:
- Many SYN packets from one source to many ports may indicate **port scanning**. Filter: `tcp.flags.syn == 1 && tcp.flags.ack == 0`.
- Repeated `arp` replies for one IP from different MAC addresses may indicate **ARP spoofing**. Filter: `arp`.
- Large outbound transfers to an unfamiliar address may indicate **data exfiltration**. Check **Statistics → Conversations**.

## Part E: Turn Findings into GRC Output (30 min)
Add two risks to your Lab 01 register, for example "If internal services use unencrypted protocols, then credentials could be intercepted, resulting in account compromise." Map each to a control.

## My Findings (fill in with your own results)
| Part | What I did | What I observed | Screenshot filename | Compliance link |
|---|---|---|---|---|
| A | | | | |
| B | | | | |
| C | | | | |
| D | | | | |
| E | | | | |

## Self-check
- Can you explain why HTTPS protects against eavesdropping but not against a malicious website?
- Did you remove or blur any personal information from screenshots before publishing?


---
© 2026 Hina Qurashee. All rights reserved.
