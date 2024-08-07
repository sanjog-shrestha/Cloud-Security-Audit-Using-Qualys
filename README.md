# Cloud Security Audit Using Qualys

## Objective

The objective of this project was to conduct a comprehensive cloud security audit of a Windows 10 virtual machine (VM) running on VMware. The goal was to leverage the Qualys cloud-based security platform to identify vulnerabilities and assess the effectiveness of the security controls in place. The ultimate aim was to use the insights gained from the vulnerability testing to harden the VM and improve its overall security posture. By gaining hands-on experience with Qualys and its capabilities, the project allowed for the development of essential skills in cloud security assessment and hardening, which can be applied to future endeavors in this domain.

### Skills Learned

-  Virtual machine setup and configuration
-  Cloud-based security platform usage (Qualys)
-  Vulnerability identification and assessment
-  Security control evaluation
-  Remediation and hardening
-  Continuous monitoring and improvement


### Tools Used

- VMware:<br>
  Used to set up and manage the Windows 10 virtual machine.
- Qualys:<br>
  A cloud-based security platform used to conduct the vulnerability testing and assessment.
  Qualys Virtual Scanner was used to scan the Windows 10 VM.
  Qualys Vulnerability Management module was used to configure the scan options and analyze the results.
- Windows 10:<br>
  The target operating system running on the virtual machine that was subjected to the security audit.
- IP Address Management:<br>
  The IP addresses of the Qualys Virtual Scanner (192.168.1.168) and the Windows 10 VM (192.168.1.141) were configured to be on the same network for the scan to be conducted.
- Option Profiles:<br>
  A security profile, named "Basic Net Scan," was created in Qualys to define the configuration for the vulnerability scan.
- Authentication:<br>
  Credentials for the Windows 10 VM were provided to Qualys to enable authenticated vulnerability scanning.

## Steps

| Devics                                        | IP Address                 |
|-----------------------------------------------|----------------------------|
| Qualys Virtual Scanner                        | 192.168.1.168              |
| Windows 10                                    | 192.168.1.141              |

Ref 1: IP Address on the project

![image](https://github.com/user-attachments/assets/974a3a12-fead-41e0-bc72-5ba3beb39bda)

Ref 2: Address Management

The role of IP address management in this project was crucial for enabling the Qualys cloud-based security platform to successfully connect to and scan the Windows 10 virtual machine. Configuring the IP addresses of the Qualys Virtual Scanner and the Windows 10 VM to be on the same network subnet allowed for the necessary connectivity and access required to perform the authenticated vulnerability assessment. Proper IP address management was a key factor in ensuring the security audit could be conducted effectively.

![image](https://github.com/user-attachments/assets/d7b676c8-209f-4865-a84f-7a0b999edb78)
![image](https://github.com/user-attachments/assets/f7f83a86-fb70-4083-98b1-0f27bdd8cd1a)

Ref 3: Authentication

The role of authentication in this project was to enable Qualys to perform a more thorough, agent-based vulnerability scan of the Windows 10 virtual machine. By providing the credentials for the Windows 10 VM to Qualys, the security platform was able to access the system directly and conduct a deeper, authenticated scan. This allowed for the identification of a more comprehensive set of vulnerabilities that could be addressed to improve the overall security posture of the VM.

![image](https://github.com/user-attachments/assets/185c91e8-ff71-4037-aa80-b9b590071169)
![image](https://github.com/user-attachments/assets/dc63b8e7-85cb-475e-95c5-477233025e60)
![image](https://github.com/user-attachments/assets/572bbf64-12e1-44a6-b691-1f0895e2d5f6)

Ref 4: Scan Results

The scan results from the Qualys vulnerability assessment played a crucial role in this project. The identified vulnerabilities and security issues provided the necessary insights to determine the appropriate remediation and hardening steps required to improve the security posture of the Windows 10 virtual machine. These scan results served as the foundation for the security enhancement process, guiding the team in prioritizing and addressing the most critical vulnerabilities to strengthen the overall security controls and configuration of the VM.




