# 🏠 Home Lab SOC

A complete Blue Team home lab for SOC Tier 1 practice and portfolio.

## 🏗️ Architecture

    HOST (Windows PC)

    VM Ubuntu 26.04              VM Windows 11 Pro
    Wazuh Manager   <--->        Wazuh Agent (win11-bruno)
    192.168.56.104               192.168.56.105

    Network: VirtualBox Host-Only Adapter

## 🛠️ Stack

| Component | Version | Role |
|---|---|---|
| VirtualBox | 7.1.10 | Hypervisor |
| Ubuntu Server | 26.04 LTS | Manager OS |
| Wazuh Manager | 4.14.5 | Central SIEM |
| Windows 11 Pro | 25H2 (26200.8037) | Monitored endpoint |
| Wazuh Agent | 4.14.5 | Endpoint sensor |
| Sysmon | 15.20 | Advanced Windows logging |
| SwiftOnSecurity Config | master | Sysmon base ruleset |

## ✅ Setup Progress

- [x] Ubuntu Server VM — Wazuh Manager installed
- [x] Windows 11 Pro VM — Wazuh Agent active (win11-bruno)
- [x] Sysmon installed with SwiftOnSecurity config
- [x] Agent sending events to SIEM in real time
- [ ] Simulated attacks and detection (nmap, brute force, mimikatz)

## 📸 Screenshots

Coming soon — attack simulations and Wazuh dashboard alerts

## 📚 References
- [Wazuh Documentation](https://documentation.wazuh.com)
- [SwiftOnSecurity Sysmon Config](https://github.com/SwiftOnSecurity/sysmon-config)
- [MITRE ATT&CK](https://attack.mitre.org)
