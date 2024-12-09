# Network Design Project: Multi-Office Company Network

## Overview
This project involves designing and configuring a network for a company with three offices: Headquarters (HQ), Branch Office 1, and Branch Office 2. The network ensures efficient communication between offices, secure VLAN segmentation, inter-VLAN communication, and dynamic routing for optimal traffic flow.

## Scenario
- **Headquarters (HQ)**: Located in City A.
- **Branch Office 1**: Located in City B.
- **Branch Office 2**: Located in City C.

Each office contains:
- Layer 2 Switches for VLAN segmentation.
- Layer 3 Switches for routing within VLANs.
- Routers for inter-office communication.
- PCs as end-user devices.

## Key Features

### 1. VLAN Segmentation
The following VLANs were created for improved segmentation:
- **VLAN 10**: Management (switches and routers)
- **VLAN 20**: Sales
- **VLAN 30**: Marketing
- **VLAN 40**: IT
- **VLAN 50**: Guest (visitors)

### 2. Trunking
- Trunk links between switches and routers were configured to carry multiple VLANs using **802.1Q encapsulation**.

### 3. Routing
#### Static Routing (HQ to Branch Office 1):
- Static routes were set up to ensure proper routing between VLANs and default gateways.

#### Dynamic Routing (HQ to Branch Office 2, Branch Office 2 to Branch Office 1):
- OSPF was configured for dynamic routing to optimize traffic flow.

### 4. Inter-VLAN Communication
Different methods were implemented to enable communication between VLANs:
- **Router on a Stick**: Configured for HQ and Branch Office 1.
- **Separated Interfaces**: Configured for Branch Office 2.
- **Layer 3 Switch Routing**: Configured for inter-VLAN routing within offices.

### 5. Security
- Disabled unused ports on switches.
- Implemented port security to limit the number of MAC addresses per port.
- Configured strong passwords for device access.

### 6. Documentation
- A detailed network diagram shows device placement, VLANs, and routing configurations.
- All device configurations are documented, including interfaces, IP addresses, and OSPF settings.

## File Structure
- `Network_Project_Efrat_Ilouz.pkt`: Packet Tracer project file for the network.
![Screenshot 2024-12-09 185534](https://github.com/user-attachments/assets/d51c7162-8874-4f39-87b4-564ba6077065)
![image](https://github.com/user-attachments/assets/60c06f5d-48c5-4ff0-8b84-a0ad8a84c77e)
![image](https://github.com/user-attachments/assets/baa78c86-2b75-45a4-b849-1104928293da)

## How to Use
1. Open the `.pkt` file in Cisco Packet Tracer.
2. Explore the network topology and configurations.
3. Test connectivity by pinging between devices in different VLANs and offices.

## Future Enhancements
- Implement advanced security measures such as access control lists (ACLs).
- Set up backup routes for high availability.

---

![image](https://github.com/user-attachments/assets/f16fd422-c5ed-4df8-a80a-ca4b30e313b1)
![image](https://github.com/user-attachments/assets/8385a50a-cf3b-404a-9c70-6eef510bf15e)
![image](https://github.com/user-attachments/assets/662755d5-4238-4988-8155-ce05450d92cd)
![image](https://github.com/user-attachments/assets/cd04000c-1851-4b39-8cf5-37e4e76347d0)


