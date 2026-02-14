# SOAR & EDR Lab Architecture

## Overview

This lab simulates a simplified SOC environment integrating Endpoint Detection & Response (EDR) with conceptual SOAR workflows.

The architecture focuses on visibility, detection, investigation, and response simulation.

---

## Architecture Components

### 1. Endpoint System

- Simulated user workstation
- Generates process, authentication, and system telemetry
- Used to execute controlled attack simulations

---

### 2. EDR Platform

- Collects endpoint telemetry
- Detects suspicious behavior
- Generates alerts based on detection logic
- Provides investigation timeline and process tree visibility

---

### 3. SOC Investigation Layer

- Alert triage
- Event correlation
- Process tree analysis
- Incident documentation

---

### 4. SOAR Simulation Layer

- Alert classification logic
- Escalation workflow simulation
- Response validation process
- Documentation and reporting flow

---

## Data Flow

1. Simulated attack executed on endpoint.
2. EDR agent collects telemetry.
3. Detection rule triggers alert.
4. SOC investigation initiated.
5. Findings documented.
6. Response workflow evaluated.

---

## Security Boundaries

- Lab operated in isolated environment.
- No production systems involved.
- No external unauthorized systems targeted.
- All activity controlled for defensive learning.

---

## Architecture Summary

The lab demonstrates:

- Endpoint telemetry collection
- Detection engineering fundamentals
- Structured SOC investigation process
- Conceptual automation workflows

This setup mirrors real-world SOC workflows at a simplified scale.

