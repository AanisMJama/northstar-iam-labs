# IAM-LAB-003 — Microsoft Entra ID Group Access Review

**Status:** Read-only review complete. No tenant settings or memberships were changed.

## Objective

Review an existing Entra security group’s membership and ownership, record a simulated business decision, and identify any access-governance gaps.

## Scenario

Northstar is a fictional company. This lab reviews the existing `Marketing` security group and its lab account, `SOC Test User`.

The tenant used is a personal Microsoft Entra ID Free test tenant. The business approval described below is simulated for this portfolio exercise; it is not a real manager approval.

## Review steps

1. Opened the `Marketing` group in the Microsoft Entra admin center.
2. Confirmed it is a cloud-sourced Security group with Assigned membership.
3. Checked the direct members and confirmed `SOC Test User` is already a member.
4. Checked group ownership and found the tenant administrator account is the sole owner.
5. Recorded the simulated manager decision to retain access for this exercise.
6. Made no changes to the tenant.

## Findings

- The reviewed membership already existed before this lab. This review does not prove how or when the original access was approved.
- The group has one direct lab user.
- The tenant administrator is the sole group owner. A separate Marketing business owner should be designated to review business need and access.
- No access was added or removed during this read-only review.

## Outcome

**Simulated review decision:** Retain `SOC Test User` in `Marketing` for this exercise.

**Recommended follow-up:** Assign an appropriate business owner and keep a real approval and review record for future access decisions.

## Evidence

Redacted screenshots of the group overview, members, and owners will be added here. Personal account details, email addresses, tenant identifiers, and object IDs must be hidden before publication.
