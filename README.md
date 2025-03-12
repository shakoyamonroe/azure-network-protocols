<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

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

<img width="649" alt="Screenshot 2025-03-12 at 12 53 35 PM" src="https://github.com/user-attachments/assets/6f26bdb9-37ee-4c2f-bc20-c420810cc9b8" />

<img width="639" alt="Screenshot 2025-03-12 at 12 54 30 PM" src="https://github.com/user-attachments/assets/dcd1a968-40b6-4d90-8622-32f573dc9a47" />


### 2️⃣ Set Up Network Security Groups (NSGs)
- Configure **NSGs** to control inbound and outbound traffic.
- Allow and block traffic for specific ports (e.g., **SSH, RDP, HTTP/S**).

### 3️⃣ Inspect Network Traffic with Wireshark
- Install **Wireshark** on the Windows VM.
- Capture traffic while initiating connections between the VMs.
- Observe packet details for different protocols (DNS lookups, HTTP requests, etc.).

<img width="742" alt="Screenshot 2025-03-12 at 12 58 03 PM" src="https://github.com/user-attachments/assets/f1e0afd8-65ac-485c-890b-69d5c0aa9046" />

<img width="728" alt="Screenshot 2025-03-12 at 1 02 57 PM" src="https://github.com/user-attachments/assets/fde3906d-c4c8-42d0-964f-6ec0ed7a9a4c" />

<img width="1010" alt="Screenshot 2025-03-12 at 1 07 03 PM" src="https://github.com/user-attachments/assets/1af2c2c0-d64c-42fa-88b4-7ad131703218" />

<img width="837" alt="Screenshot 2025-03-12 at 1 08 32 PM" src="https://github.com/user-attachments/assets/51b33487-5f02-44a6-862c-57bbc77bc814" />


### 4️⃣ Analyze and Adjust Firewall Rules

- Modify **NSG rules** to observe changes in network behavior.
- Block/allow specific traffic and analyze its impact in **Wireshark**.
- Ensure security policies align with organizational requirements.
  
<img width="851" alt="Screenshot 2025-03-12 at 1 11 16 PM" src="https://github.com/user-attachments/assets/1f569b18-97eb-454a-b7a6-5afd2ce1a74a" />

<img width="521" alt="Screenshot 2025-03-12 at 1 12 46 PM" src="https://github.com/user-attachments/assets/99735303-84e7-41f4-ba6a-da0d17fd08bb" />

<img width="865" alt="Screenshot 2025-03-12 at 1 14 20 PM" src="https://github.com/user-attachments/assets/44771031-c8ac-4260-91df-f1b7ed020c07" />

<img width="98" alt="Screenshot 2025-03-12 at 1 15 50 PM" src="https://github.com/user-attachments/assets/09db141b-8c4a-4d33-96e5-309788fa3217" />


