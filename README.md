# SOC Analyst Home Lab

## Project Overview
This SOC lab simulates a real Security Operations Center using Wazuh (SIEM/XDR), Snort IDS, Windows endpoint monitoring, and Kali Linux attack traffic. The environment collects and correlates logs from endpoints, detects network intrusions, monitors file integrity, and provides visibility into system activity across the network.

I built this project to understand how modern SOC tools detect threats across endpoints and networks. By integrating Wazuh and Snort, then generating traffic from Kali, the lab demonstrates log collection, alerting, intrusion detection, and event correlation, core skills required in SOC Analyst Level 1 roles.

## Features
- **Bulk User Creation**: Automated generation of 1,000+ AD accounts via PowerShell
- **Domain Configuration**: Deployed forest (mydomain.com) with OUs and security groups
- **Network Services**: Configured DHCP scopes (172.16.0.0/24) and DNS for client connectivity
- **Virtual Lab**: Built dual-network environment in VirtualBox (NAT + Internal)
- **Client Integration**: Successfully joined Windows 10 clients to the domain

## Technologies & Skills Gained

### Technical Skills
- **SIEM Deployment:** Wazuh Manager installation and configuration
- **IDS Configuration**: Snort installation, rule configuration, syslog output
- **XDR Concepts**: Endpoint telemetry, process monitoring, agent registration
- **File Integrity Monitoring**: Windows directory monitoring using Wazuh
- **Log Correlation**: Multi-source log ingestion (Windows, Ubuntu, Snort)
- **Linux Administration**: Ubuntu Server setup, systemctl, permissions, config editing
- **Network Scanning**: Nmap & ping sweeps from Kali Linux
- **Virtualization**: Multi-VM setup on VirtualBox (Ubuntu & Kali)
- **Troubleshooting**: Agent connectivity, permissions, syslog parsing

### Soft Skills Developed
- Process Automation
- Technical Documentation

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
