#  Cybersecurity Internship – Task 4
###  Configure & Test Windows Firewall Rules


## Objective
Set up and test a firewall rule to block **inbound traffic on TCP port 23 (Telnet)** using **Windows Defender Firewall**, verify its effectiveness, and then remove the rule to restore the original firewall state.


## Steps Performed

### 1. Opened Windows Defender Firewall (Advanced Settings)
- Accessed the **Firewall with Advanced Security** tool from Windows.

### 2. Created a New Inbound Rule
- Configured a rule to:
  - **Block TCP port 23 (Telnet)**
  - Rule name: **“Block Telnet Port 23”**
- Applied to:
  - **Domain**, **Private**, and **Public** profiles.

### 3. Verified the Rule
- Attempted to initiate a **Telnet connection** to verify the block was working.
- The connection was successfully **blocked**, confirming the rule was active.

### 4. Removed the Rule (Restored State)
- Deleted the test firewall rule to return the firewall to its original configuration.


## Screenshots

|    |   Description                   | Image                                             |
|----|---------------------------------|------------------------------------------------------|
| 1  | Inbound Rules – Overview        | ![Inbound Overview](screenshots/firewall-overview-inbound.png) |
| 2  | Outbound Rules – Overview       | ![Outbound Overview](screenshots/firewall-overview-outbound.png) |
| 3  | Block Rule for Port 23 Created  | ![Rule Created](screenshots/rule-created.png)        |
| 4  | Rule Deleted After Testing      | ![Rule Deleted](screenshots/rule-deleted.png)        |



## Summary of Learning
-  Learned how to configure **inbound firewall rules** in Windows.
-  Understood how firewalls filter traffic based on **IP, port, and protocol**.
-  Practiced blocking a high-risk service (**Telnet on port 23**) to prevent unencrypted remote access attempts.
-  Restored the original firewall state after testing, demonstrating good firewall management practices.



## Why Block Telnet (Port 23)?
- Telnet transmits data in **plain text**, including usernames and passwords.
- Blocking Telnet reduces risk by preventing insecure remote access.
- Modern systems prefer secure alternatives like **SSH (Port 22)**.


## Key Concepts Practiced
- Firewall configuration (Inbound/Outbound rules)
- Port-based traffic filtering
- Network security hardening
- Windows Defender Firewall management
