# Policy description:
  This policy audits whether LogRetention for SQL Server is enabled. 
  A log data retention period of 90 days or more, should allow you to 
  collect the necessary amount of audit data useful to check for anomalies \
  and potential security breaches, or misuse of information and access to the 
  SQL servers. This policy becomes non-compliant if LogRetention 
  for SQL Server is not enabled.   

# Services involved
    1. SQL SERVER
    2. SQL DATABASE

# NON COMPLIANT TEST SCENARIO
    Login to Azure
    Create an SQL Server and an SQL Database
    Click on the newly created SQL Server
    Click on Backups and navigate to Retension Polices
    Select the SQL Database
    Click on Configure Policies
    Keep the LTR value below 90 days and apply

# COMPLIANT SCENARIO
    Follow the Non compliance scenario just update the LTR value to more
    than 90 days.