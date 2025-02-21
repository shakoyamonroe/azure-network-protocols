<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups]
- https://youtu.be/Mu_2UnOdVHM?si=s2FpRS4c_3tgaiKu
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

1. **Deploy Azure Virtual Machines**
2. **Set Up Network Security Groups (NSGs)**
3. **Inspect Network Traffic with Wireshark**
4. **Analyze and Adjust Firewall Rules**

## ⚙️ Actions and Observations

### 1️⃣ Deploy Azure Virtual Machines
- Create a **Windows 10 VM** and an **Ubuntu Server VM** in Azure.
- Ensure both machines are in the same virtual network for traffic inspection.

### 2️⃣ Set Up Network Security Groups (NSGs)
- Configure **NSGs** to control inbound and outbound traffic.
- Allow and block traffic for specific ports (e.g., **SSH, RDP, HTTP/S**).

### 3️⃣ Inspect Network Traffic with Wireshark
- Install **Wireshark** on the Windows VM.
- Capture traffic while initiating connections between the VMs.
- Observe packet details for different protocols (DNS lookups, HTTP requests, etc.).

### 4️⃣ Analyze and Adjust Firewall Rules
- Modify **NSG rules** to observe changes in network behavior.
- Block/allow specific traffic and analyze its impact in **Wireshark**.
- Ensure security policies align with organizational requirements.
