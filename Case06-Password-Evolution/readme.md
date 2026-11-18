# TECHNICAL LOG & EXPLORE THE EVOLUTION OF PASSWORD METHODS

## DEVASC
**CCNP Miguelangel Luna**

---

## CONTENIDOS:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude . |


[Google](https://www.google.com)

## 1. Introduction and Theoretical Framework

**A library:** is a collection of reusable code — functions, classes, modules — that someone else has already written and packaged so that you can use it in your own programs without having to reinvent it. A library can be a small piece of reusable code, like a function called **sumar.py that takes two variables (A and B) and returns a result (C) using the formula A + B = C**. You don't need to know how it works internally; you just call it and use the result

Example. the library **sumar.py** :


# sumar.py  (una librería)
def sumar(a, b):
    return a + b

## 2. Topology and BGP Neighbor Establishment

The topology consists of four routers across different Autonomous Systems (AS 100, AS 200, AS 300, and AS 400). Before advertising prefixes, BGP neighbor adjacencies were established on each device.

![BGP WEIGTH](images/01Topologia.jpg)



## Part 3: Install Packages and Create a Web Service:

In your DEVASC VM, open VS Code, go to File > Open Folder... and select the **labs/devnet-src/security folder.**

Open the **password-evolution.py** file.

Open a terminal in VS Code (Terminal > New Terminal) and run the installation of the necessary packages.

**What is PyOTP?** 

PyOTP is a Python library for generating and verifying time-based one-time passwords (TOTP) and counter-based one-time passwords (HOTP). It is mainly used to implement **two-factor authentication (2FA)**.

**What is Flask?**

Flask is a micro web framework for Python. It is used to build web applications and APIs in a lightweight and flexible way. It is called "micro" because it includes only the essentials and lets you add the rest as needed (unlike heavier frameworks such as Django).

**What is it used for?**
With Flask you can:

Create websites and REST APIs.

Define routes (URLs) and associate them with Python functions.

Handle HTTP requests (GET, POST, etc.) and return responses.

Render HTML templates (with Jinja2).

Manage sessions, cookies, and forms.

Serve static files (CSS, JS, images).

**PYOTP and FLASK installation:**

```text
pip3 install pyotp
pip3 install flask
```

### 4. BGP Configuration:

