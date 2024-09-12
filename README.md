# Wazuh Home SIEM Lab

## Overview
This project involves setting up a Wazuh-based Security Information and Event Management (SIEM) system to detect advanced threats like Mimikatz. The lab consists of a Wazuh server and a Windows 10 VM with Sysmon installed, configured as an agent.

## Architecture
- **Wazuh Server**: Deployed on a cloud-based virtual machine.
- **Windows 10 VM**: Configured with Sysmon on VirtualBox, acting as a Wazuh agent.

## Features
- Detection of Mimikatz, even with file name changes.
- Sysmon-only logging through modified `ossec.conf`.
- Event archiving enabled via Filebeats.
- Real-time event ingestion with custom Sysmon rules.

## Steps
1. **Wazuh Server Setup**: Installed on a virtual machine.
2. **Windows 10 Agent Setup**: Configured with Sysmon and added to Wazuh as an agent.
3. **Rule Modification**: Modified Sysmon rule to detect Mimikatz.
4. **Testing**: Ran Mimikatz to verify detection before and after file name change.


