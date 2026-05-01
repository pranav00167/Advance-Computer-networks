# 🏢 Small Office Network Design (Cisco Packet Tracer)

## 📌 Overview

This project simulates a **small office network** using Cisco Packet Tracer.
It demonstrates how multiple departments can be interconnected using **routers, switches, and subnetting**, enabling efficient communication across different networks.

---

## 🧠 Network Architecture

The network is divided into **four departments**, each operating on a separate subnet:

| Department          | Network        | Gateway     |
| ------------------- | -------------- | ----------- |
| Chairman            | 192.168.1.0/24 | 192.168.1.1 |
| IT Department       | 192.168.2.0/24 | 192.168.2.1 |
| Computer Department | 192.168.3.0/24 | 192.168.3.1 |
| Server Room         | 1.0.0.0/24     | 1.0.0.1     |

---

## 🔗 Network Topology

* Each department has its own **switch (LAN)**
* Two routers are used:

  * **Main Router** → connects Computer Dept + Server Room
  * **Router-1** → connects IT Dept + Chairman Dept
* Routers are connected via a **backbone network (10.0.0.0/30)**

---

## 🧱 Components Used

### 🔹 End Devices

* PCs (Employees, Managers, Chairman, VC)
* Laptop
* Server
* Printers

### 🔹 Network Devices

* Switches (for LAN communication)
* Routers (for inter-network communication)

---

## ⚙️ IP Addressing Scheme

### 📍 Computer Department (192.168.3.0)

* Gateway: 192.168.3.1
* Devices: 192.168.3.2 – 192.168.3.6

### 📍 IT Department (192.168.2.0)

* Gateway: 192.168.2.1
* Devices: 192.168.2.2 – 192.168.2.5

### 📍 Chairman Department (192.168.1.0)

* Gateway: 192.168.1.1
* Devices: 192.168.1.2 – 192.168.1.3

### 📍 Server Room (1.0.0.0)

* Gateway: 1.0.0.1
* Server: 1.0.0.2
* Laptop: 1.0.0.3

### 📍 Router Interconnection

* Network: 10.0.0.0/30
* Main Router: 10.0.0.1
* Router-1: 10.0.0.2

---

## 🔄 Working of the Network

### 🟢 Within Same Department (LAN)

* Communication happens through **switches**
* Uses **MAC addresses (Layer 2)**

### 🔵 Between Different Departments

* Data is sent to the **default gateway (router)**
* Router forwards packets using **routing table (Layer 3)**

---

## 📡 Example Data Flow

### 🔹 IT PC → Server

1. PC sends packet to gateway (192.168.2.1)
2. Router-1 forwards to Main Router (10.0.0.1)
3. Main Router sends to Server (1.0.0.2)

### 🔹 Computer Dept → Chairman

1. PC → Switch → Main Router
2. Main Router → Router-1
3. Router-1 → Chairman PC

---

## 🧪 Testing & Verification

### ✔ Ping Test

```bash
ping 1.0.0.2
```

### ✔ Routing Table

```bash
show ip route
```

---

## 🧠 Key Concepts Used

* IP Addressing & Subnetting
* LAN & WAN Communication
* Switching (Layer 2)
* Routing (Layer 3)
* Default Gateway
* Inter-network communication

---

## 🌍 Real-World Application

This project represents a **real office network** where:

* Each department has its own network
* A central server provides services
* Routers ensure communication between departments

---

## 🏁 Conclusion

The network successfully enables communication between multiple departments using structured subnetting and routing.
It demonstrates a scalable and efficient design for a small office environment.

---

## 🚀 Author

**Pranav Bhardwaj**

---

