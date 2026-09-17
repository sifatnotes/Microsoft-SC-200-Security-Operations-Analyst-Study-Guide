# Microsoft-SC-200-Security-Operations-Analyst-Study-Guide
SC-200 study guide covering Microsoft Defender XDR, Sentinel, Defender for Cloud, incident response, KQL threat hunting, detection engineering, and security operations.
# Microsoft SC-200: Security Operations Analyst Study Guide

## Introduction

This independent study guide is for **Microsoft SC-200: Microsoft Security Operations Analyst**.

It covers security operations using Microsoft Defender XDR, Microsoft Sentinel, Microsoft Defender for Cloud, Microsoft Entra ID, Microsoft Purview, KQL, incident response, detection engineering, automation, and threat hunting.

Microsoft's current skills measured are dated **July 28, 2026**. [1]

## Exam Overview

| Item | Information |
|---|---|
| Vendor | Microsoft |
| Exam | SC-200 |
| Certification | Microsoft Certified: Security Operations Analyst Associate |
| Level | Intermediate |
| Role | Security Operations Analyst |
| Purpose | Investigate, respond to, and hunt security threats |
| Duration | 100 minutes |
| Passing score | 700 or greater |
| Languages | English, Japanese, Chinese (Simplified), Korean, French, German, Spanish, Portuguese (Brazil), Chinese (Traditional), Italian |
| Price | $165 USD* |

\*Microsoft states that exam pricing depends on the country or region where the exam is proctored. Verify current pricing before registration. [2]

The certification is renewed every 12 months through Microsoft's renewal assessment process. [2]

## Who Should Take It?

SC-200 is designed for security operations analysts who monitor, investigate, triage, respond to incidents, hunt threats, and engineer detections.

Useful background includes:

- Microsoft security solutions
- Microsoft 365
- Azure
- Microsoft Sentinel
- Microsoft Defender XDR
- Microsoft Defender for Cloud
- Microsoft Entra ID
- KQL
- Windows and Linux
- Basic cloud and networking concepts

Microsoft also expects familiarity with AI agents and Copilots used within security operations. [1]

## Exam Objectives / Domains

### 1. Manage a Security Operations Environment — 40–45%

Study:

- Microsoft Defender XDR
- Microsoft Sentinel
- Defender for Endpoint
- Security policies
- Alert configuration
- Alert tuning and suppression
- Notifications
- Automated investigation and response
- Automatic attack disruption
- Custom data collection
- Attack Surface Reduction rules
- Microsoft Sentinel workspaces
- Data connectors
- Analytics rules
- Automation rules
- Playbooks
- Threat intelligence
- Content Hub
- Workbooks
- UEBA
- Security monitoring

### 2. Respond to Security Incidents — 35–40%

Focus on:

- Alerts
- Incidents
- Triage
- Investigation
- Microsoft Defender XDR incidents
- Defender for Endpoint incidents
- Microsoft Sentinel incidents
- Microsoft 365 activity investigation
- Identity threats
- Endpoint threats
- Email threats
- Cloud threats
- Remediation
- Evidence collection
- Incident response workflows
- Automated response

### 3. Perform Threat Hunting — 20–25%

Study:

- Kusto Query Language (KQL)
- Hunting queries
- Advanced hunting
- Microsoft Sentinel hunting
- Defender XDR hunting
- Threat indicators
- MITRE ATT&CK concepts
- Query filtering
- Joins
- Aggregation
- Time-based analysis
- Investigation of suspicious activity
- Custom detections

These three domains and weightings are Microsoft's current published skills measured. [1]

## Detailed Study Notes

### Microsoft Defender XDR

Defender XDR correlates security signals across Microsoft security products.

Understand:

**Alert → Incident → Investigation → Response → Remediation**

Study incidents, alerts, advanced hunting, automated investigation and response, attack disruption, and security recommendations.

### Microsoft Sentinel

Sentinel is Microsoft's cloud-native SIEM and security analytics platform.

Understand:

- Log Analytics workspaces
- Data connectors
- Analytics rules
- Incidents
- Automation rules
- Playbooks
- Workbooks
- Threat intelligence
- Hunting
- UEBA

