# Cloud Security Audit Using Qualys

## Objective

The objective of this project is to establish and secure a controlled home network environment using virtualization technology. By creating a lab consisting of multiple virtual machines, this project aims to demonstrate network segmentation, firewall configuration, and the deployment of an Intrusion Detection System (IDS). The goal is to simulate real-world network scenarios, enforce security policies, and showcase the ability to detect and respond to potential security threats. Through this project, the intended outcomes are to gain hands-on experience with virtualization software, network segmentation, firewall configuration, and IDS systems, ultimately enhancing the understanding and application of network security best practices.

### Skills Learned

-  Virtualization using VMware
-  Network segmentation
-  Firewall configuration (PfSense)
-  IDS/IPS deployment and configuration (Snort on PfSense)
-  Network traffic monitoring and analysis
-  Basic network security best practices
-  Hands-on experience with Windows XP, Ubuntu 24.04, Debian 12.0.0, and PfSense


### Tools Used

Virtualization:
- VMware Workstation Pro

Operating Systems:
- Windows XP (Virtual Machine)
- Ubuntu 24.04 (Virtual Machine)
- Debian 12.0.0 (Virtual Machine)
- PfSense (Virtual Machine)

Firewall:
- PfSense (Firewall and Router)

Intrusion Detection System (IDS):
- Snort (IDS)

Networking:
- Wireshark (Network traffic analysis)
- ping (Network connectivity test)


## Steps
![image](https://github.com/user-attachments/assets/d9f89e7c-cf67-41b0-bb94-b1339bc768d0)

Ref 1: Network Diagram

![image](https://github.com/user-attachments/assets/922a8d41-a961-4fb7-af93-9d775d7dfb6a)

Ref 2: Use of aliases in pfsense

It is used in PfSense to group IP addresses for easier management and reference in firewall rules. It is created for gateway IP addresses (192.168.199.1 and 192.168.94.1) to simplify rule creation and maintenance which allowed for more readable and organized firewall rules by replacing IP addresses with descriptive names (e.g., "Gateway").

![image](https://github.com/user-attachments/assets/d8edf45d-26ae-45af-821d-e833a9440466)
![image](https://github.com/user-attachments/assets/cf3d504a-5d09-4b8a-9ceb-087254e168e1)

Ref 3: Firewall Rules

The LAN rules in this project play a crucial role in controlling and securing the network traffic within one of the network segments. Specifically:
The first LAN rule allows all devices in that network segment to access the gateway IP address. This ensures that devices on the LAN can connect to the other network segment through the gateway.
The second LAN rule explicitly allows a specific device (or group of devices) to access any device on the network. This is likely done to grant certain devices the necessary access to communicate with other devices.
The third LAN rule explicitly denies any other devices in that network segment from connecting to devices outside of that segment. This rule enforces the network segmentation by restricting access between the two network segments, except for the specific access granted in the previous rules.
These LAN rules, in combination with the rules for the other network segment, demonstrate a well-thought-out network segmentation strategy. This strategy controls and limits the communication between the different network segments, enhancing the overall security of the home network setup.

![image](https://github.com/user-attachments/assets/2f4410e0-adf8-407b-8c5e-e6144cd1c2c9)
![image](https://github.com/user-attachments/assets/d139d1f1-5226-46be-b899-cb875ecc4f21)
![image](https://github.com/user-attachments/assets/1bd8b6af-d1dd-4a0b-8281-3d89f126d9ca)

Ref 4: Proof of Evidence

![image](https://github.com/user-attachments/assets/d11ffbfc-cd1d-4ac6-bcf7-d91e4a31bba2)
![image](https://github.com/user-attachments/assets/947fe078-b023-45be-a636-f956379349ef)
![image](https://github.com/user-attachments/assets/745c8195-7cdb-4472-8b7a-9632cceb6fe2)

Ref 5: Snort Configuration

In this project, Snort was configured as an Intrusion Detection System (IDS) to monitor and analyze the network traffic within the 192.168.199.0/24 network segment. Snort was deployed on the Pfsense firewall and was set to operate in IDS mode, rather than IPS (Intrusion Prevention System) mode, which means it was tasked with detecting and logging potential security threats, but not automatically blocking them.

The purpose of including Snort in this home network security setup was to provide an additional layer of security by detecting and alerting on any suspicious or malicious network activity. By analyzing the network traffic against a set of predefined rules, Snort was able to identify potential intrusion attempts and generate alerts, allowing the network administrator to further investigate and respond to any security incidents.

The successful deployment and testing of Snort in this project demonstrated the value of incorporating an IDS system as part of a comprehensive network security strategy, even in a home network environment. The ability to monitor and detect potential threats in real-time can greatly enhance the overall security posture and help the network administrator take appropriate actions to mitigate any identified risks.





