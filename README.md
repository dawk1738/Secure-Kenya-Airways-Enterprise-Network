# ✈️ Kenya Airways (KQ) Enterprise Network Infrastructure

## 📖 Project Overview
This project focuses on designing and implementing a robust, scalable, and secure network for **Kenya Airways**. The architecture connects the **Nairobi HQ** and the **JKIA Branch**, ensuring 99.9% uptime for critical airline operations through a redundant hierarchical design.

## 🏗️ Network Architecture
The project follows the Cisco Three-Tier Hierarchical Model:
* **Core Layer:** Dual Cisco 2911 routers providing high-speed WAN routing between HQ and JKIA.
* **Distribution Layer:** Multilayer 3560 switches handling Inter-VLAN routing and redundancy.
* **Access Layer:** Cisco 2960 switches providing port-security and VLAN segmentation for HQ departments.

## 🔒 Security & Services
* **Perimeter Defense:** Cisco ASA 5505 Firewall managing traffic between Inside, Outside (Internet), and DMZ zones.
* **DMZ (Demilitarized Zone):** Isolated server farm hosting public-facing Web and Email services.
* **Departmental VLANs:** Dedicated segments for Admin, Finance, Flight Ops, and IT Support.
* **Guest Services:** Secure WPA2-protected Wireless Access Point for JKIA passenger lounge, isolated from internal traffic.

## 🛠️ Tools Used
* **Cisco Packet Tracer 8.x**
* **VLSM (Variable Length Subnet Masking)** for optimized IP addressing.
* **CLI (Command Line Interface)** for manual device configuration.

## 🚀 How to Run
1. Download and install **Cisco Packet Tracer**.
2. Clone this repository or download the `.pkt` file.
3. Open the file to view the topology and test pings between departments.
