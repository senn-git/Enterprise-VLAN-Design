# Enterprise VLAN Design

## Project Overview
Enterprise VLAN Design demonstrates the implementation of Virtual Local Area Network (VLAN) segmentation in a multi-department office environment using a Cisco 2960 switch in Cisco Packet Tracer.

The network is logically divided into three departments — HR, IT, and Finance — to enhance security, control broadcast traffic, and improve overall network management.

---

## Tools & Technologies
- Cisco Packet Tracer
- Cisco 2960 Switch
- End Devices (PCs)
- VLAN Configuration
- Switch Port Management

---

## Network Design

| Department | VLAN Name | VLAN ID | Ports Assigned | No. of PCs |
|-----------|------------|---------|----------------|------------|
| HR        | VLAN A     | 5       | Fa0/1 – Fa0/5  | 2 PCs      |
| IT        | VLAN B     | 10      | Fa0/6 – Fa0/10 | 5 PCs      |
| Finance   | VLAN C     | 15      | Fa0/11 – Fa0/15| 3 PCs      |

---

## Configuration Summary

- Created VLANs on the Cisco 2960 switch:
  - **VLAN 5 → HR Department**
  - **VLAN 10 → IT Department**
  - **VLAN 15 → Finance Department**

- Assigned VLAN names:
  - VLAN 5 → A  
  - VLAN 10 → B  
  - VLAN 15 → C  

- Configured and mapped switch ports to their respective VLANs  
- Ensured proper departmental segmentation through VLAN isolation  

---

## Communication Testing

Message transfer tests were performed to verify VLAN isolation:

- **PC0 → PC1 (Same Department – IT):** Successful  
- **PC2 → PC0 (Different Departments):** Failed  
- **PC6 → PC9 (Different Departments):** Failed  
- **PC2 → PC6 (same Department - Finance):** Successful  

These results confirm that communication is allowed only within the same VLAN, while inter-VLAN communication is restricted due to the absence of inter-VLAN routing.

---

## Project Objectives

- Implement enterprise-level network segmentation  
- Improve security between departments  
- Reduce broadcast domains  
- Understand VLAN creation and port assignment  
- Gain hands-on experience with switch configuration  

---

## Screenshots Included

- Network topology showing VLAN segmentation  
- VLAN creation on switch CLI  
- Port-to-VLAN assignment configuration  
- Message transfer test results  

---

## Files Included

- `.pkt` file containing the complete VLAN network setup  
- Configuration and testing screenshots  

---

## Learning Outcomes

- Practical understanding of VLAN segmentation  
- Experience configuring VLANs on Cisco switches  
- Knowledge of broadcast domain isolation  
- Improved enterprise network design fundamentals  

---

## Future Enhancements

- Configure Inter-VLAN Routing using a router or Layer 3 switch  
- Implement VLAN trunking between multiple switches  
- Apply ACLs for department-level access control  
- Integrate DHCP for dynamic IP allocation  
