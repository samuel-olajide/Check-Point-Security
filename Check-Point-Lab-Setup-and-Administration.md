# Part A 1: Prepare VMware and the private network

## Step 1: Install the Windows tool
### A1 
**VMware Workstation**
  - <img width="650" height="499" alt="image" src="https://github.com/user-attachments/assets/a2824b64-d170-466a-9ec6-5ab331c9e26b" />
  - Source: I already had the software installed before the program
R82 SmartConsole desktop
  - <img width="688" height="327" alt="image" src="https://github.com/user-attachments/assets/de51d227-c2f1-425b-bf2a-bd2993e07771" />
  - Source: I used the link provided by the instructor

## Step 2: Load "A SMS" and check its adapter
### A2
<img width="1365" height="666" alt="image" src="https://github.com/user-attachments/assets/f5d87de4-74a0-4931-bd7e-bb80160e5dd0" />
<img width="815" height="679" alt="image" src="https://github.com/user-attachments/assets/b0041cc6-bfa4-4e7f-93cf-40856c893f80" />

## Step 3: Set the VMnet8 network
### A3
<img width="491" height="523" alt="image" src="https://github.com/user-attachments/assets/7d87fef5-b97e-4765-acf6-a34dab99d909" />
<img width="390" height="288" alt="image" src="https://github.com/user-attachments/assets/6ca99260-8ead-48b9-94e8-0b76525fee13" />

# Part A 2: Set the addresses and verify Gaia

## Step 4: Set the Windows VMnet8 address
### A4 
<img width="584" height="126" alt="image" src="https://github.com/user-attachments/assets/58308183-ca9a-462d-9ca8-4541718cd937" />

## Step 5: Boot "A SMS" and inspect eth0
### A5
<img width="845" height="389" alt="image" src="https://github.com/user-attachments/assets/ad66df59-ef5f-4538-aeb0-e1296a4c75cb" />

## Step 6: Check access from Windows
### A6
<img width="539" height="247" alt="image" src="https://github.com/user-attachments/assets/6bc95428-c699-4c0e-8060-ea5c03b1694a" />
<img width="1365" height="703" alt="image" src="https://github.com/user-attachments/assets/03526226-5171-46b8-86fc-8770acd259d2" />

# Part A 3: Connect SmartConsole

## Step 7: Verify the server and sign in
### A6 
**Gaia Portal:** <img width="1365" height="610" alt="image" src="https://github.com/user-attachments/assets/89d39f25-3fa9-4b8c-81dc-ad617b4ce5d2" />
**Smart Console:** <img width="1045" height="469" alt="image" src="https://github.com/user-attachments/assets/3260da21-5dae-4979-8c9d-1a4c92781977" />
**Fingerprint Check:** The ICA fingerprint displayed in Smart Console matches the one on the "A SMS" terminal. 

# Part B: Explain the Check Point architecture

## B1: Explain the architecture
Check Point uses a three-tier architecture consisting of SmartConsole, the Security Management Server, and the Security Gateway.
1. SmartConsole (Windows): Used by administrators to create and manage security policies.
2. Security Management Server: The Security Management Server stores policies and network objects.
3. Security Gateway: The Security Gateway protects the network by enforcing policies.

## B2: Explain management services and deployment
The Security Management Server performs several functions:
  1. Database: Stores security policies, objects, and configurations.
  2. Log Server: Collects and stores security logs from gateways.
  3. Monitoring: Displays CPU, memory, disk usage, and traffic statistics.

## B3: Choose the correct administration interface

## B4: Explain security features and policy handling
1. Firewall: Controls network traffic based on security rules. For example, it can block unauthorised access to an organisation's internal network.
2. URL Filtering: Controls access to websites based on categories. For example, it can block malicious or inappropriate websites.
Publishing and installing policies are separate actions because publishing saves changes to the management database and makes them available to other administrators, while policy installation distributes the published policy to the Security Gateway, where it becomes active and is enforced.

## B5: Interpret your own lab evidence
1. VMnet8 uses a private virtual network, so its IP addresses can remain unchanged even when the computer switches Wi-Fi networks.
2. VMware DHCP does not change the A-SMS address because its network interface is configured with a static IP address.
3. A successful ping confirms basic network reachability through ICMP, but it does not confirm that SmartConsole can connect. A successful SmartConsole login confirms that the management service is accessible and the credentials are accepted.
4. An unavailable gateway object or empty log view does not automatically indicate a fault. Further checks are necessary because the object may be missing or incorrectly configured, while logs may be absent due to filters, logging settings, or lack of traffic.

# Part C: Explore Gaia Portal
## C1: Inspect the system overview
### G1
<img width="1365" height="605" alt="image" src="https://github.com/user-attachments/assets/e409081b-f6d9-431d-8c82-2ef2d078d38e" />


## C2: Compare the navigation modes
### G2
- **DHCP Server:** This can be used to assign IP addresses automatically to devices that are connected to the server. This option can only be found in the Advanced view mode on the GAIA server web portal.
- **System logging:** This can be found in the Advanced view mode on the GAIA web portal. It sends log entries to a remote syslog server.
- 
**Basic View:** <img width="1365" height="608" alt="image" src="https://github.com/user-attachments/assets/81437b93-39e6-4450-b78d-6257e40247e8" />
**Advance View:** <img width="1362" height="606" alt="image" src="https://github.com/user-attachments/assets/718f393d-dc68-48c4-9378-ec0d9803e4e1" />

## C3: Inspect the management interface
### G3
<img width="1039" height="54" alt="image" src="https://github.com/user-attachments/assets/9119fbe0-06d0-46f2-891c-260e735402b0" />
<img width="456" height="344" alt="image" src="https://github.com/user-attachments/assets/4350979f-8dab-4bd4-9423-7a5ded5c5dd3" />

## C4: Inspect routes and DNS
### G4

## C5: Locate maintenance and administration functions
### G5

