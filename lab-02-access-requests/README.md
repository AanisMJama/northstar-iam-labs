# IAM-LAB-002 — Access Request and Least Privilege

**Status:** Lab execution complete — read access allowed; file creation denied.

## Objective

Process an access request with approval, grant only the required access through a security group, and verify the result.

## Fictional ticket

- **Company:** Northstar
- **Requester:** Finance Manager
- **User:** Samira Ahmed, Finance Assistant
- **Request:** Read-only access to the Finance shared resource
- **Proposed AD group:** `NS-Finance-ReadOnly`
- **Manager approval:** Simulated approval recorded — Hassan Ali, Finance Manager, 16 October 2026. Approved scope: read-only Finance access only.
- **Environment:** Isolated `cyberlab.local` lab

## Workflow performed

1. Recorded the fictional access request and manager approval.
2. Confirmed Samira’s identity and read-only business need.
3. Created the `NS-Finance-ReadOnly` group and configured the Finance share permissions.
4. Added Samira to the group after approval.
5. Tested access from `WIN10-CLIENT01`: reading succeeded; creating a file was denied.
6. Recorded the results for the audit trail.


## Results

- Recorded simulated manager approval from Hassan Ali, Finance Manager, for read-only Finance access.
- Added Samira Ahmed to `NS-Finance-ReadOnly`.
- Signed in as Samira on `WIN10-CLIENT01` and opened `\\DC-01\Finance`.
- Confirmed Samira could view `Finance-ReadOnly-Test.txt`.
- Tried to create a text document. Windows displayed **Destination Folder Access Denied**; the folder still contained only the original file.

## Evidence

Portfolio screenshots will be added to this lab folder.
