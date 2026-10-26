# Lab 12: RBAC and Least Privilege

## Objective
Apply role-based access control (RBAC) by choosing a role with only the permissions needed for a task.

## Scenario
A support technician needs to reset passwords for non-administrator users. The Password Administrator role is more appropriate for this task than Global Administrator.

## Actions performed
- Reviewed the Password Administrator role description and permissions in Microsoft Entra.
- Confirmed the role had no existing assignments.
- Assigned Password Administrator to the SOC Test User at directory scope.
- Removed the temporary role assignment after verifying it.

## Result
The test account received the selected role, and the assignment was then removed. No user password was reset; this exercise demonstrated role assignment and removal.

## Evidence
- Password Administrator role description.
- Role assignment to the SOC Test User at directory scope.
- Successful removal confirmation and empty assignments list.
![Password Administrator role assignment removed](password-administrator-assignment-removed.png.png)
