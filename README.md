# Network Traffic Analysis — Wireshark & Suricata

**SOC Analyst L1 Lab · Network Detection · Packet Investigation**

> 🟢 **Status: Active — evidence library is being expanded**

### 🧰 Stack
<img src="https://img.shields.io/badge/Wireshark-1679A7?logo=wireshark&logoColor=white" alt="Wireshark"> <img src="https://img.shields.io/badge/Suricata-EF4B4B?logo=suricata&logoColor=white" alt="Suricata"> <img src="https://img.shields.io/badge/PCAP-Analysis-555555" alt="PCAP Analysis">

## 🎯 Why I built this lab
To practise the connection between **raw packets and IDS alerts** — understand the traffic first, then use Suricata telemetry to validate and investigate the security signal.

## 🔎 Investigation workflow

1. Acquire or generate traffic in an authorised lab environment.
2. Use Wireshark filters to isolate hosts, protocols, ports and conversations.
3. Follow TCP/HTTP streams and inspect DNS activity.
4. Run traffic through Suricata and review generated alerts.
5. Correlate IDS alerts with the underlying packets.
6. Document malicious, suspicious or benign conclusions with evidence.

## 🧪 Analysis areas

- Port scanning and reconnaissance
- Suspicious network connections
- DNS anomalies
- HTTP activity
- Beaconing indicators
- IDS alert validation

## 🧠 What I'm practising
**Wireshark • PCAP analysis • Suricata • packet-level investigation • IDS correlation • network anomaly analysis**

## 📌 Evidence roadmap

The repository is being expanded with sanitised PCAP screenshots, Suricata alert examples and analyst-style case notes. No sensitive network data will be published.

## Scope & ethics
Traffic analysis is limited to authorised lab environments and public/educational datasets.
