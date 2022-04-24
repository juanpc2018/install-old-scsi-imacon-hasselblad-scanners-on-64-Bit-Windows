# install-old-scsi-imacon-hasselblad-scanners-on-64-Bit-Windows

You need Hasselblad FlexColor 4.0.3 thats the latest version that supports SCSI scanners.
after installing,
The 32-Bit .INF driver is located on C:/Program Files (32-Bit)/Hasselblad/INF
That driver is for 32-Bit Only, Does Not work.
requires a small modification to allow Windows Imagine Devices to Detect the Driver in 64-Bit Windows. 

Tested:
XP 64-Bit
Vista 64-Bit
Windows7 64-Bit
Windows 8.1 64-Bit
Windows 10 64-Bit
Windows 11 untested.

Problem #1.
modified Driver here is Not signed,
Wont install.

To solve that problem:
1. Reboot Windows in Advanced Mode to Disable Driver Signature Enforcement Requirement.

Windows 8.1 procedure, similar for W10:
PC Settings.
Update & Recovery.
Recovery.
Advanced Startup.
Reboot Now.
A New screen will appear at boot.
Select Option 7 or F7

Then Windows will boot normally,
right click in Windows Logo in taskbar.
click Device Manager
Select the SCSI device usually with a Yellow Triangle,
requires the SCSI scanner connected and Turned-ON.
If Using ATTO UL5D PCIe card, requires to be turned-on since PC is turned-On,
latest drivers for OSX here:
https://macintoshgarden.org/apps/atto-ul4x-and-ul5x-scsi-ultra-320-drivers
https://www.macintoshrepository.org/33038-atto-ul4x-and-ul5x-scsi-ultra-320-drivers
Latest UL5D configtool & Firmware for Windows & Linux
https://members.driverguide.com/driver_search.php

ATTO is more advanced, has many more options to configure,
ATTO UL5D has 2x Port VHDCI 68-pin "0.8mm pin",
Imacon Scanners are Centronics 50-pin Female, and has a small SCSI ID rotary switch on the back.
require an Special Cable from VHDCI to Centronics 50-pin Male,
3feet or 6 feet, SCSI has limited distance.
http://www.granitedigital.com/688mmvhdm-50centm3.aspx
http://www.granitedigital.com/688mmvhdm-50centm6.aspx

SCSI Scanners Require an Active or Passive Centronics SCSI 50-pin Male terminator device.
The best made were Granite Digital Part Number 7359
http://www.granitedigital.com/50pincentronicsm.aspx
http://www.granitedigital.com/scsispecsheet.aspx

Ratoc is almost Plug´n Play, very easy to configure.
has HD50 Male, requires HD50-Female to Centronics 50-Pin Male adapter/converter.
http://www.granitedigital.com/50fmicrodto50mcentronics.aspx
SCSI Terminator, and Firewire Cable 6-6 "400-400" or 9-6 "800-400"

IF Using the Ratocsystems FireWire to SCSI adapter FireREX1 or FS1SX
Firmware 1.23 1.32 or 1.36
can be used with FireWire800 9-pin to FireWire400 6-pin cable.
Some old laptops have Firewire 4-pin to 6-pin untested.

Ratoc SCSI converter or ATTO SCSI PCIe must be configured to be Async, Not Sync 5MB-10MB-20MB-40MB.
Scanners are Async.

The Free Ratoc Configurator Tool for PowerMac G4 works in OSX SnowLeopard 10.6.8 for intel with Rosetta PPC CPU emulator if installed.
also Ratoc has a Free config tool for WindowsXP 32-Bit, 64-Bit untested.

There is an optional paid Config Tool $20usd. in the Japan Ratoc web store. 
English website store is broken,

To purchase the optional config tool + 1.36 FW.
requires Website translator, Chrome or browser.Yandex.com 
Select Standard Ground Shipping and will give automatically a Download Link.
Japanese websites are strange.

The Optional paid config tool + Firmware 1.36 its designed for Windows Vista Only, 
does Not work in Windows8.1 64-Bit, using Vista compatibility installs, runs, but does Not detect the Scsi converter, gives error.
Windows7 64-Bit untested, but probaly wont work.
Optional paid Config Tool is Vista Only.

The 1.36 Firmware vs. Free 1.32 or 1.23 is the aditional support for Power Management Stand-By feature for FireWire introduced in Vista.
Older FirmWare does Not have that, FireWire Power is Always ON.

Install Driver in Windows8.1 from Device Manager,
Select Have a Disk,
will ask what kind of Driver is...
select Image Devices.
Should be a Imacon or Hasselblad manufacturer, but Not the Scanner 343, Photo, 646, Precision II, Precision III, etc...
choose disk...
Download this .inf file
search x64.INF in your download folder
select proper Scanner from List.
Reboot,
DONE.

FlexColor 4.0.3 should detect the scanner at start-up,
but scanner must be Turned-On before opening the FlexColor Software,
at least 3 minutes, to allow Imacon scanner to Boot, or FlexColor Software wont detect it.
Imacon Photo scanner has a 386sx CPU, with 4MB of RAM.
cant remember the Speed 20MHz, 33MHz?
Anyway, it needs time to boot.

Software options should be different,
Default options are for Digital Cameras.
Scanner Serial ID should be in Devices Menu in FlexColor 4.0.3 SW.

2. Set Windows in Test mode, to Allow Test Signed Driver.
bcdedit /set testsigning on
But this method only works with TestSigned drivers.
This driver is Old XP era, probably this method wont work.


