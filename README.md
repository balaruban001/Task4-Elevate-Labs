#  Task 4: Setup and Use a Firewall on Windows

## Objective
Configure and test basic firewall rules using **Windows Defender Firewall** to allow or block specific network traffic.

---

## 🛠 Tools Used
- **Operating System**: Windows 10/11  
- **Firewall**: Windows Defender Firewall with Advanced Security  
- **Command Prompt**  
- **Telnet Client** (Optional Windows Feature)

---

##  Steps Performed

### 1. Open Firewall Configuration Tool
- Launched using `wf.msc` from the Run dialog (`Win + R`).
- Accessed the **Inbound Rules** section.

### 2. List Current Firewall Rules
- Reviewed existing **Inbound Rules** to understand current traffic policies.

### 3. Block Inbound Traffic on Port 23 (Telnet)
- Created a new **Inbound Rule**:
  - **Type**: Port
  - **Protocol**: TCP
  - **Port**: 23
  - **Action**: Block the connection
  - **Name**: `Block Telnet Port 23`

### 4. Test the Rule
- Ran:
  ```bash
  telnet localhost 23
