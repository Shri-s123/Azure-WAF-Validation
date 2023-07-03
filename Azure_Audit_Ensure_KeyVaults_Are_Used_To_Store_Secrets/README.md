# Policy description:
  This policy audits whether Key vaults are used to store secrets. 
  Encryption keys,Certificate thumbprints and Managed Identity Credentials can be stored 
  in Keyvault to maintain security of these keys. This policy becomes non-compliance if the 
  Key vaults are not used to store secrets.  

# Services involved
    1. Azure Key Vault

# NON COMPLIANT TEST SCENARIO
    Login to Azure
    Create Key Vault
    Navigate to the Objects section, ensure no Keys and Secrets are present
    Run this policy and check for violation

# COMPLIANT SCENARIO
    Follow the non compliance scenarion, just add a new Key and Secret value to 
    simulate the compliant scenario