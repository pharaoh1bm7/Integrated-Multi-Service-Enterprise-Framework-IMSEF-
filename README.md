# Integrated Multi-Service Enterprise Framework (IMSEF) 🌐📞

<img width="1399" height="839" alt="Screenshot 2026-04-05 092535" src="https://github.com/user-attachments/assets/98a42d1f-2380-40ae-89bc-421b6fb48ef9" />

---


**IMSEF** is a comprehensive network infrastructure simulation designed to model a robust, scalable, and converged enterprise environment. The project integrates multi-site routing, switching, and Voice over IP (VoIP) services into a single unified framework.

## 📌 Project Overview
This framework simulates a corporate network consisting of four interconnected main branches (Top, Right, Bottom, and a Data Center/Left branch). It demonstrates the seamless integration of data and voice services across a distributed topology using Cisco technologies.



---

## 🛠️ Technical Stack & Features

### 1. Network Core (Routing)
* **Dynamic Routing:** Implemented **OSPF (Open Shortest Path First)** to ensure high availability and dynamic path selection between the 4 routers.
* **Redundancy:** Configured for resilient communication, allowing traffic to reroute automatically in case of link failure.
* **Inter-VLAN Routing:** Enabled communication between different departments while maintaining broadcast domain isolation.

### 2. Voice over IP (VoIP)
* **Telephony Service:** Configured Cisco IP Phones (7960 series) with unique directory numbers (101, 201, 301).
* **Dial-Peers:** Established VoIP dial-peers to route calls across the wide-area network (WAN) links.
* **Voice VLANs:** Segregated voice traffic from data traffic to ensure Quality of Service (QoS).

### 3. Services & End-Devices
* **DHCP Services:** Centralized and localized DHCP pools for automated IP assignment to Laptops, PCs, and IP Phones.
* **Server Farm:** Integrated dedicated servers (HTTP, DNS, etc.) to simulate a real-world Data Center environment.
* **Endpoint Diversity:** Support for various devices including Printers, Laptops, and Desktop PCs across all branches.

---

## 🏗️ Topology Architecture
The network follows a mesh-like core topology:
* **Top Branch:** Serving workstations and IP Phone 101.
* **Right Branch:** Serving workstations and IP Phone 201.
* **Bottom Branch:** Serving mobile users (Laptops) and IP Phone 301.
* **Data Center (Left):** Hosting critical enterprise server resources.



---

## 🚀 How to Run the Simulation
1.  Download the `.pkt` file from this repository.
2.  Open it using **Cisco Packet Tracer** (v8.0 or higher recommended).
3.  Wait for the OSPF convergence (green lights on all serial links).
4.  Test connectivity using `Ping` or the `IP Phone` tool to place calls between branches.

---

## 📝 Author
**Belal Eladawy**
---

