# Network Traffic Analysis — Wireshark & Suricata

**SOC Analyst L1 Lab · Network Detection · Packet Investigation**

> 🟢 **Status: Active — evidence library is being expanded**

### 🧰 Stack
<img src="https://img.shields.io/badge/Wireshark-1679A7?logo=wireshark&logoColor=white" alt="Wireshark"> <img src="https://img.shields.io/badge/Suricata-EF4B4B?logo=suricata&logoColor=white" alt="Suricata"> <img src="https://img.shields.io/badge/PCAP-Analysis-555555" alt="PCAP Analysis">

## 🎯 Objective
Practise the connection between **raw packets and IDS alerts**: understand the traffic first, then use Suricata telemetry to validate and investigate the security signal.

## 🗺️ Repository map

| Path | Purpose |
|---|---|
| [`docs/01-analysis-standard.md`](docs/01-analysis-standard.md) | Repeatable packet/IDS investigation workflow |
| [`cases/`](cases/) | Individual investigations and reusable case template |
| [`evidence/`](evidence/) | Evidence quality and sanitisation rules |

## 🔎 Investigation workflow

1. **Scope** the authorised traffic and investigation question.
2. **Filter** hosts, protocols, ports and conversations in Wireshark.
3. **Inspect** TCP/HTTP streams and DNS activity.
4. **Review** Suricata alerts and metadata.
5. **Correlate** IDS signals with packet-level evidence.
6. **Assess** benign, suspicious or malicious behaviour.
7. **Document** the conclusion and recommended action.

## 🧪 Analysis areas

- Port scanning and reconnaissance
- Suspicious network connections
- DNS anomalies
- HTTP activity
- Beaconing indicators
- IDS alert validation

## 🧠 Skills being practised
**Wireshark • PCAP analysis • Suricata • packet investigation • IDS correlation • network anomaly analysis**

## Scope & ethics
Traffic analysis is limited to authorised lab environments and public/educational datasets. Sensitive network data and live malicious payloads are not published.
