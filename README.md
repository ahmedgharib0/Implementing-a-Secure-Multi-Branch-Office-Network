# 📡 Secure Multi-Branch Office Network (DEPI Graduation Project)

A hands-on graduation project under the **Digital Egypt Pioneers Initiative (DEPI)**.  
The objective was to **design, implement, and secure** a simulated enterprise network interconnecting a main office with multiple branches using **Cisco technologies**.

---

## 🛠️ Project Overview.

This project simulates a real-world enterprise network setup, focusing on:

- 🏢 Branch interconnectivity via VPN
- 🔐 VLAN segmentation
- 🚦 Routing protocols (OSPF with Authentication)
- 🔒 Site-to-site IPsec VPN
- 📜 Firewall rules & ACLs
- 🛡️ Security hardening and protection techniques

---

## 🧩 Network Architecture

- **Main Office** + **3 Branches** (HR, Finance, Sales)
- Interconnected over a **public network using IPsec VPN**
- Internal segmentation with **VLANs & Inter-VLAN Routing**
- **OSPF** for dynamic routing with authentication
- Multiple **security layers** including ACLs, firewall rules, and IDS/IPS

---

## 🖼️ Network Topology Diagram

![Network Design Diagram](./Project%20Design.png)

---

## 🔐 Key Features

- 🧱 VLANs & Subinterfaces for segmentation
- 📡 OSPF for routing between branches and main office
- 🔐 IPsec VPN tunnels for secure site-to-site communication
- 📜 ACLs to control inbound/outbound access
- 🛡️ IDS/IPS for intrusion detection testing
- 📄 Documented security policies and hardening methods

---

## 🧱 VLAN Design

### 🔹 Main Branch VLANs

| Department        | Devices Count | Description                           |
| ----------------- | ------------- | ------------------------------------- |
| HR                | ~15           | Staff PCs and printers                |
| CCTV              | ~25           | IP Cameras and NVRs                   |
| ATM               | ~6            | ATM Machines                          |
| Management        | ~8            | Executives’ desktops and laptops      |
| Voice             | ~251          | IP Phones across departments          |
| Guest             | ~251          | Visitors and mobile devices via Wi-Fi |
| Retail Banking    | ~40           | Tellers and front desk devices        |
| Credits and Loans | ~20           | Loan officers and support staff       |
| Customer Service  | ~25           | Support agents and service counters   |
| IT                | ~15           | Engineering and testing workstations  |
| Digital Banking   | ~10           | Developers and systems                |
| Manage            | ~16           | Network/Admin consoles                |

### 🔸 Branch VLANs (HR / Finance / Sales)

| Department        | Devices Count | Description                     |
| ----------------- | ------------- | ------------------------------- |
| CCTV              | ~25           | IP Cameras and NVRs             |
| ATM               | ~4            | ATM Machines                    |
| Management        | ~3            | Executives’ laptops             |
| Voice             | ~251          | IP Phones                       |
| Guest             | ~251          | Wi-Fi devices                   |
| Retail Banking    | ~8            | Front office devices            |
| Credits and Loans | ~10           | Loan officers and support staff |
| Customer Service  | ~8            | Support desks                   |
| IT                | ~3            | Tech staff systems              |
| Manage            | ~9            | Network/Admin consoles          |

---

## 🔐 Security Implementations

### 📍 Access Layer

| Feature                    | Description                               |
| -------------------------- | ----------------------------------------- |
| **Port Security**          | Restrict MAC addresses on switch ports    |
| **Disable Unused Ports**   | Shutdown of all unused interfaces         |
| **DHCP Snooping**          | Block rogue DHCP servers                  |
| **Dynamic ARP Inspection** | Protect against ARP spoofing              |
| **BPDU Guard**             | Prevents rogue STP attacks via user ports |
| **Disable CDP**            | Prevent exposure of device info           |

### ✅ Distribution & Core Layer Security

| Feature                 | Description                                  |
| ----------------------- | -------------------------------------------- |
| **ACLs**                | Control traffic flow between VLANs/sites     |
| **OSPF Authentication** | Only trusted routers can exchange routes     |
| **Passive Interface**   | Suppress OSPF updates on unneeded interfaces |

### ✅ Edge Router, DMZ, and Firewall Security

| Feature                 | Description                                    |
| ----------------------- | ---------------------------------------------- |
| **OSPF Auth + Passive** | Secure route advertisements                    |
| **Firewall Policies**   | Access rules for all zones                     |
| **Disable CDP**         | Limit info exposure                            |
| **VPN (IPsec)**         | Secure tunnel between branches                 |
| **NAT**                 | Public IP mapping for internal hosts           |
| **Disable Proxy ARP**   | Prevent man-in-the-middle and spoofing attacks |

---

## 🧪 Testing & Validation

- ✅ End-to-end **ping** and **traceroute** tests between all network segments
- 🔐 IPsec VPN tunnels confirmed via encryption inspection
- 🛑 ACLs validated with **allow/deny scenarios**
- 🔁 VLAN isolation and inter-VLAN communication tested
- 🔍 Wireshark used to inspect traffic and encryption

---

## 🧰 Tools & Technologies

- 🖥️ Cisco Packet Tracer / GNS3
- 💻 Cisco IOS CLI commands
- 🔎 Wireshark (for VPN traffic inspection)
- 🗺️ Microsoft Visio (for network diagrams)

---

## 🏁 Final Notes

This project demonstrates a secure and scalable enterprise network design using industry standards.  
We implemented layered security, optimized routing, and secure branch interconnectivity to simulate a real-world banking infrastructure.

---

## 🧑‍💻 Team Members

- [Ahmed Mohamed Gharib](https://www.linkedin.com/in/ahmedgharib0/).
- [Abdul Rahman Mohammed Hamed](https://www.linkedin.com/in/abdomohammed2410/)
- [Hassan Muhammed Abdelnabi](https://www.linkedin.com/in/hassan-abdalnabi-57533617b/)
- [Muhammed Sami Elhamzawy](https://www.linkedin.com/in/mosami74/)
- [Muhammed Mustafa Gomaa](https://www.linkedin.com/in/muhammed-gomaa/)

---

**Keywords:** DEPI, Network, Enterprise Network, VLAN, VPN, Cisco, Secure Network, Multi-Branch Network , Cisco , Network , OSPF , VTP
