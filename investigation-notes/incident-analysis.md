# Incident Analysis – Simulated Alert Investigation

## Overview

This document outlines the investigation process performed during the SOAR & EDR lab after generating simulated attack activity on the monitored endpoint.

The goal was to analyze alerts triggered by the EDR platform and follow a structured SOC-style investigation process.

---

## Alert Trigger

After executing controlled attack simulation activity on the endpoint, the EDR platform generated an alert based on suspicious behavior.

The alert was reviewed within the monitoring dashboard.

---

## Investigation Steps

### 1. Alert Review

- Reviewed alert summary
- Identified affected endpoint
- Observed timestamp of activity
- Noted alert severity level

---

### 2. Process Analysis

- Examined process tree
- Reviewed parent-child process relationships
- Checked command-line arguments
- Confirmed execution context

---

### 3. Context Validation

- Verified whether the activity was intentionally simulated
- Confirmed no unintended system impact
- Ensured activity aligned with the controlled lab scenario

---

## Findings

- Alert was successfully triggered by simulated activity
- Detection logic responded as expected
- Process relationships were clearly visible in the EDR platform
- Investigation workflow followed structured SOC methodology

---

## Conclusion

The lab demonstrated how endpoint telemetry is collected, how alerts are generated, and how a SOC analyst would investigate suspicious activity within an EDR platform.

This exercise reinforced the importance of reviewing process context and validating alerts before escalation.
