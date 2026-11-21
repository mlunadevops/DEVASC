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

- **Parte 1:** Iniciar la VM DEVASC.
- **Parte 2:** Configurar Ansible (Inventario y Configuración).
- **Parte 3:** Verificar la comunicación con el Servidor Web Local.
- **Parte 4:** Crear Playbooks para automatizar la instalación de Apache.
- **Parte 5:** Agregar opciones al Playbook (Cambiar el puerto a 8081).



## 2. Topology and BGP Neighbor Establishment

The topology consists of four routers across different Autonomous Systems (AS 100, AS 200, AS 300, and AS 400). Before advertising prefixes, BGP neighbor adjacencies were established on each device.

![BGP WEIGTH](images/01Topologia.jpg)

 four routers across different Autonomous Systems (AS 100, AS 200, AS 300, and AS 400). Before advertising prefixes, BGP neighbor adjacencies were established on each device.

## 3. ANSIBLE IMPLEMENTACION:



**Router:**

```text
router bgp 100
```

### 4. BGP Configuration:

