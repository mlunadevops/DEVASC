# Technical Documentation: Installing 

## Traffic Manipulation via the Weight Attribute
**Miguelangel Luna**

---

[Proxmox Backup Server](https://www.proxmox.com/en/downloads/proxmox-backup-server)

## 1. Introduction and Theoretical Framework

### Proxmox Backup Server (PBS):

## 2. Prerequisites

Before deploying and executing the script on any new Proxmox VE server, ensure the following requirements are met:
1. **Proxmox VE Connected to PBS:** The PVE node must have the Proxmox Backup Server storage added to its configuration.
2. **Dependency Installation (`jq`):** The JSON processor must be present on the base operating system.
3. **Proxmox API Token:** An authentication token with administrator privileges is required to interact with the local API without needing plain-text passwords.

## 3. Implementation and Deployment Steps
Follow these steps on any new Proxmox VE server to make the restoration script fully operational:

### Step 1: Install the `jq` Dependency
Run the following command in the terminal to install the JSON processor:

**JQ Tool (pve shell)**

```text
& "C:\Program Files\Oracle\VirtualBox\VBoxManage.exe" modifyvm "com.cisco.csr1000v" --nictype1 virtio
```


![BGP WEIGTH](images/01Topologia.jpg)

 


### 4. BGP Configuration:
