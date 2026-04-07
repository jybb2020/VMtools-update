# VMtools-update
Bat script to update the VMtools 


This script is designed to update the vmtools drivers update via common network path 

Pre requisties

1.The network path is to be accessable via the client devices,and authurized services accounts
2.Ensure the Proper Downtime of the devices as while the .bat exec the client device is rebooted.
3.saved the text file in the format of .bat and make it use as Group Policy or directly via executing.
4.This can be used  for any .exe file update ,ensure the path and name of the  file is updated


Key Benefits

✅ No ISO mounting required on individual servers
✅ Centralized management of VMware Tools installer
✅ Reduced operational effort and execution time
✅ Can be scheduled, enabling unattended updates
✅ Consistent version deployment across all servers
✅ Works even where vCenter-based upgrades are restricted
=============================================================================
How It Works (High-Level Flow)

VMware Tools installer EXE is placed in a common SAN/shared folder
The BAT script:

Connects to the shared folder
Copies the installer locally (optional but recommended)
Executes the VMware Tools installer in silent mode


The update runs without user interaction


To download old versions : https://packages.vmware.com/tools/releases/
To download latest version : https://packages.vmware.com/tools/releases/latest/windows/