### KQL

KQL is essential for SC-200.

Practice:

```kql

Know:

where
project
extend
summarize
count()
distinct
sort
join
union
has
contains
ago()
Time filtering

Focus on understanding what a query returns rather than memorizing syntax.

Incident Response

A useful investigation sequence is:

Detect → Triage → Investigate → Contain → Remediate → Validate

Understand incident severity, related alerts, entities, evidence, timelines, affected users/devices, and response actions.

Defender for Endpoint

Study:

Device onboarding
Alerts
Incidents
Advanced hunting
Endpoint detection
Attack Surface Reduction
Automated investigation
Remediation
Device isolation
Live response
Vulnerability information
Defender for Cloud

Understand:

Cloud security posture
Workload protection
Security recommendations
Alerts
Cloud resources
Regulatory/compliance information
Defender plans
Identity Threats

Review Microsoft Entra security concepts:

Sign-in logs
Risky users
Risky sign-ins
Authentication
Conditional Access
Identity Protection
Suspicious authentication activity
Threat Hunting

Threat hunting is proactive investigation rather than waiting for alerts.

Use:

Hypothesis → KQL query → Evidence → Investigation → Detection/response

Look for unusual users, devices, processes, authentication patterns, network activity, and cloud behavior.

Important Concepts

Revise:

Microsoft Defender XDR
Microsoft Sentinel
Defender for Endpoint
Defender for Cloud
Microsoft Entra ID
Microsoft Purview
SIEM
SOAR
Incidents
Alerts
Triage
Advanced hunting
KQL
Analytics rules
Automation rules
Playbooks
Data connectors
Workbooks
UEBA
Threat intelligence
Attack Surface Reduction
Automated investigation and response
Automatic attack disruption
Endpoint isolation
Incident remediation
Threat hunting
MITRE ATT&CK
Detection engineering
Practical Examples / Labs

Use only authorized Microsoft tenants and test environments.

Create a Microsoft Sentinel workspace.
Configure supported data connectors.
Create an analytics rule.
Generate and investigate a test incident.
Configure an automation rule.
Create an authorized Logic App playbook.
Explore Defender XDR incidents.
Investigate Defender for Endpoint alerts.
Practice Advanced Hunting.
Write KQL queries using security tables.
Investigate suspicious sign-ins.
Review Microsoft Entra risk information.
Investigate a simulated phishing incident.
Review Defender for Cloud recommendations.
Configure an ASR policy in a test environment.
Practice endpoint isolation with an authorized test device.
Create a hunting query for unusual authentication.
Create a custom detection scenario.
Review threat-intelligence indicators.
Build an end-to-end incident investigation workflow.
Study Strategy

Use Microsoft Learn, official documentation, the SC-200 study guide, hands-on labs, Microsoft's Practice Assessment, and the exam sandbox.

Prioritize:

Defender XDR
Microsoft Sentinel
KQL
Incident investigation
Detection and automation
Defender for Cloud
Identity investigation
Threat hunting

Microsoft recommends hands-on experience and provides a free Practice Assessment and exam sandbox. 1

30-Day Study Plan

Days 1–4: Security operations concepts, Defender XDR, Microsoft security architecture, alerts, and incidents.

Days 5–8: Microsoft Sentinel, workspaces, data connectors, analytics rules, incidents, workbooks, and threat intelligence.

Days 9–12: Sentinel automation rules, Logic Apps, playbooks, UEBA, and security monitoring.

Days 13–16: Defender for Endpoint, endpoint alerts, ASR, automated investigation, remediation, and advanced hunting.

Days 17–19: Defender for Cloud, workload protection, recommendations, alerts, and cloud investigation.

Days 20–22: Microsoft Entra ID, sign-in investigation, risky users, risky sign-ins, and identity threats.

Days 23–26: KQL fundamentals, filtering, aggregation, joins, time analysis, and advanced hunting.

Days 27–28: Threat hunting, custom detections, threat intelligence, and MITRE ATT&CK concepts.

Day 29: Full incident-response scenarios and troubleshooting.

Day 30: Practice Assessment, exam sandbox, weak-area revision, and final review.

Common Mistakes
Memorizing KQL instead of understanding query logic
Confusing alerts with incidents
Ignoring incident timelines and entities
Treating Sentinel and Defender XDR as identical products
Ignoring data connectors when investigating missing telemetry
Creating overly broad analytics rules
Ignoring false-positive tuning
Confusing prevention with detection and response
Investigating identity threats without checking sign-in context
Using response actions without validating their scope
Studying outdated SC-200 objectives
Practicing security actions against unauthorized systems
Exam-Day Tips
Read the complete scenario before choosing an answer.
Identify whether the problem concerns detection, investigation, response, or hunting.
For Sentinel questions, identify the relevant workspace, connector, rule, incident, or automation component.
For KQL questions, trace the query line by line.
For Defender questions, determine which security workload owns the alert or investigation.
For identity questions, examine sign-in and risk context.
Eliminate solutions that use unnecessary response actions.
Manage the 100-minute exam carefully.
Microsoft requires 700 or greater to pass. 1
Final Checklist
 Understand Defender XDR
 Understand Microsoft Sentinel
 Know Defender for Endpoint
 Know Defender for Cloud
 Understand Microsoft Entra security
 Know Microsoft Purview security/compliance context
 Can investigate incidents
 Can triage alerts
 Can configure Sentinel data connectors
 Understand analytics rules
 Understand automation rules
 Know playbooks
 Comfortable with KQL
 Can perform advanced hunting
 Understand ASR
 Understand automated investigation
 Know endpoint remediation
 Understand threat intelligence
 Can investigate identity threats
 Can perform threat hunting
 Completed hands-on labs
 Completed Microsoft's Practice Assessment
 Used the exam sandbox
 Reviewed the current official study guide
Official Resources
SC-200 Exam:
https://learn.microsoft.com/credentials/certifications/exams/sc-200/
SC-200 Study Guide:
https://learn.microsoft.com/credentials/certifications/resources/study-guides/sc-200
Security Operations Analyst Associate:
https://learn.microsoft.com/credentials/certifications/security-operations-analyst/
Microsoft Sentinel:
https://learn.microsoft.com/azure/sentinel/
Microsoft Defender XDR:
https://learn.microsoft.com/defender-xdr/
Microsoft Defender for Cloud:
https://learn.microsoft.com/azure/defender-for-cloud/
Microsoft Defender for Endpoint:
https://learn.microsoft.com/defender-endpoint/
Kusto Query Language:
https://learn.microsoft.com/kusto/query/
Microsoft Learn:
https://learn.microsoft.com/training/
Practice Assessments:
https://learn.microsoft.com/credentials/certifications/practice-assessments-for-microsoft-certifications

Always verify current SC-200 objectives, exam format, pricing, languages, certification requirements, and policies directly with Microsoft.

Voucher / Discount

Learn SecByte, an official Microsoft reseller partner, provides certification voucher options and discounts where available.

Learn SecByte's official Black Friday offer provides up to 70% off selected Microsoft exam vouchers.

SC-200 voucher:

https://learn.secbyte.org/vouchers/microsoft-sc-200

Check the current offer and availability before purchasing. Do not assume this specific exam is 70% off unless the current offer explicitly states it. Voucher pricing and availability may change.

Disclaimer

This is an independent/community study guide and is not an official Microsoft certification document. Microsoft, Microsoft Sentinel, Microsoft Defender, Microsoft Entra, Microsoft Purview, Azure, and related trademarks belong to Microsoft.

Candidates should verify current exam information, objectives, pricing, policies, certification requirements, and voucher availability directly with Microsoft.

This repository does not contain exam dumps, leaked questions, or recalled exam questions. It is intended for legitimate education, authorized hands-on practice, and certification preparation only.


Microsoft's current SC-200 study guide lists the three domains as **Manage a security operations environment (40–45%)**, **Respond to security incidents (35–40%)**, and **Perform threat hunting (20–25%)**; the study guide was updated for skills measured **July 28, 2026**. :contentReference[oaicite:0]{index=0} 
| where TimeGenerated > ago(24h)
| summarize Count=count() by Account
| order by Count desc
