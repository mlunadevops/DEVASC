# TECHNICAL LOG & DOCKER CONTAINER

## DOCKER CONTAINERS
**CCNP Miguelangel Luna**

---

## CONTENIDOS:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude . |

[Docker](https://www.netacad.com/es/)

## 1. Introduction and Theoretical Framework

The Weight attribute is a Cisco proprietary parameter used in BGP (Border Gateway Protocol) for best path selection. Its main characteristics are:

* **Local Scope:** It has meaning exclusively within the local router where it is configured and is not propagated via BGP routing updates to neighbors.

## 2. Build a Sample Web App in a Docker Container
 
**Part 2.1:** Launch the DEVASC VM

* Launch the DEVASC Virtual Machine using VirtualBox or VMWare.

Bash scripting is a prerequisite for automation, CI/CD, and managing development environments. 

1. **Create and navigate to the working directory**:
   
```bash
   cd labs/devnet-src/sample-app/
```
```bash
   touch user-input.sh
```

2.**Open the file in nano and add the shebang and script logic:**

```bash
   nano user-input.sh
```

3. **Add the initial content (the shebang line and the commands to prompt for the name):**

```bash
   #!/bin/bash
   echo -n "Enter Your Name: "
   read userName
   echo "Your name is $userName."
```
4. **Grant execution permissions and rename the file:**

```bash
   chmod a+x user-input.sh
```
```bash
   mv user-input.sh user-input
```

5. 


![BGP WEIGTH](images/01Topologia.jpg)

 four routers across different Autonomous Systems (AS 100, AS 200, AS 300, and AS 400). Before advertising prefixes, BGP neighbor adjacencies were established on each device.

## 3. BGP Configuration:

**Router A (RTA - AS 100):**

```text
! 
router bgp 100
!
```

### 4. BGP Configuration:

