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
![Tines Workflow Part 1](img/a1.png) 
### SOAR Workflow in Tines (Part 2)
![Tines Workflow Part 2](img/a2.png) 

*Combined, these screenshots represent the full SOAR playbook structure inside Tines, which connects LimaCharlie detections with automated actions such as Slack and Email notifications.* --- 
## Workflow 
Steps 
1. [Endpoint Enrollment](img/01.png)

   *The EDR agent (`touta-soar-edr`) is successfully installed, connected, and the firewall has been configured.*
   
2. [Attack Simulation](img/02.png)

  *The `lazagne.exe` program was executed on the test machine hosted on Vultr to test the firewall and the security defenses by attempting to access stored credentials, which triggers alerts if blocked.*

3. [Tines Alert Reception](img/03.png)

  *Tines successfully received an alert via webhook from the EDR system. The workflow is triggered automatically, and the firewall rules ensure that incoming alerts are accepted only from trusted sources.*
   
4. [Slack Notification](img/04.png)

 *The alert from Tines was forwaded to Slack, providing detailed information about the endpoint event. Firewall and integration rules ensure that only authorized notifications are sent to the designated Stack channel.*

5. [Email Notification](img/05.png)

 *Tines automatically sent an alert via email to the designated recipient, containing all relevant details about the endpoint event. Firewall and email security rules ensure that notifications are sent securely and only to authorized personnel.*

6. [Slack Notification](img/06.png)
9. [Email Notification](img/07.png)
10. [Response Action](img/08.png)
