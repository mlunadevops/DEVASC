# TECHNICAL LOG & BGP ENGINEERING GUIDE

## Traffic Manipulation via the Weight Attribute
**CCNP Miguelangel Luna**

---

## CONTENIDOS:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude . |

[Google](https://www.google.com)

## 1. Introduction and Theoretical Framework

**Part 1:** Start the DEVASC VM.

Part 2: Configure Ansible (Inventory and Configuration).

Part 3: Verify communication with the Local Web Server.

Part 4: Create Playbooks to automate the installation of Apache.

Part 5: Add options to the Playbook (Change the port to 8081).



## 2. Topology and BGP Neighbor Establishment

The topology consists of four routers across different Autonomous Systems (AS 100, AS 200, AS 300, and AS 400). Before advertising prefixes, BGP neighbor adjacencies were established on each device.

![BGP WEIGTH](images/01Topologia.jpg)

 four routers across different Autonomous Systems (AS 100, AS 200, AS 300, and AS 400). Before advertising prefixes, BGP neighbor adjacencies were established on each device.

## 3. ANSIBLE IMPLEMENTACION:

**3.1)** Configurar Ansible (Inventario y Configuración):


**Router:**

```text
router bgp 100
```

### 4. BGP Configuration:

