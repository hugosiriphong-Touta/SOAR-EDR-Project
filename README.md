# SOAR–EDR Integration Project

## Project Overview
This project demonstrates how I integrated a **SOAR platform (Tines)** with an **EDR solution (LimaCharlie)** to automate incident detection and response.  

**Goal:** Reduce manual workload during incident handling by creating an automated playbook capable of:  
- Detecting suspicious endpoint activity  
- Sending alerts to communication channels (Slack / Email)  
- Allowing analyst decisions (isolate or investigate further)  
- Automating response actions like endpoint isolation  

---

## Tools & Technologies
- **SOAR:** Tines  
- **EDR:** LimaCharlie  
- **Communication:** Slack, Email  
- **Automation:** Webhooks, API calls  
- **Scripting:** PowerShell  
- **Hosting / Testing:** Vultr  
- **Repository & References:** GitHub (for scripts, playbooks, and guidance like LaZagne.exe usage)  

---

## Architecture Workflow

The following diagram illustrates the playbook workflow:

<a href="https://github.com/hugosiriphong-Touta/SOAR-EDR-Project/blob/main/documentation/SOAR~EDR%20PLAYBOOK.png"> Architecture Workflow Diagram </a>

**Workflow Summary:**  
1. **Detection** → LimaCharlie identifies suspicious endpoint activity.  
2. **Alert Forwarding** → Event is sent to Tines.  
3. **Notification** → Tines sends Slack/Email alerts with details.  
4. **Analyst Decision** → A user prompt asks whether to isolate the endpoint.  
   - **YES** → LimaCharlie isolates the endpoint + sends status to Slack.  
   - **NO** → A message of investigation is sent for further review.  

---

## Features
- Automated suspicious activity detection and alerting  
- Slack and Email integration for real-time notifications  
- Analyst decision-making directly in the workflow  
- Automatic endpoint isolation when approved  
- Clear audit trail through Slack updates  

---

## Repository Contents
- `/docs` → Diagrams, documentation, screenshots

---

## Outcomes & Learning
- Reduced time between detection and response  
- Hands-on experience with SOAR orchestration  
- Learned how to integrate APIs between SOAR, EDR, and communication tools  
- Gained understanding of incident response workflows and decision automation  

---

## References
- [Tines Documentation](https://tines.com/docs)  
- [LimaCharlie API Docs](https://www.limacharlie.io/docs)  
- [LaZagne Project](https://github.com/AlessandroZ/LaZagne)  
- [Slack API Documentation](https://api.slack.com)  
- [Vultr Cloud Hosting](https://www.vultr.com)  
