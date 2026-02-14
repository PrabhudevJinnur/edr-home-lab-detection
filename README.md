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
- Comm
