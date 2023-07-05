
## Policy Description
This policy audits whether Virtual Machines with IP Forwarding Enabled. Enabling IP forwarding on a virtual machine's NIC allows the machine to receive traffic addressed to other destinations. IP forwarding is rarely required (e.g., when using the VM as a network virtual appliance), and therefore, this should be reviewed by the network security team. This policy becomes non-compliant if Virtual Machines has IP Forwarding Enabled.
## SERVICES INVOLVED
 Appservices

## COMPLIANT TEST SCENARIO
    Login to azure portal
    Create Vm
    Go to Network Interface of the VM
    Click on IP Configurations from the left menu
    Uncheck the Enable IP Forwarding checkbox
    

## NON COMPLIANT TEST SCENARIO
    Enable IP Forwarding 



