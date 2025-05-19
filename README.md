<p align="center">
  <a href="https://github.com/Samuel-Cavada" target="_blank">
    <img src="https://img.shields.io/badge/Back_to_Main_Page-000000?style=for-the-badge&logo=github&logoColor=white" alt="Back to Main Page"/>
  </a>
</p>

<h1 align="center">Linux VM Agent-Based Vulnerability Scanning with Tenable</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Local%20VM-0078D4?style=for-the-badge&logo=linux&logoColor=white" alt="Platform" />
  <img src="https://img.shields.io/badge/OS-Linux-0078D6?style=for-the-badge&logo=linux&logoColor=white" alt="OS" />
  <img src="https://img.shields.io/badge/Tool-Tenable.io-00B388?style=for-the-badge&logo=tenable&logoColor=white" alt="Tool" />
  <img src="https://img.shields.io/badge/Focus-Agent%20Based%20Scanning-orange?style=for-the-badge" alt="Focus Area" />
</p>

---

## Project Objective
> This project showcases how to securely deploy a Tenable Nessus Agent on a Linux virtual machine and run a triggered vulnerability scan. The process includes provisioning, linking, monitoring, and cleanup, highlighting how agent-based scanning is useful for systems not always reachable through direct scanning.

---

## Tools & Technologies
- **Platform:** Local Virtual Machine
- **OS:** Linux (Ubuntu or similar)
- **Tools:** Tenable.io (Cloud), Nessus Agent
- **Languages/Scripts:** Bash, curl

---

## Skills Gained / Focus Areas
- Deployed Nessus Agent using secure Bash scripting
- Configured Linux scan triggers for agent-based scanning
- Monitored agent registration, scan execution, and service status
- Practiced remote Linux administration via SSH
- Completed full cleanup lifecycle in Tenable.io

---

## Environment Setup
> A Linux VM was provisioned using a secure username and password. The Nessus Agent was installed and linked to a cloud-based Tenable.io environment. A trigger file was used to initiate the scan locally from the agent, ensuring that vulnerability data was collected and uploaded back to the portal.

![Environment Setup](assets/images/setup.jpg)

---

## Walkthrough
1. [Step 1: Provision VM and Agent Group](#step-1-provision-vm-and-agent-group)
2. [Step 2: Install Nessus Agent](#step-2-install-nessus-agent)
3. [Step 3: Trigger Agent Scan](#step-3-trigger-agent-scan)
4. [Step 4: Monitor and Analyze Results](#step-4-monitor-and-analyze-results)

---

### Step 1: Provision VM and Agent Group
> - Created a secure Linux VM (do **not** use labuser/Cyberlab123!)
> - Created an Agent Group under:  
  `Settings → Sensors → Nessus Agents → Agent Groups → +Add Agent Group`

![Step 1](assets/images/step1.jpg)

---

### Step 2: Install Nessus Agent
> - Logged into Tenable.io at [https://cloud.tenable.com](https://cloud.tenable.com)
> - Started provisioning a Nessus Agent  
> - Edited and copied the following Bash command:


> - Exported results if needed  
> - Deleted scan, agent group, unlinked agent, and deleted VM

![Step 4](assets/images/step4.jpg)

---

## Outcomes and Lessons Learned
- **Technical Insight:** Trigger-based agent scans are effective for segmented or remote environments where persistent connections aren’t feasible.
- **Configuration Skills:** Practiced editing curl commands and configuring Nessus triggers in Linux.
- **Troubleshooting:** Managed Linux service issues and file permissions to ensure scan execution.
- **Takeaway:** Agent-based scanning is a lightweight and flexible method for vulnerability monitoring across mixed environments.

---

## References
- [Tenable Agent Deployment Docs](https://docs.tenable.com/cloud/Content/NessusAgents/Install.htm)
- [Nessus Agent Trigger File Location](https://docs.tenable.com/cloud/Content/NessusAgents/TriggerScan.htm)
- [Tenable.io Portal](https://cloud.tenable.com/)

