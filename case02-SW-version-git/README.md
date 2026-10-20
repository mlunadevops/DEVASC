# TECHNICAL LOG & SOFTWARE VERSION CONTROL WITH GIT

## Version Control
**CCNP Miguelangel Luna**

---

## CONTENIDOS:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude . |

[Cisco Networking Academy](https://www.netacad.com/es/)

## 1. Introduction and Theoretical Framework

* **Local Scope:** It has meaning exclusively within the local router where it is configured and is not propagated via BGP routing updates to neighbors.


## 2. Topology and BGP Neighbor Establishment

The topology consists 

![BGP WEIGTH](images/01Topologia.jpg)

### 3. Github:

**Step 1:** Initialize Git and Configure Your User

In the terminal, run the following commands to configure your local identity (replace UsernameGitHub and mailgithub@example.com with your details or your GitHub username from now on):

**Linux SHELL (DEVASC):**

```text
! 
git config --global user.name "UsernameGitHub"
git config --global user.email "mailGithub@example.com"
!
```


```text
! 
git config --list
!
```


```text
! 
cd labs/devnet-src/
mkdir git-intro
cd git-intro
!
```
Initialize the Git repository and verify the creation of the hidden folder.

```text
! 
git config --list
ls -a
!
```
