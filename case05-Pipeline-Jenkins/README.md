# TECHNICAL LOG & Build a CI/CD Pipeline Using Jenkins

## CI/CD
**CCNP Miguelangel Luna**
---

## CONTENIDOS:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude . |

[Cisco Networking Academy](https://www.google.com)

## 1. Introduction and Theoretical Framework

The Weight attribute is a Cisco proprietary parameter used in BGP (Border Gateway Protocol) for best path selection. Its main characteristics are:

* **Local Scope:** It has meaning exclusively within the local router where it is configured and is not propagated via BGP routing updates to neighbors.

## 2. Topology and BGP Neighbor Establishment

The topology consists of four routers across different Autonomous Systems (AS 100, AS 200, AS 300, and AS 400). Before advertising prefixes, BGP neighbor adjacencies were established on each device.

![BGP WEIGTH](images/01Topologia.jpg)

## 3. CI/CD Pipeline Configuration:

3.1 **Send the Sample Application to Git**

Follow these steps in your virtual machine terminal:

#### 1. Configure your local Git credentials:
Replace `"Sample User"` with your real name and `user@example.com` with your email address (you can use your GitHub account details):

**Router A (RTA - AS 100):**

```text
! 
router bgp 100
!
```

### 4. BGP Configuration:

