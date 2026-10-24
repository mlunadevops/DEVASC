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

2.1 **Create and navigate to the working directory**:
   
```bash
   cd labs/devnet-src/sample-app/
```
```bash
   touch user-input.sh
```

2.2 **Open the file in nano and add the shebang and script logic:**

```bash
   nano user-input.sh
```

2.3 **Add the initial content (the shebang line and the commands to prompt for the name):**

```bash
   #!/bin/bash
   echo -n "Enter Your Name: "
   read userName
   echo "Your name is $userName."
```
2.4 **Grant execution permissions and rename the file:**

```bash
   chmod a+x user-input.sh
```
```bash
   mv user-input.sh user-input
```

![Program Excution](images/01Docker.png)

3. **Moving on to Part 3: Create a Sample Web App**

In this part, we will create a simple Python web application using the **Flask** framework, which will display the IP address of the client making the request.

Follow these steps in your terminal inside the DEVASC VM:

3.1 **Install Flask and open the port in the firewall (if necessary):**
   
```bash
sudo apt update && sudo apt install -y python3-pip
pip3 install flask
```

3.2 **Create / open the `sample_app.py` file:**

```bash
nano sample_app.py
```

```bash
from flask import Flask
from flask import request

sample = Flask(__name__)

@sample.route("/")
def main():
    return "You are calling me from " + request.remote_addr + "\n"

if __name__ == "__main__":
    sample.run(host="0.0.0.0", port=8080)
```
```bash
python3 sample-app.sh
```

![Program Execution WEB](images/02Executionweb.png)

3.3 **Open another terminal and use curl:**

```bash
curl http://0.0.0.0:8080
```
![Program Execution CURL](images/03Executionweb.png)

4 **Moving on to Part 4: Configure the Web App to Use Website Files**

Now we will expand our application to use static HTML and CSS files instead of returning plain text directly from Python.

Follow these steps in your terminal (make sure you stopped the previous server with `CTRL + C` if it was still running):

4.1 **Explore the existing directories (`templates` and `static`):**

Previous folders with `index.html` and `style.css` already exist. You can check their content with:

```bash
   cat templates/index.html
   cat static/style.css
```

4.2 **Update the `sample_app.py` code:**

Edit your `sample_app.py` file to import `render_template` and render the HTML template.

```bash
 from flask import Flask
from flask import request
from flask import render_template

sample = Flask(__name__)

@sample.route("/")
def main():
    return render_template("index.html")

if __name__ == "__main__":
    sample.run(host="0.0.0.0", port=8080)
```

```bash
python3 sample_app.py
```
