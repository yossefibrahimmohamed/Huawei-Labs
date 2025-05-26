🔧 Network Simulation Projects (eNSP)

This repository contains two comprehensive network simulation projects created using Huawei’s eNSP (Enterprise Network Simulation Platform). The projects simulate realistic enterprise-level network environments for training, testing, and educational purposes.

📁 Project 1: Full Project (Multi-Vendor Simulation)


![1746412327772](https://github.com/user-attachments/assets/c2dea2e8-bac8-4d25-a6e2-9ce762b8acd4)


🖼️ Network Topology

📄 Overview

This project simulates a multi-vendor enterprise network incorporating Huawei, Cisco, and IBM network domains. Each domain features its own internal subnet, security policies, and routing configurations, demonstrating interoperability and prioritization techniques between different vendor systems.
🧱 Components

    Huawei Zone (Red)

        Network: 10.1.0.0/24

        NAT & Firewall Policies

        Priority: Medium

        Includes static routing and service manager

    Cisco Zone (Green)

        Network: 19.2.0.0/24

        High-priority routing

        Centralized routing core

    IBM Zone (Brown)

        Network: 13.0.0.0/24

        Low-priority traffic

        Zone-based routing

🌐 Connectivity

    Each vendor connects via a common router to a public cloud (200.10.10.0/24) simulating internet access.

    Priorities are managed using policy-based routing and Quality of Service (QoS).

📁 Project 2: Final Project (Firewall and DMZ Design)


![1747281846606](https://github.com/user-attachments/assets/67811d8f-e35b-4eaf-8d6e-83eb96a8d362)



🖼️ Network Topology

📄 Overview

This project simulates a redundant firewall architecture with an active-standby firewall setup, a DMZ (Demilitarized Zone), and various trust zones. It emphasizes security zone isolation, policy management, and availability.
🧱 Components

    Active and Standby Firewalls

        Dual-firewall design for high availability

        Monitored failover system

    DMZ Zone

        Hosts publicly accessible services (10.1.10.0/24)

    Trust / Untrust Zones

        Untrust Zone: Public IP 1.1.1.1 (1.1.1.0/24)

        Trust Zone: Internal LANs and services

    Service Policies

        Includes policies for VPN, email, web, and NAT

🔐 Security Features

    Multi-zone configuration:

        Trust ↔ Untrust ↔ DMZ

    Stateful inspection and NAT

    VPN and security policy enforcement per zone

✅ Skills Demonstrated

    Multi-vendor network simulation

    Security zone design and implementation

    NAT, routing (static and dynamic), and firewall policy management

    High availability and failover configuration

    Network segmentation and prioritization

📦 Tools Used

    eNSP (Enterprise Network Simulation Platform)

    Virtual Routers and Switches (Huawei & Cisco)

    Firewall Simulation and Zone Configuration

🔧 How to Use

    Place the image files (full_project.jpeg, final_project.jpeg) in a folder called images/ in the root of your project.

    Open the .esnp project files in eNSP.

    Power on all devices.

    Verify connectivity with ping and tracert.

    Inspect routing tables, NAT rules, and firewall policies for validation.
