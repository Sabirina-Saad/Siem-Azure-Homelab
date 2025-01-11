# Siem-Azure-Homelab

## Introduction
In this project I deployed Azure Virtual Machine(VM) as a honeypot. The main goal of this project was to get practical knowledge on how Azure Sentinel Siem detects real-time threats and visualize them. I used ingested logs sources from windows event logs for failed RDP attacks into Log Analytics workspace, which is then used by Microsoft Sentinel to build attack maps. I observed live RDP Brute Force attacks from all around the world as the VM was exposed as vulnerable on the internet. 

### Step details of the project
This section explains the steps I followed to ensure the successful completion of this project.
1. Create Azure VM: I configured and deployed Azure VM as a honeypot while also configuring RDP access to the VM.
2. Create Log Analytics Workspace to ensure it collects logs from Windows log events especially failed login attempts. This Log Analytics also contains custom Log that contains the geographic information of the attacker by using IP Geolocation API.
3.  Create Azure sentinel to visualize attack data and security threats.
4. Use custom powershell script to extract failed RDP logon logs from windows event viewer by providing attackers geolocation information.
5.  Use Geolocation API to get details geographic location on the attackers login.
6.  Create custom logs to extract fields

### Snapshot of the project
![Capture](https://github.com/user-attachments/assets/99e8e4e0-0e69-42ce-86af-8ff990445db2)

![Capture2](https://github.com/user-attachments/assets/8c51fadf-61b8-4e68-878d-9724b8114b9b)





