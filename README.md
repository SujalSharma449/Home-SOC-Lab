# Home SOC Lab – Security Monitoring and Threat Detection

## Project Overview
This project demonstrates a hands-on Security Operations Center (SOC) lab built using Wazuh SIEM, Windows 10, and Kali Linux in a virtualized environment.

The objective was to configure endpoint monitoring, collect security events, investigate alerts, and perform controlled security testing.

## Lab Environment
- **SIEM:** Wazuh 4.14.9
- **Endpoint:** Windows 10
- **Attacker/Test Machine:** Kali Linux
- **Virtualization:** Oracle VirtualBox
- **Network:** Isolated SOC-LAB internal network

## Security Activities
- File Integrity Monitoring (FIM)
- Failed login detection
- User account creation monitoring
- Process creation monitoring
- PowerShell-related activity monitoring
- Microsoft Defender EICAR test
- Network connectivity and Nmap port scanning
- Firewall-drop alert observation

## Key Findings
- Windows 10 endpoint successfully connected to Wazuh.
- File creation and modification events were detected.
- Failed authentication and test account creation events were recorded.
- Process creation events were collected.
- Microsoft Defender detected the EICAR test file, and related events were visible in Wazuh.
- Nmap identified the Windows endpoint as reachable, with 100 scanned TCP ports reported as filtered.

## Limitations
- Dedicated Wazuh detection of the Nmap scan was not confirmed.
- Direct ingestion of the raw Windows firewall log file into Wazuh was not fully verified.
- Complete process command-line capture was not confirmed.

## Project Documentation
The detailed project report and supporting screenshots will be maintained in this repository.

## Disclaimer
This lab was created for educational and defensive cybersecurity learning in a controlled virtual environment. All testing was performed on systems under my control.
