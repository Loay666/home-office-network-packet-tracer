# home-office-network-packet-tracer
# 🚀 Full Home & Office Network Simulation – Cisco Packet Tracer

## 💡 Project Overview

This project is a complete simulation of a hybrid wired and wireless network, implemented in **Cisco Packet Tracer**, combining everything learned across 17 modules of the **Cisco Networking Essentials** curriculum.

It includes full configuration of:

* IP addressing (IPv4 & DHCP)
* Switching & routing
* Wireless setup
* Application layer services (HTTP, FTP, DNS)
* Network testing & troubleshooting tools

> 📁 File: `PROJECT1.pkt`

---

## 🧠 What You Will Learn

* 🤩 Network topology design (LAN + WLAN)
* ⚙️ Manual interface configuration (IP, subnetting)
* 📶 Wireless configuration (SSID, security, DHCP)
* 🛡️ Router setup and inter-VLAN routing
* 🧪 Network testing tools (ping, tracert, ipconfig)
* 🛠️ Simulation and packet-level analysis

---

## 💻 Network Topology

```
               [Cloud (ISP)]
                      |
                 [Router]
                /        \
         [Switch1]      [Switch2]
         /   |   \           |
     PC1  PC2  Server   Wireless Router
                                |
                          [Wi-Fi Clients]
                          Laptop1, PC3
```

---

## 🧾 IP Addressing Plan

| Device          | Interface     | IP Address         | Role             |
| --------------- | ------------- | ------------------ | ---------------- |
| Router          | Fa0/0         | 192.168.1.1        | Gateway for LAN1 |
| Router          | Fa1/0         | 192.168.2.1        | Gateway for LAN2 |
| Router          | Serial2/0     | 10.0.0.1           | Internet Gateway |
| Server          | -             | 192.168.1.100      | FTP / HTTP / DNS |
| PC1             | -             | DHCP (192.168.1.x) | Client           |
| PC2             | -             | DHCP (192.168.1.x) | Client           |
| Switch1         | VLAN1         | 192.168.1.2        | Management       |
| Switch2         | VLAN1         | 192.168.2.2        | Management       |
| Wireless Router | Internet Port | 192.168.2.254      | DHCP for WiFi    |
| Laptop1 / PC3   | Wi-Fi         | DHCP (192.168.2.x) | Wireless Clients |

---

## ⚙️ Configuration Summary

* **Router**:

  * IP Addressing
  * Interface activation (`no shutdown`)
  * Static routes (if cloud used)
  * DHCP pools for clients

* **Switches**:

  * VLAN1 configuration
  * No shutdown on ports

* **Wireless Router**:

  * Custom SSID
  * WPA2 Security
  * DHCP enabled for WiFi clients

* **End Devices**:

  * Static IP for server
  * DHCP for all clients

---

## 🔧 Tools Used

* 🧠 Cisco Packet Tracer 8.x
* 👨‍💻 CLI (Command Line Interface)
* 📶 Wireless interface simulation
* 🛁 IP Configuration + DHCP Pools
* 🛠️ Testing: `ping`, `tracert`, `ipconfig`

---

## 🧪 Example Testing Commands

```bash
C:\> ping 192.168.1.1
C:\> ping 192.168.1.100
C:\> ipconfig
C:\> tracert 8.8.8.8
```

---

## ✅ Status

* ✅ Devices configured
* ✅ Network simulated successfully
* ✅ All PCs can ping each other
* ✅ Server tested (ping, HTTP, FTP)
* ✅ Wireless connectivity works

---

## 📸 Screenshots

> Add screenshots of your topology + successful pings

---

## 📌 Author

* 👨‍💼 **Loay Mohamed Abdelfattah**
* 💼 Student in Computer Science | Cybersecurity Track
* 🇪🇬 Egypt
* 🌐 [LinkedIn Profile](https://www.linkedin.com/in/YOUR_USERNAME)
