<h1 align=center> 🌐 Design and Simulation of a Resilient Network Infrastructure for INTECH Computer Systems (Pvt.) Ltd. </h1>

<p align="center">
  <strong>An Individual Academic Project Focused on Designing, Implementing and Simulating Enterprise Network Infrastructure using GNS3</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Project-Individual-2563EB" alt="Individual Project">
  <img src="https://img.shields.io/badge/GNS3-Network%20Simulation-5A9A3A" alt="GNS3">
  <img src="https://img.shields.io/badge/Cisco-IOS-00AEEF" alt="Cisco IOS">
  <img src="https://img.shields.io/badge/VLAN-Network%20Segmentation-8B5CF6" alt="VLAN">
  <img src="https://img.shields.io/badge/OSPF-Dynamic%20Routing-10B981" alt="OSPF">
  <img src="https://img.shields.io/badge/HSRP-High%20Availability-F59E0B" alt="HSRP">
  <img src="https://img.shields.io/badge/DHCP-IP%20Address%20Management-0891B2" alt="DHCP">
  <img src="https://img.shields.io/badge/STP-Loop%20Prevention-EF4444" alt="STP">
  <img src="https://img.shields.io/badge/ACL-Network%20Security-DB2777" alt="ACL">
  <img src="https://img.shields.io/badge/Wireshark-Packet%20Analysis-2563EB" alt="Wireshark">
</p>

---

## 📌 Project Overview

This individual project focuses on the design and simulation of a scalable, secure, and resilient enterprise network infrastructure for **INTECH Computer Systems (Pvt.) Ltd.**

The project addresses challenges identified in the existing network environment, including scalability limitations, unreliable connectivity, network management difficulties, security vulnerabilities, and the lack of effective redundancy mechanisms.

A structured enterprise network architecture was designed and implemented using **GNS3**, incorporating hierarchical network design, VLAN-based segmentation, dynamic routing, automated IP address allocation, redundancy, and network security mechanisms.

The proposed infrastructure aims to improve network reliability, strengthen internal security, simplify network management, and support future organizational expansion.

---

## 🎯 Project Objectives

The primary objectives of this project are to:

- Design a scalable and structured enterprise network topology.
- Implement VLAN-based network segmentation.
- Configure inter-VLAN routing for departmental communication.
- Implement OSPF for dynamic routing.
- Configure DHCP for automated IP address allocation.
- Improve network availability using HSRP and redundant network paths.
- Apply STP to prevent Layer 2 switching loops.
- Strengthen network security using ACLs, Port Security, and DHCP Snooping.
- Explore network monitoring and intrusion detection concepts.
- Validate network functionality through simulation-based testing.

---

## 🏗️ Enterprise Network Architecture

The proposed network follows a **three-layer hierarchical network architecture**, consisting of:

| Network Layer | Main Responsibilities |
|---|---|
| Core Layer | High-speed network connectivity and backbone communication |
| Distribution Layer | Routing, policy enforcement, and network aggregation |
| Access Layer | End-device connectivity and departmental network access |

This hierarchical structure supports modular network management, scalability, fault isolation, and improved network organization.

### Network Topology

The network blueprint represents the proposed enterprise infrastructure, including network devices, departmental segments, interconnections, and the overall network architecture.

![Enterprise Network Blueprint](Network%20Design/INTECH.png)

---

## 🔧 Technologies & Tools

| Category | Technologies / Tools |
|---|---|
| Network Simulation | GNS3 |
| Network Operating System | Cisco IOS |
| Dynamic Routing | OSPF |
| Network Segmentation | VLAN, VTP |
| IP Address Management | DHCP |
| Inter-VLAN Communication | Router-on-a-Stick, Multilayer Switching |
| High Availability | HSRP |
| Switching & Loop Prevention | STP, Rapid PVST+ |
| Network Security | ACLs, Port Security, DHCP Snooping |
| Network Monitoring | Syslog, SNMP Concepts |
| Intrusion Detection | Snort IDS Integration Concept |
| Packet Analysis | Wireshark |
| Configuration & CLI | Solar-PuTTY, Notepad++ |

---

## 🔐 Key Network Features

### 1. Hierarchical Enterprise Network Design

- Designed a structured three-layer enterprise network architecture.
- Organized network infrastructure into core, distribution, and access layers.
- Considered scalability, network availability, and centralized management.
- Planned departmental network segmentation and DMZ-based security zones.

### 2. VLAN Segmentation & Inter-VLAN Routing

- Configured VLANs to logically separate departmental networks.
- Implemented access and trunk port configurations.
- Used VTP for VLAN management and propagation.
- Enabled communication between network segments through inter-VLAN routing.
- Applied network segmentation to improve traffic organization and isolation.

### 3. Dynamic Routing with OSPF

- Configured Open Shortest Path First (OSPF) for dynamic route exchange.
- Established OSPF neighbor relationships between network devices.
- Used dynamic routing to support communication between different network segments.
- Evaluated routing behavior and convergence through simulation-based testing.

