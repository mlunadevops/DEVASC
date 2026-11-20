# TECHNICAL LOG & Ansible to Back Up and Configure a Device

## ANSIBLE CISCO

**CCNP Miguelangel Luna**

---

## CONTENT:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude . |

[Google](https://www.google.com)

## 1. Introduction and Theoretical Framework

Use Ansible to Back Up and Configure a Device, objectives:

**Part 1:** Start the DEVASC VM and the CSR1000v VM.

**Part 2:** Configure Ansible.

**Part 3**: Use Ansible to back up the configuration.

**Part 4:** Use Ansible to configure a device (IPv6).
---

## Parte 1: Iniciar las VMs

1. Asegúrate de tener encendida y funcionando tu máquina virtual **DEVASC**.
2. Asegúrate de tener encendida tu máquina virtual **CSR1000v** (con la IP `192.168.56.101` o la que le haya asignado tu red).
3. Desde la terminal de la VM DEVASC, verifica la conectividad haciendo un ping al router:
   ```bash
   ping 192.168.56.101

The:

* **Local Scope:** It has meaning exclusively within the local router where it is configured and is not propagated via BGP routing updates to neighbors.

## 2. Topology and BGP Neighbor Establishment

The topology.

![BGP WEIGTH](images/01Topologia.jpg)

 four routers across different Autonomous Systems (AS 100, AS 200, AS 300, and AS 400). Before advertising prefixes, BGP neighbor adjacencies were established on each device.

## 3. BGP Configuration:

**Router:**

```text
router bgp 100
```
