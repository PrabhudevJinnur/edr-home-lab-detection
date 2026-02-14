# SOAR & EDR SOC Lab

## Project Overview

This project demonstrates a hands-on Security Operations Center (SOC) lab focused on **Endpoint Detection & Response (EDR)** and **Security Orchestration, Automation, and Response (SOAR)**.

The objective was to simulate adversary activity on monitored endpoints, analyze generated alerts, and perform structured SOC-style investigations in a controlled environment.

---

## Objectives

- Deploy and configure endpoint monitoring
- Simulate realistic attack behaviors
- Generate and analyze security alerts
- Conduct structured SOC investigations
- Validate detection rules and response workflows
- Understand how automation supports incident handling

---

## Lab Architecture

The lab environment consisted of:

- **Monitored Endpoint System**
  - Simulated user workstation
  - Generated attack telemetry

- **EDR Platform**
  - Collected endpoint telemetry
  - Triggered security alerts
  - Provided investigation timeline and event visibility

- **SOAR Workflow**
  - Simulated automated alert handling
  - Structured response validation
  - Incident documentation process

All activities were performed in an isolated test environment.

---

## Attack Simulation

Controlled attack scenarios were executed to generate meaningful telemetry, including:

- Suspicious process execution
- Credential-based activity
- Unauthorized system modifications
- Potential lateral movement indicators

The goal was visibility and detection validation — not exploitation.

---

## Detection & Investigation Process

### 1. Alert Generation

Simulated adversary activity triggered EDR alerts based on:

- Process behavior anomalies
- Suspicious command execution
- Unusual parent-child process relationships

---

### 2. Alert Triage

Each alert was analyzed by reviewing:

- Process tree relationships
- Command-line arguments
- File hashes
- User context
- Network indicators (if applicable)

Key triage questions:

- Is this behavior expected?
- Is this benign administrative activity?
- Does this match known attacker techniques?

---

### 3. Investigation Workflow

Investigation steps included:

- Reviewing event timeline
- Identifying initial execution vector
- Checking persistence indicators
- Evaluating lateral movement attempts
- Assessing impact and scope

---

### 4. SOAR Workflow Simulation

Response workflows were documented to simulate:

- Alert classification
- Incident creation
- Escalation criteria
- Containment steps
- Documentation procedures

Automation logic was evaluated conceptually to understand how repetitive SOC tasks can be reduced.

---

## Key Findings

- High-fidelity alerts require context validation before escalation.
- Process tree analysis is critical in endpoint investigations.
- Many alerts require correlation across multiple events.
- Structured investigation methodology prevents premature conclusions.
- Automation enhances efficiency but must be carefully tuned.

---

## Limitations

- Lab environment simulated controlled attack scenarios.
- No live production infrastructure was involved.
- Automation workflows were conceptual.
- Limited endpoint diversity.

---

## Future Improvements

- Integrate automated containment actions (e.g., host isolation)
- Develop custom detection rules
- Expand to multi-endpoint investigation scenarios
- Integrate threat intelligence enrichment
- Simulate phishing-to-endpoint attack chains

---

## Lessons Learned

- Endpoint visibility is critical for detecting post-compromise activity.
- Alert context is more important than alert volume.
- Investigation discipline reduces analyst bias.
- SOAR is most effective when paired with strong detection logic.

---

## Disclaimer

This lab was conducted in an isolated test environment for educational purposes only. All simulated attacks were controlled and intended for defensive learning.
