
## Policy Description
This policy audits whether Network Interfaces have any Public IP address assigned to it. Public IPs increase your chances of cyberattacks, privacy breaches, and identity thefts. This policy becomes non-compliant if the Network Interfaces which are having associated Public IP addresses.

## SERVICES INVOLVED
 Network Interface

## COMPLIANT TEST SCENARIO
    Login to azure portal
    Create Network Interface
    Associate Public Ip address to an IP Configuration

## NON COMPLIANT TEST SCENARIO
    Dissociate all Public Ips attached.
