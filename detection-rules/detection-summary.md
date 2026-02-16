# Detection Summary – SOAR & EDR Lab

## Overview

This document summarizes the custom detection and response rule created during the SOAR & EDR lab.

Unlike relying solely on default detection logic, a custom detection rule was configured to identify specific adversary behavior simulated on the monitored endpoint.

---

## Custom Detection Rule

A detection rule was created to monitor for execution of a credential dumping tool (LaZagne).

The rule was configured to trigger when:

- The executable name matched `LaZagne.exe`
- Suspicious command-line arguments were observed
- Execution occurred from a user download directory
- File was unsigned or untrusted

---

## Response Logic

Upon detection, the system:

- Generated a high-severity alert
- Sent structured alert details including:
  - Time
  - Computer name
  - Source IP
  - Process name
  - Command line
  - File path
  - File hash
- Routed notification through Slack and Email
- Prompted the user for endpoint isolation decision

If isolation was confirmed:
- The endpoint was isolated via response action.

If isolation was declined:
- A notification message was sent indicating the system was not isolated.

---

## What Was Validated

- Custom detection logic successfully triggered on simulated credential dumping activity.
- Alert metadata contained sufficient forensic context for investigation.
- Response workflow executed as expected.
- Endpoint isolation functionality operated correctly.

---

## Key Learning

This lab demonstrated how custom detection engineering can improve visibility beyond default EDR alerts.

It reinforced the importance of:

- Defining detection conditions carefully
- Validating alert fidelity
- Integrating detection logic with automated response workflows
