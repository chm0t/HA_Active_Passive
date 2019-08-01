# HASkillet
The HASkillet will configure two firewalls into a HA A/P configuration. All 
of the recommended HA settings are configured. The HA1-primary and HA1 backup 
network IP and netmask are pre-configured.

Support platforms for this HA skillet:
    PA-3200
    PA-5200
    PA-7k
    
Supported PanOS versions:
    8.1.x
    9.0.x
    
**_Preparing the Firewall for HA_**
    
HA interface connections:
    1. Connect HA1-a
    2. Connect HA1-b
    3. Connect HA2 using the HSCI interface.
    
**_How to run the HASkillet:_**

FWA:
    1. Find the HASkillet Collection in the "Skillet Collections", select "Go".
    2. Select one firewall that will be FWA, click "Go"
    3. The preconfigured HA settings will be displayed for FWA. click "Submit"
    4. Enter the management IP address for the device to be FWA.
    5. Enter the Username and Password.
    6. Select the Commit Options. click "Submit" 
        - The HA configurations will be pushed to the firewall.
        - You will receive a response after the Job has been completed.
        - The "Debug" option will show you what XML commands being pushed.

FWB:
    1. Find the HASkillet Collection in the "Skillet Collections", select "Go".
    2. Select one firewall that will be FWB, click "Go"
    3. The preconfigured HA settings will be displayed for FWB. click "Submit"
    4. Enter the management IP address for the device to be FWB.
    5. Enter the Username and Password.
    6. Select the Commit Options. click "Submit" 
        - The HA configurations will be pushed to the firewall.
        - You will receive a response after the Job has been completed.
        - The "Debug" option will show you what XML commands being pushed.

After completing the two skillets above, verify the HA settings on both firewalls.     


## Support Policy
The code and templates in the repo are released under an as-is, best effort,
support policy. These scripts should be seen as community supported and
Palo Alto Networks will contribute our expertise as and when possible.
We do not provide technical support or help in using or troubleshooting the
components of the project through our normal support options such as
Palo Alto Networks support teams, or ASC (Authorized Support Centers)
partners and backline support options. The underlying product used
(the VM-Series firewall) by the scripts or templates are still supported,
but the support is only for the product functionality and not for help in
deploying or using the template or script itself. Unless explicitly tagged,
all projects or work posted in our GitHub repository
(at https://github.com/PaloAltoNetworks) or sites other than our official
Downloads page on https://support.paloaltonetworks.com are provided under
the best effort policy.
