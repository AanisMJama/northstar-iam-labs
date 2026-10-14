# Lab 1 — Identity Lifecycle

**Status:** Planned  
**Company:** Northstar Community Services Ltd. *(fictional)*  
**Ticket:** IAM-LAB-001

## Objective

Practise an approved joiner, mover and leaver process in the isolated Active Directory lab. Apply least privilege, verify each access change, and keep an audit trail.

## Scenario

HR requests access for **Maya Noor**, a fictional employee joining as a Service Desk Analyst. Later, Maya moves into an IAM Analyst role and eventually leaves the company.

## Planned workflow

- **Joiner:** Record HR and manager approval, create the account, and grant the approved `NS-Staff` and `NS-ServiceDesk` group access.
- **Mover:** Record approval for the new role, remove `NS-ServiceDesk` access, and add approved `NS-IAM-Analysts` access.
- **Leaver:** Record the effective leaving time, disable the account promptly, remove access, and retain the account record for audit according to the scenario.

## Evidence to add after performing the lab

- Approval and request record using fictional details.
- Screenshots showing account status and group membership at each stage.
- A short action log with timestamps and verification results.
- A closure summary explaining how access was removed.

## Safety and scope


## Results

*Pending lab execution.*
