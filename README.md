# Hands-On Tier-1 SOC Operations Using Wazuh: Detection, Investigation, and Incident Documentation

## Overview

This project demonstrates the design and implementation of a SOAR-based automated incident response system using Shuffle.

The platform was built to simulate real SOC automation workflows that respond to SIEM alerts by validating risk, applying decision logic, and executing controlled response actions.

The objective was to demonstrate how Tier-1 SOC investigations can transition into structured, auditable automated response playbooks while maintaining security guardrails.

## SOC Role Alignment

This project reflects Tier-1 and Tier-2 SOC responsibilities, including:

- Translating SIEM alerts into structured response workflows
- Applying validation logic before automated actions
- Simulating containment actions such as IP blocking and account disablement
- Automating phishing response while maintaining analyst oversight
- Maintaining audit logs for SOC accountability

## Lab Environment

- Ubuntu Server (SOAR host)
- Shuffle SOAR platform running in Docker containers
- Simulated SIEM alerts delivered via webhooks
- Controlled virtual lab environment (VirtualBox)

The environment was designed to model how real SOC teams integrate SIEM alerts with SOAR automation.

## Automation Playbooks Implemented

Three automated SOC response workflows were developed:

1. **Malicious IP Auto Response**
   - Validates severity of SIEM alerts
   - Simulates IP blocking action
   - Logs response for SOC audit

2. **Account Compromise Auto Response**
   - Validates failed login thresholds
   - Simulates disabling compromised user accounts
   - Records actions and notifies SOC

3. **Phishing Email Auto Isolation**
   - Simulates threat intelligence hash checks
   - Applies decision logic before isolating email
   - Logs response and alerts analysts

Each playbook demonstrates structured decision-making, not blind automation.


## Evidence and Documentation

This repository includes:

- Incident reports documenting investigation findings
- Screenshots of SIEM alerts and telemetry
- A clear investigation methodology
- Supporting lab configuration notes

All evidence is preserved and organized to reflect real SOC documentation standards.

## Skills Demonstrated

- SOAR platform deployment and configuration
- Automation workflow design and testing
- Security decision logic implementation
- Simulated incident containment procedures
- SOC audit logging and response documentation
- Integration of SIEM alerts into automated workflows

## Disclaimer

All activities in this project were conducted in a controlled lab environment for educational and defensive security purposes only.
No real-world systems or data were targeted.
