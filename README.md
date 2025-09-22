# Above-Basic VPN Network Configuration

This project demonstrates the implementation of an IPSec VPN tunnel paired with advanced ACL (Access Control List) configurations on Cisco routers. The goal is to securely connect two different LANs over an untrusted WAN (simulated ISP) while applying granular access control between the sites.

![Network Topology](./path/to/your/image.png) <!-- Replace with actual image path if committed. -->

---

## 📝 Project Overview

The network topology consists of:

- **Two LANs** (192.168.10.0/24 and 192.168.20.0/24)
- **Two edge routers** (R1 and R2, Cisco 2911)
- **An ISP router** simulating the public network
- **Switches and PCs at each site**
- **IPSec VPN** configured between R1 and R2
- **Advanced ACLs** on routers to restrict/allow traffic as required

This setup is intended for testing and learning about site-to-site VPNs and advanced ACL filtering in Cisco environments.

---

## 🖥️ Network Diagram

![Network Diagram](image1) <!-- Reference to the image provided by the user. -->

---

## ⚙️ Key Features

- **IPSec Site-to-Site VPN**: Provides secure, encrypted communication between two remote LANs.
- **Advanced ACL Configuration**: Controls which traffic is permitted through the VPN, allowing for granular security policies.
- **Realistic Topology**: Simulates a real-world scenario with two branch offices and an ISP.

---

## 📑 Setup Details

- **LAN 1 (Blue Box):**
  - Network: `192.168.10.0/24`
  - Devices: PC0, PC1
  - Switch: 2960-24TT
  - Router: 2911 (R1)
- **LAN 2 (Green Box):**
  - Network: `192.168.20.0/24`
  - Devices: PC2, PC3
  - Switch: 2960-24TT
  - Router: 2911 (R2)
- **ISP Router**: 2911
- **WAN Links:**
  - R1 <-> ISP: `20.20.20.0` network
  - ISP <-> R2: `30.30.30.0` network

---

## 🔒 Security Components

- **IPSec Configuration**: Ensures confidentiality, integrity, and authenticity of packets exchanged between R1 and R2.
- **Advanced ACLs**: Applied on tunnel and LAN interfaces to control which subnets, protocols, or hosts are allowed or denied across the VPN.

---

## 🚀 Usage

1. **Clone the Repo**:
   ```bash
   git clone https://github.com/Srisudharson/Above-Basic-VPN-Network-Configuration.git
   ```
2. **Open the Project** in Cisco Packet Tracer or your preferred network simulator.
3. **Review Router Configurations** for IPSec and ACL setup.
4. **Test Connectivity**:
   - Try to ping between PCs in different sites to verify VPN and ACL functionality.
   - Modify ACLs to see their effect on permitted/denied traffic.

---

## 📂 Files

- `R1_Config.txt` – Sample configuration for R1 (IPSec + ACL)
- `R2_Config.txt` – Sample configuration for R2 (IPSec + ACL)
- `ISP_Config.txt` – Sample configuration for ISP router
- `*.pkt` – Packet Tracer project files (if provided)
- `README.md` – Project documentation

---

## 🧑‍💻 Author

- **Srisudharson**  
  [GitHub Profile](https://github.com/Srisudharson)

---

## 📜 License

This project is for educational and testing purposes.

---

## 📷 Topology Reference

![Network Topology Reference](image1)

---

Feel free to explore, modify, and learn!
