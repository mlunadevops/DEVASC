# TECHNICAL LOG & ANSIBLE WEB SERVER

## ANSIBLE
**CCNP Miguelangel Luna**

---

## CONTENT:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude . |

[Google](https://www.google.com)

## 1. Introduction and Theoretical Framework

**Part 1:** Start the DEVASC VM.

**Part 2:** Configure Ansible (Inventory and Configuration).

**Part 3:** Verify communication with the Local Web Server.

**Part 4:** Create Playbooks to automate the installation of Apache.

**Part 5**: Add options to the Playbook (Change the port to 8081).

## 2. Topology and BGP Neighbor Establishment

![BGP WEIGTH](images/01Topologia.jpg)

## 3. ANSIBLE IMPLEMENTACION:

**3.1)** Configurar Ansible (Inventario y Configuración):

By default, the SSH server is turned off in the DEVASC VM to save resources. Ansible needs it to be on in order to connect to itself. Run in the terminal:

```text
sudo systemctl start ssh
```
**3.2)** : Open the working directory in VS Code. Open VS Code.

Go to File > Open Folder... and navigate to /labs/devnet-src/ansible.

We will work inside the ansible-apache folder.

**3.3)** Edit the inventory file **(hosts)**

Open the hosts file inside ansible-apache.

[webservers]

```text
[webservers]
192.0.2.3 ansible_ssh_user=devasc ansible_ssh_pass=Cisco123!
```






### 4. BGP Configuration:

