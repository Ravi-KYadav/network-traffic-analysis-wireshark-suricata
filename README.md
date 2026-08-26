# Network Traffic Analysis (Wireshark & Suricata)

Capture and analysis of network traffic to identify malicious patterns, using Wireshark for packet-level inspection and Suricata for signature-based detection.

## 🎯 Objective

To build the ability to look at raw network traffic and answer the question a SOC analyst is regularly asked: "is this connection normal, or is it something we need to worry about?"

## 🧰 Tools & Environment

| Component | Details |
|---|---|
| Packet Capture / Analysis | Wireshark |
| IDS/IPS Engine | Suricata |
| Traffic Source | *<!-- e.g. sample PCAPs from Malware-Traffic-Analysis.net, or lab-generated traffic -->* |
| Lab Setup | *<!-- e.g. isolated VM network -->* |

## 🔧 Methodology

1. **Capture / Source Acquisition**
   - *<!-- Describe whether traffic was captured live in your lab or sourced from public PCAP repositories for analysis practice -->*
2. **Wireshark Analysis**
   - Applied display filters to isolate traffic of interest (e.g. `http`, `dns`, `tcp.flags.syn==1`)
   - Followed TCP/HTTP streams to reconstruct full conversations
   - Identified anomalies: unusual ports, beaconing patterns, plaintext credentials, DNS tunneling indicators
3. **Suricata Detection**
   - Ran captured traffic through Suricata with the default/updated ruleset
   - Reviewed generated alerts (`fast.log` / `eve.json`) and matched them back to the relevant packets in Wireshark
4. **Correlation**
   - Cross-referenced Suricata alerts against manual Wireshark findings to validate true positives
   - Documented any traffic Suricata missed but manual analysis caught, and vice versa

## 📋 Analysis Summary

| Capture # | Traffic Type | Suricata Alert? | Verdict |
|---|---|---|---|
| 1 | *<!-- e.g. Port scan -->* | *<!-- Yes/No -->* | *<!-- Malicious/Benign -->* |
| 2 | *<!-- add more -->* | | |

## 🔍 Example Investigation

**Capture Description:** *<!-- what the traffic sample represents -->*
**Filter(s) Used:** *<!-- e.g. `ip.addr == x.x.x.x && tcp.port == 443` -->*
**Suricata Alert Triggered:** *<!-- signature name, e.g. ET MALWARE Suspicious User-Agent -->*
**Analysis:** *<!-- what the packets showed -->*
**Verdict:** *<!-- malicious / benign, with reasoning -->*
**Screenshot:** *<!-- Wireshark stream + Suricata alert log -->*

## 🧠 Skills Demonstrated

- Packet-level traffic analysis with Wireshark (filters, stream following)
- Signature-based detection using Suricata
- Correlating IDS alerts with raw packet evidence
- Identifying anomalous network behavior

## 📚 What I Learned

*<!-- 3-4 sentences: a traffic pattern that was hard to identify manually, how Suricata's alerts changed your approach, why packet-level validation matters even when a tool flags something automatically -->*

## 🔗 Related

Part of a 5-project SOC Analyst portfolio. See also: [Phishing Email Analysis](https://github.com/Ravi-KYadav/phishing-email-analysis) · [MITRE ATT&CK Mapping](https://github.com/Ravi-KYadav/mitre-attack-threat-intel-mapping)
