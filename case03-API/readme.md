# TECHNICAL LOG & API

## API
**CCNP Miguelangel Luna**

---

## CONTENIDOS:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude . |

[Google](https://www.google.com)

## 1. Introduction and Theoretical Framework

**API:** It is a "bridge" or interface that allows two software systems to communicate with each other, facilitating the use of another application's features without needing to know its internal code.

**Synchronous API:** It is one in which the client (the application making the request) sends a request and waits for the server to process the information and return the response in real time. During that time, the connection remains open and the process typically blocks until the result is received.

**Asynchronous API:** It is one in which the client sends a request and the server only confirms that it has received it (for example, by returning an acceptance code), without waiting for the task to finish. The server processes the operation in the background and, when completed, notifies the client through a notification (such as a webhook), a message, or by allowing the client to check the status later (polling).

![API types](images/00APItypes.jpg)

**Webhook:** is an automated communication mechanism between applications. In simple terms, **it is an event-based real-time notification.** It allows one application to automatically send data to another application only when a specific event occurs, instead of the second application having to constantly ask if there are updates.

**How does a Webhook work?**

1. **URL (Endpoint) Definition:** The client application provides a web address (URL) to the server.
2. **Event Trigger:** An action occurs on the server (for example: a customer makes a payment).
3. **Message Delivery:** The server automatically sends an HTTP request (usually via a POST request) with the event details to the registered URL.
4. **Reception and Action:** Your application receives the notification and immediately performs the corresponding action (for example: sends the invoice by email).

![Webhooks](images/01APIWebhooks.jpg)

**Common API Architectural Styles**

Although an application can create a freeform or unstructured interface to interact with third parties, the best practice is to follow specific standards, protocols, and architectural styles. This makes it much easier for developers to understand and use the API, as the concepts will be familiar to them.
The three most popular API architectural styles are:
1. **RPC (Remote Procedure Call):** Is a request-response model that lets an application (acting as a client) make a procedure call to another application (acting as a server). The "server" application is typically located on another system within the network.

RPC is an API style that can be applied to different transport protocols. Example implementations include:
- XML-RPC
- JSON-RPC
- NFS (Network File System)
- Simple Object Access Protocol (SOAP)

2. **SOAP (Simple Object Access Protocol):** SOAP is a messaging protocol. It is used for communicating between applications that may be on different platforms or built with different programming languages. It is an XML-based protocol that was developed by Microsoft. SOAP is commonly used with HyperText Transfer Protocol (HTTP) transport, but can be applied to other protocols. SOAP is independent, extensible, and neutral.
   
4. **REST (Representational State Transfer):** REST as a hybrid style, derived from several network-based architectural styles he described elsewhere in the paper, "combined with additional constraints that define a uniform connector interface."

   
## 2. Topology and BGP Neighbor Establishment







## 3. BGP Configuration:

**Router A (RTA - AS 100):**

```text
! 
router bgp 100
!
```

### 4. BGP Configuration:


