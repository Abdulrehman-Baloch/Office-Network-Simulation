# Corporate Office Network Simulation

## Project Overview
This project simulates a corporate office network for a multi-department organization using Cisco Packet Tracer. The network is designed to connect multiple departments (Sales, IT, and HR) while ensuring secure and efficient communication.

## Features Implemented
- **Network Segmentation**: Three subnets for Sales, IT, and HR to improve security and traffic management.
- **DHCP Implementation**: A dedicated DHCP server dynamically assigns IP addresses to devices in each subnet.
- **Routing Configuration**: RIP v2 is used for dynamic routing to enable communication between departments.
- **Internet Access via NAT**: Network Address Translation (NAT) is configured on the main router to allow internet access for internal devices.
- **Scalability**: The network is designed for future expansion, making it easy to add new departments or devices.

## Technologies Used
- **Software**: Cisco Packet Tracer
- **Protocols**:
  - **Routing**: RIP v2
  - **Addressing**: DHCP
  - **NAT**: Dynamic NAT for internet access

## Network Design
- **IP Addressing Scheme** (Class C: 192.168.1.0/24)
  - Sales Department: `192.168.1.0/26`
  - IT Department: `192.168.1.64/26`
  - HR Department: `192.168.1.128/26`
  - Server Room: `192.168.1.192/29`
  - Router Subnets: `192.168.1.200/29`, `192.168.1.208/29`, `192.168.1.216/29`

## Implementation Details
1. **Subnetting**: The network is divided into smaller subnets to optimize performance and security.
2. **Routing**: RIP v2 is configured on routers to dynamically manage route advertisements.
3. **NAT Configuration**: The main router translates private IPs to public IPs for internet access.
4. **DHCP Setup**: A dedicated DHCP server provides IP addresses for client devices.
5. **Device Connectivity**: PCs, routers, and switches are configured to ensure smooth communication between departments.

## Testing & Results
- **DHCP**: Verified automatic IP assignment to devices.
- **Routing**: Ensured inter-departmental communication via RIP v2.
- **NAT**: Successfully provided internet access to internal users.

## Challenges & Learnings
### Challenges:
- Configuring NAT with access lists for secure internet access.
- Managing dynamic routing with proper route advertisements.
- Ensuring seamless DHCP relay across subnets.

### Learnings:
- Gained hands-on experience with RIP v2, NAT, and DHCP configurations.
- Improved troubleshooting skills in network simulation environments.
- Enhanced understanding of corporate network design and security.

## Future Enhancements
- Implement **OSPF or EIGRP** for better scalability.
- Introduce **VLANs** to optimize network segmentation.
- Enhance security with **firewalls and VPNs**.

## How to Use the Project
1. Open the **Packet Tracer (.pkt) file** in Cisco Packet Tracer.
2. Review the network topology and configurations.
3. Use CLI commands to verify routing, DHCP, and NAT functionality.
4. Perform connectivity tests using the `ping` command.

## Author
**M. Abdulrehman**  
Student ID: 22I-1182  
Course: Computer Networks  
FAST, Islamabad  

## License
This project is open-source and available for educational purposes.

