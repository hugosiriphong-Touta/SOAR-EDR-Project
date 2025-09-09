# SOAR–EDR Integration Project

This project demonstrates the integration of a SOAR platform (Tines) with an EDR solution (LimaCharlie) to automate incident detection and response. The lab environment was hosted on a Vultr virtual machine.  

## Overview

- Goal: Automate detection and response to endpoint threats  
- Tools Used:  
  - LimaCharlie (EDR)  
  - Tines (SOAR)  
  - Slack & Email (notifications)  
  - Vultr (virtual machine hosting)  
- Scenario: An attacker runs a credential-dumping tool (`lazagne.exe`) on a Windows endpoint.  
  - EDR detects malicious behavior  
  - SOAR ingests the alert and triggers a playbook  
  - Automated notifications and response actions are executed 
---

## Architecture

The SOAR–EDR architecture was designed and implemented inside **Tines**.  
Because the workflow is large, it is shown in two parts below.

### SOAR Workflow in Tines (Part 1)
<a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/a1.png">View Screenshot Part 1</a>

### SOAR Workflow in Tines (Part 2)
<a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/a2.png">View Screenshot Part 2</a>

*Combined, these screenshots represent the full SOAR playbook structure inside Tines, which connects LimaCharlie detections with automated actions such as Slack and Email notifications.*

---

## Workflow Steps

1. <a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/01.png">Endpoint Enrollment</a>  
2. <a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/02.png">Attack Simulation</a>  
3. <a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/03.png">EDR Detection</a>  
4. <a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/04.png">Event Forwarding to SOAR</a>  
5. <a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/05.png">SOAR Playbook Trigger</a>  
6. <a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/06.png">Slack Notification</a>  
7. <a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/07.png">Email Notification</a>  
8. <a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/img/08.png">Response Action</a>  