### 4. Redundancy & High Availability

- Implemented HSRP for default gateway redundancy.
- Configured redundant network paths to improve availability.
- Used Spanning Tree Protocol (STP) to prevent Layer 2 switching loops.
- Evaluated gateway failover behavior through simulated device and interface failures.

### 5. Network Security & Access Control

- Applied Access Control Lists (ACLs) to control network traffic.
- Configured switch port security to restrict unauthorized device access.
- Incorporated DHCP Snooping as a protection mechanism against unauthorized DHCP activity.
- Considered DMZ-based network isolation for public-facing services.
- Explored intrusion detection concepts for improved security awareness.

### 6. Network Monitoring & Packet Analysis

- Explored SNMP-based network monitoring concepts.
- Used Syslog and interface statistics for network visibility.
- Used Wireshark for packet inspection and protocol analysis.
- Applied command-line diagnostic tools to investigate connectivity and routing behavior.

---

## 🧪 Network Testing & Validation

The implemented network was evaluated using GNS3, command-line utilities, and packet analysis tools.

Testing activities included:

| Test Area | Validation Activities |
|---|---|
| Connectivity Testing | Ping tests between network segments |
| Path Verification | Traceroute testing |
| VLAN Testing | VLAN assignment and inter-VLAN communication |
| STP Testing | Root bridge election and redundant path handling |
| OSPF Testing | Neighbor relationships and route convergence |
| HSRP Testing | Gateway redundancy and failover behavior |
| Security Testing | ACL, Port Security, and DHCP Snooping checks |
| Packet Analysis | Wireshark-based traffic inspection |

### Selected Simulation Results

- **Ping Testing:** Approximately 95% average ping success was reported, with occasional packet loss associated with ARP resolution and routing convergence.
- **Traceroute Testing:** Most tests displayed the expected routing paths, although some intermediate hops were not visible due to ICMP response and filtering behavior.
- **VLAN Testing:** Inter-VLAN communication worked through the configured routing approach after identified trunk and VLAN database inconsistencies were corrected.
- **STP Testing:** Redundant paths were managed to prevent switching loops. Initial convergence delays were observed and improvements were made using PortFast and Rapid PVST+.
- **OSPF Testing:** OSPF neighbor adjacencies and route exchange operated successfully, with minor convergence delays observed after simulated interface or router changes.
- **HSRP Testing:** The standby router successfully assumed the active role within approximately 5–10 seconds during the tested failure scenario.

These results reflect the behavior observed within the simulated project environment and do not represent measurements from a live production deployment.

---

## 💡 Project Outcomes

The project provided practical experience in planning, designing, configuring, and evaluating a resilient enterprise network infrastructure.

Key outcomes included:

- A structured hierarchical enterprise network architecture.
- VLAN-based departmental network segmentation.
- Inter-VLAN communication and dynamic routing using OSPF.
- DHCP-based IP address allocation.
- Gateway redundancy through HSRP.
- Loop prevention through STP.
- Network access control using ACLs and switch security configurations.
- Simulation-based connectivity, routing, and failover testing.
- Practical experience in network troubleshooting and packet analysis.

---

## ⚠️ Project Limitations

- The project was implemented in a virtualized simulation environment; physical network deployment was not included.
- GNS3 resource requirements can affect the performance of larger network topologies.
- Integration of third-party security and monitoring appliances may introduce compatibility or stability limitations.
- Advanced monitoring and intrusion detection capabilities are subject to the limitations of the simulated environment.
- Long-term production network maintenance and operational management were outside the project scope.
- Real-world traffic loads and physical hardware performance were not fully represented by the simulation.

---

## 🔒 Copyright & Usage Policy

### © 2026 Yesmin Jalaldeen. All Rights Reserved.

This repository showcases an individual academic project developed by the author.

The original project materials, including network architecture designs, topology diagrams, documentation, configurations, and project-specific implementation work, are protected by the author's stated copyright and usage policy, subject to applicable third-party and institutional rights.

**No permission is granted to copy, reproduce, modify, redistribute, republish, or submit the author's original project materials as another person's academic or professional work without prior written permission.**

This policy applies to the author's original contributions, including:

- Network topology diagrams and architecture designs.
- Original network configurations and implementation materials.
- Project documentation and reports.
- Original project-specific technical content.

Public access to this repository does not, by itself, grant permission to reuse the author's original work.

### 📩 Permission Requests

Anyone wishing to reuse or redistribute protected original materials must obtain prior written permission from the author.

---

<div align="center">

### ✍️ Yesmin Jalaldeen

*Project Author & Network Designer*

**BIT (Hons) Specialized in Computer Networks**  
**BCS HEQ PGD in Computer Networks**

*“Building Resilient Networks Through Structured Design and Practical Simulation.”*

**© 2026 Yesmin Jalaldeen — All Rights Reserved.**

</div>
