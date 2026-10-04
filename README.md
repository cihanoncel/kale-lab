# KALE — Home Defense Lab

A layered home-network defense lab: DNS filtering, intrusion detection, and SIEM log aggregation running 24/7 on local hardware.

## Architecture

| Layer | Tool | Role |
|---|---|---|
| DNS filtering | Pi-hole | Blocks malicious/tracker domains |
| IDS | Suricata | Network intrusion detection |
| SIEM | Wazuh | Log aggregation, alerting, dashboard |

## Detection engineering

Custom detection rules written for this lab (brute-force attempts, phishing domains, anomalous night-time traffic). Each rule is documented with its logic and test evidence.

## Triage process

Alert → checklist → analysis → incident note. AI-assisted triage workflow, documented end-to-end.

## Metrics

- Blocked malicious domains (30-day rolling)
- Alerts triaged per week
- Mean time to triage in lab conditions

## Status

🛠️ Planned — build starts after hardware decision (Raspberry Pi vs. repurposed PC).

> **Note:** This is a home lab built for learning. All systems monitored are owned by the lab operator. No production data.
