# Policy description:
    This policy audits if key vault objects are not recoverable. 
    Soft Delete feature helps to effectively hold the resources for a given 
    retention period (90 days) even after a DELETE operation, while giving the 
    appearance that the object is deleted. When 'Purge protection' is on, a 
    vault or an object in deleted state cannot be purged until the retention period 
    of 90 days has passed. These vaults and objects can still be recovered, assuring 
    customers that the retention policy will be followed.

# Services involved
    1. KeyVault

# NON COMPLIANT TEST SCENARIO
    Login to Azure
    Create a KeyVault
    Ensure purge, recovery protection is not applied
    Run the policy to get the violation

# COMPLIANT SCENARIO
    Follow the Non compliance scenario apply purge or recovery protection
    to key vault to resolve the violation