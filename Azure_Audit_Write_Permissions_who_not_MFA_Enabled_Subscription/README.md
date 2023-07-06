
## Policy Description
This policy audits whether Accounts with write permissions that are MFA disabled in subscription. It should be done for all subscription accounts with write privileges to prevent a breach of accounts or resources.

## SERVICES INVOLVED
 Azure Subcription

## COMPLIANT TEST SCENARIO
    Login to azure portal
    Go to Subcription
    Click on IAM in left menu
    Filter users with writer role and get the result
    Go to the Active Directory
    Navigate to Users 
    Click on Per User MFA 
    Enable MFA for all users with writer role

## NON COMPLIANT TEST SCENARIO (NO Adequate Permissions to simulate)
    Go to AD->Properties in left menu under manage
    Disable Security Defaults
    Go to the Active Directory
    Navigate to Users 
    Click on Per User MFA 
    Disable MFA for users with writer role


