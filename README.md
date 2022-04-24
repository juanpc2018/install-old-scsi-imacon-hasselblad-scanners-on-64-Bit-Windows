# install-old-scsi-imacon-hasselblad-scanners-on-64-Bit-Windows

The 32-Bit .INF file has a small modification to allow Imagine Devices to Detect the Driver in 64-Bit. 

Works in Windows7 64-Bit, 
Windows 8.1 64-Bit
Windows 10 64-Bit,
Windows 11 untested.

Problem #1.
Driver is Not signed. WHQL

To solve that problem:
1. Reboot Windows in Advanced Mode to Disable Driver Signature Enforcement Requirement.

Windows 8.1 procedure:
PC Settings.
Update & Recovery.
Recovery.
Advanced Startup.
Option 7 or F7

Device Manager,
Select the SCSI device usually with a Yellow Triangle.

Install Driver from Select Disk,
search .INF driver
will ask what kind of Driver is...
select Image Devices.
Should be a Imacon or Hasselblad manufacturer,
or choose disk...
select proper Scanner from List.
Reboot,
DONE.

2. Set Windows in Test mode, to Allow Test Signed Driver.
bcdedit /set testsigning on
But this option only works with TestSigned drivers.

This driver is Old XP era.


