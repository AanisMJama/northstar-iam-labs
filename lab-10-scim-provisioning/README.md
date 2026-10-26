# Lab 10: SCIM Provisioning and Deprovisioning

## Goal
Document how an organization could automatically create, update, and deactivate user accounts in a SaaS application using SCIM 2.0.

## Exercise type
**Design exercise only.** No SCIM endpoint is connected, and no accounts were provisioned in Microsoft Entra ID.

## Example onboarding plan
- **Example app:** Northstar Learning Portal
- **Source of user data:** Microsoft Entra ID
- **Users assigned through group:** `APP-Northstar-Learning-Users`
- **Account created when:** A user is added to the assigned group and provisioning is enabled.
- **Account updated when:** The user's name, email, or department changes in Entra ID.
- **Account deactivated when:** The user is removed from the assigned group or disabled in Entra ID, according to the app's provisioning rules.

## Attribute mapping plan

| Entra ID value | SCIM user attribute |
|---|---|
| User principal name | `userName` |
| First name | `name.givenName` |
| Last name | `name.familyName` |
| Work email | `emails[type eq "work"].value` |
| Department | `department` |
| Account enabled status | `active` |

## Deprovisioning check
When access is removed, the provisioning service should set the user's SCIM `active` value to `false` or deactivate the account, based on the SaaS app's supported behavior. The app owner should verify that access is revoked and determine how the app retains the user's data.

## What a real setup needs
A real integration requires a reachable SCIM 2.0 endpoint, credentials or a secret token, supported attribute mappings, and a test assignment. Those were not available for this exercise.

## Result
Documented a group-based SCIM onboarding and offboarding design, including example attribute mappings and the information needed before a live integration can be tested.
