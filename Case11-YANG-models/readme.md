# TECHNICAL LOG & AUTOMATION ENGINEERING GUIDE

## YANG MODELS
**CCNP Miguelangel Luna**

---

## CONTENIDOS:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude . |

[Google](https://www.google.com)

## 1. Introduction and Theoretical Framework

Explore YANG Models
Objectives

**Part 1:** Start the DEVASC VM.

**Part 2:** Explore a YANG model on GitHub and download it to the VM.

**Part 3:** Use pyang to transform the YANG model into a readable format (tree).




## 2. Topology and BGP Neighbor Establishment

![BGP WEIGTH](images/01Topologia.jpg)

## 3. IMPLEMENTATION:

**Step 3.1:** Explore the model in the browser
Open the Chromium browser inside the DEVASC VM.

Go to the URL: **https://github.com/YangModels/yang**

On the master branch, navigate through the folders until you reach the IOS XE 16.9.3 version:

vendor > cisco > xe > 1693

Look for the **ietf-interfaces.yang** file and open it.

You will see the source code of the model. If you are familiar with Cisco's show interfaces, you will see concepts such as leaf enabled (which is a boolean that indicates whether the interface is active or not)

```text
python3 -m venv csr1kv
```

```text
pyats --help
```
