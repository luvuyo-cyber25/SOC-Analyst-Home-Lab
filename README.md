# SOC Analyst Home Lab

## Project Overview
This SOC lab simulates a real Security Operations Center using Wazuh (SIEM/XDR), Snort IDS, Windows endpoint monitoring, and Kali Linux attack traffic. The environment collects and correlates logs from endpoints, detects network intrusions, monitors file integrity, and provides visibility into system activity across the network.

I built this project to understand how modern SOC tools detect threats across endpoints and networks. By integrating Wazuh and Snort, then generating traffic from Kali, the lab demonstrates log collection, alerting, intrusion detection, and event correlation, core skills required in SOC Analyst Level 1 roles.

## Features
- **Wazuh SIEM Deployment**: Installed Wazuh Manager + Dashboard on Ubuntu Server
- **Windows Endpoint XDR**: Installed and registered Wazuh Agent on Windows
- **File Integrity Monitoring**: Real-time monitoring of Windows directory changes
- **Snort IDS Integration**: Configured Snort alerts to feed into Wazuh SIEM
- **Network Attack Simulation**: Performed ping sweeps, Nmap scans, and traffic tests from Kali Linux
- **Alert Correlation**: Combined IDS & FIM activity into a single dashboard
- **Log Analysis**: Parsed alerts for process activity, file changes, and network intrusions

## Tools & Skills Gained

### Technical Skills
- **SIEM Deployment**: Installed and configured Wazuh Manager
- **IDS Configuration**: Snort installation, rules, and syslog outpu
- **XDR Concepts**: Endpoint telemetry, agent registration, and monitoring
- **File Integrity Monitoring**: Windows directory monitoring via Wazuh Agent
- **Incident Response**: Observed alerts and analyzed potential threats
- **Log Correlation**: Aggregated logs from Windows, Ubuntu, and Snort
- **Linux Administration**: Ubuntu Server setup, systemctl, config editing
- **Kali Linux**: Nmap scanning, ping sweeps, and traffic simulation
- **Network Scanning**: Active scanning to generate test alerts
- **Virtualization**: Multi-VM lab setup in VirtualBox
- **Configuration Management**: Edited configs for Wazuh and Snort integration
- **Security Monitoring**: Continuous log and network monitoring
- **Endpoint Monitoring**: Observed Windows agent telemetry
- **Alert Analysis**: Viewed, filtered, and interpreted alerts on Waz

## Screenshots
1. **VirtualBox Network Configuration**  
   ![Network Setup](vbox_network.png)  
   *Dual adapter configuration (NAT + Internal)*

2. **OU Structure & Admin Creation**  
   ![ADMINS OU](admins_ou.png)  
   *Organizational Unit design with _ADMINS group and custom admin user*

3. **PowerShell Automation**  
   ![PS Script](powershell_script.png)  
   *Bulk user creation script output*

4. **DHCP Scope Configuration**  
   ![DHCP Setup](dhcp_scope.png)  
   *172.16.0.100/24 scope with gateway*

5. **Client Domain Join**  
   ![Joined Client](client_join.png)  
   *CLIENT1 successfully joined to domain*

6. **User Login Test**  
   ![Login Test](user_login.png)  
   *Domain user authentication*

7. **AD Users & Computers**  
   ![ADUC View](ad_users.png)  
   *1,000+ users in OU structure*

## Installation
1. **Requirements**:
   - Oracle VirtualBox
   - Linux Ubuntu 20.04+ (ISO)
   - Kali Linux VM
