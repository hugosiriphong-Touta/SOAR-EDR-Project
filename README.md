# Cybersecurity Project – SOAR + EDR with Tines & LimaCharlie

## Objective
- Automate the detection and response of endpoint threats by integrating a **SOAR platform (Tines)** with an **EDR tool (LimaCharlie)**.
- Create automated workflows that respond in real time to suspicious activity on Linux and Windows endpoints.
- Simulate a real SOC environment for hands-on experience.

## Skills Learned
- Built automated security workflows using Tines SOAR.
- Monitored and analyzed endpoint activity with LimaCharlie EDR.
- Planned and executed incident response scenarios.
- Practiced scripting and automation to integrate multiple security tools.
- Developed critical thinking and problem-solving skills for SOC operations.

## Tools Used
- **Tines** – Automation & SOAR platform
- **LimaCharlie** – Cloud-native EDR
- **Linux & Windows endpoints** – Test machines
- **GitHub** – Documentation and project sharing
- **Automation/testing tools** – e.g., Atomic Red Team

## Steps
- **Deploy LimaCharlie Agent**
  - Install the LimaCharlie agent on Linux/Windows endpoints
  - Configure detection rules for privilege escalation, persistence, and malware execution

- **Configure Tines Integration**
  - Create Tines stories (automation workflows)
  - Connect Tines to LimaCharlie via API/webhooks
  - **Example workflow:**
    - Trigger: LimaCharlie detects suspicious activity
    - Action: Tines sends Slack/Teams alert, quarantines host, or creates a Jira ticket

- **Simulate Attacks**
  - Use tools like Atomic Red Team or manual testing (privilege escalation, credential dumping)
  - Verify that alerts are detected and automated responses executed

## Example Screenshots
- **Ref 1: Network Diagram** – Shows the test lab setup including endpoints, Tines, and LimaCharlie connections.
- **Ref 2: Tines Workflow** – Example of automated response triggered by a suspicious event.
- **Ref 3: Detection Alert** – Screenshot showing LimaCharlie detecting a test attack and triggering the SOAR workflow.
