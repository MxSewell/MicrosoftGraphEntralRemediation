# Entra Graph Remediation Toolkit

Modular Powershell scripts for Entra ID security remediation using Microsoft Graph Powershell 7 SDK.

## Scripts
-  **Revoke-Sessions.ps1**
    Invalidate refresh tokens and revoke user sign-in sessions.
-  **Remove-Authenticator.ps1**
    Lists a user's Microsoft Authenticator methods and prompts script operator to choose which method(s) to remove.
-  **Reset-Password.ps1**
    Generates and assigns a strong/complex temporary password (>=16 chars).

## Requirements
-    Microsoft Graph Powershell SDK v2
-    Delegated Scopes:
      -  User.ReadWrite.All
      -  AuditLog.Read.All
 
## Usage Examples
-    .\Revoke-Sessions.ps1 -Users johndoe@contoso.com
-    .\Remove-Authenticator.ps1 -Users janedoe@fabrikam.com
