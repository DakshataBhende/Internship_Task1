# Task 1 
This repository contains all the submission material regarding task 1 for the internship.

## Task: Scan Your Local Network for Open Ports
- Objective: Learn to discover open ports on devices in your local network to understand network exposure.
- Tools: Nmap (free), Wireshark (optional)

## Steps:  
1. I was working on **Windows**, so I installed Nmap from the official website: [](https://nmap.org/download.html). It comes with both the command-line tool and the Zenmap GUI.
2. I opened **Command Prompt** and ran `ipconfig` to list the IP address for my local network.
   - It listed the IP ranges including the IPv4 address, which I used to determine my subnet (e.g., `192.168.0.0/24`).
![Screenshot 2025-06-23 173754](https://github.com/user-attachments/assets/1674b7d7-4a70-46b8-afe3-5596b5cd96a2)
3. I ran the help command to view the available options in Nmap: `nmap -h`.
4. I selected useful options based on the context:
   - `-sS` for stealth SYN scan
   - `-Pn` to skip host discovery (in case ping is blocked)
   - `-p-` to scan all 65535 ports
   - `-oN` to save the result into a normal text file
![Screenshot 2025-06-23 174457](https://github.com/user-attachments/assets/d50f6693-1196-48bb-8f66-533f269b9c29)
5. Reviewing the Scan Results: Once the scan completed, I analyzed the output file (scan_results.txt).
6. Assessing Security Risks: I researched the common vulnerabilities associated with the open ports discovered during the scan. That can be found in Risk_Assessed file.

### Outcome: 
By completing this task, I gained practical experience with port scanning techniques and tools. I now understand how to:
- Identify devices on a local network.
- Enumerate open ports and the services running on them.
- Recognize how misconfigured or exposed services can present security risks.
  
## Conclusion:
This exercise offered hands-on exposure to one of the most fundamental concepts in cybersecurity — network reconnaissance. Using Nmap, I was able to effectively map my local network, identify service exposures, and assess potential weak points.
