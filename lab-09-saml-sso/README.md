# Lab 9: SAML Single Sign-On

## Objective
Configure Microsoft Entra ID to provide SAML single sign-on to the Microsoft Entra SAML Toolkit.

## Configuration
- Identity provider: Microsoft Entra ID
- Service provider: Microsoft Entra SAML Toolkit
- Toolkit connection ID: 22757
- Entity ID: `https://samltoolkit.azurewebsites.net`
- Reply URL: `https://samltoolkit.azurewebsites.net/SAML/Consume/22757`
- Sign-on URL: `https://samltoolkit.azurewebsites.net/SAML/Login/22757`

## Test result
The SAML sign-in completed successfully. The Toolkit home page displayed the signed-in test user.

## Evidence
- `04-saml-sso-success.png` — redact the user’s email before uploading.
