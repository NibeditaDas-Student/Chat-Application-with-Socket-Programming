# Java Client–Server Chat Application

A simple **Client–Server Chat Application** built using **Java Socket Programming**, demonstrating real-time text communication between multiple clients and a server over TCP/IP.

---

## Project Overview

This project implements a basic chat system where:

* A **Server** listens for incoming client connections
* Multiple **Clients** can connect to the server
* Messages sent by one client are transmitted through the server
* Sound notification is played on message receipt

This project is ideal for understanding **network programming**, **sockets**, and **multithreading** in Java.

---

## Technologies Used

* **Java (JDK 8+)**
* **Socket Programming (TCP)**
* **Multithreading**
* **Java I/O Streams**

---

## Project Structure

```
ChatApplication/
│
├── client/
│   ├── Client.java        # Handles client-side socket communication
│   └── ClientMain.java    # Client application entry point
│
├── serverr/
│   ├── Server.java        # Manages server-side logic & client connections
│   └── ServerMain.java    # Server application entry point
│
├── sound/
│   └── chat_sound.mp3     # Notification sound for incoming messages
```

---

## How It Works

1. **Server starts first** and listens on a specific port.
2. **Clients connect** to the server using the server IP and port.
3. Messages typed by clients are sent to the server.
4. The server processes and forwards messages.
5. Clients receive messages and play a notification sound.

---

## How to Run the Project

### 1️⃣ Prerequisites

* Java JDK installed
* Command Prompt / Terminal

### 2️⃣ Compile the Project

```bash
javac ChatApplication/serverr/*.java
javac ChatApplication/client/*.java
```

### 3️⃣ Run the Server

```bash
java ChatApplication.serverr.ServerMain
```

### 4️⃣ Run the Client (in a new terminal)

```bash
java ChatApplication.client.ClientMain
```

 Run multiple clients to simulate a real chat environment.

---

## Features

* Real-time client-server communication
* Multiple client handling
* Sound notification on message arrival
* Clean separation of client and server logic

---

## Learning Outcomes

* Understanding **Java Sockets**
* Client–Server architecture
* Handling multiple connections using **threads**
* Java networking fundamentals

---

## Author

**Nibedita Das**

---

## License

This project is for **educational purposes** and open for learning and modification.
