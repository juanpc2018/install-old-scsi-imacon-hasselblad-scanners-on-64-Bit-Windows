FR1SX Utility Disk Ver4.6
==============================================================================

  FR1SX FireWire - Ultra SCSI Converter Supplement
                                                             06 / Feb. / 2006
                                                           RATOC Systems, Inc.
                                    Copyright(C) 2000-2006 RATOC Systems, Inc.
==============================================================================


Thank you for purchasing the FR1SX.
This document contains information that supplements the "User's Manual".



<<CONTENTS>>
1.Directory Structure
2.What's new from the previous version
3.Caution when you update firmware 
  with Configuration utility version 1.4 or older 
4.FR Configuration
5.Caution when you connect the FR1SX in daisy-chain
6.RATOC Systems Technical Support


1. Directory Structure
----------------------

   This FR1SX has the following files:

 /+
 |
 +--README-E.TXT ( This file )
 |
 +--SETUP.EXE  ( FireREX1 Utility Setup )
 |
 +--Firmware
 |   +--FR0133.BIN       ( Firmware data )
 |      +--OLD FIRM
 |         +--FR0123.BIN ( OLD Firmware data )
 |
 +--Format
      +--FrFmtW9xJ.TXT   ( Formatter WinMe/98 JAPANESE README ) 
      +--FrFmtW9xE.TXT   ( Formatter WinMe/98 ENGLISH  README ) 
      +--FrFmtW9x.EXE    ( Formatter WinMe/98 Utility ) 
      +--RSFmt2XPJ.TXT   ( Formatter Win2000/XP JAPANESE README ) 
      +--RSFmt2XPE.TXT   ( Formatter Win2000/XP ENGLISH README ) 
      +--RSFmt2XP.EXE    ( Formatter Win2000/XP Utility ) 


2.What's new from the previous version
------------------------------------------------------------
  What's new from Rev 4.5 to Rev 4.6

  (1) Supports FR1SX Configuration Utility for Windows on Windows XP x64.

  What's new from Rev 4.4 to Rev 4.5

  (1) Supports FR1SX Configuration Utility for Mac OS X on Mac OS 10.2.1 - 10.4.x.
      (Require FR1SX lot2 later)
  (2) Improve Formatting Utility.

  What's new from Rev 4.3 to Rev 4.4

  (1) B'sCrew FW and B'sCrew SIM Driver removed.
      You can download from http://www.ratocsystems.com after registration.
  (2) Improve Formatting Utility.
  (3) Combine CDROM Japanese version and English version.


  What's new from Rev 4.2 to Rev 4.3

  (1) The latest firmware Version 1.33 for the FR1SX was provided.
      -Change setting SCSI ID=6, When version 1.23 is SCSI ID=0.
      -Support Minolta Film Scanner Elite F-2900   (Mac OS 9/X ).
      -Support AKAI Professional Sampler CD3000XL  (Target SCSI ID=6 setting).
      -Support Agfa DuoScan T1200, UMAX Astra1220S (Use VueScan7.5)
      -Support SCSI HDD Emulation Mode of PowerBookG3.
  (2) FR1 Utility for Mac OS 9 changed.
      -Fixed reverse setting when firmware update.


  What's new from Rev 4.1 to Rev 4.2

  (1) FR1 Unity for Mac OS 9 changed.
      The following bug was fixed:
      Writing firmware sometimes fails.
    
  (2) FR1 Utility for Mac OS X changed.
      -The FR1 Utility didn't work fine if root password was null,
       but this version fixed this bug.       
      -The FR1 Utility didn't work fine if your system was Mac OS 10.1.2,
       but this version fixed this bug.    
      -The FR1 Utility didn't work fine without drivers,
       but this version fixed it to work fine without drivers.

  (3) This version stop bundling RadiaLogic.


  What's new from Rev 4.0 to Rev 4.1

  (1) The latest firmware Version 1.23 for the FR1SX was provided.
      -The system freezed up when a bad sector data was read
       with Olympus MO MOS3381 on Mac OS X. This version fixed the bug.
      -Windows 2000 hanged up or restarted when format was executed
       to an unformatted MO media with write-protect. This version
       fixed the bug.
      -Windows 2000 freezed up or restarted when Disk Administrator
       was executed to DSC-U20GTV HDD made by Melco.
      -Write/Read error happened when a MO drive was accessed with
       IBM Think PAD i1200. This version fixed the bug.
      -The error message saying "format failed" appeared when
       a HDD was formatted with NTFS by using Disk Administrator
       on Windows 2000. This version fixed the bug.
      -The media at CD-R/RW CWR2100SX made by YAMAHA wasn't recognized
       with Writing Software Toast installed on Macintosh.
       This version fixed the bug.


  What's new from Rev 2.0 to Rev 4.0

   (1)Configuration utility FRCFGLDR version was updated to 2.1.
      We added [Max payload size] item to the advanced function
      of the FRCFGLDR.
      We fixed the following bug.
      This utility fails to detect the FR1SX on Windows 98SE/Me.

   (2)We provided the latest firmware Version 1.20
      MaxPayload can be set, using the utility.
      We fixed the following bug.
      When you play back a specific data created for QuickTime in a SCSI drive 
      connected to the FR1SX, data discrepancy happens.

   Rev 3.0 is exclusive use for Macintosh. Windows version isn't available.

   What's new from Rev 1.1 to Rev 2.0

   (1)We provided an installer for each utility.
      Each utility will be installed in the hard drive by the installer. 

   (2)The file name of the Configuration utility was changed from
      FRCFGUTY.EXE to FRCFGLDR.EXE.

   (3)We added update function to FRCFGLDR.
      With this update function, you can update the old firmware in the FR1SX.
   (4)We provided the latest firmware.( FR0114.BIN Version 1.14 )
   (5)We added the advanced function to FRCFGLDR.



   What's new from Rev 1.0 to Rev 1.1

   (1)With this version, you can run FRCFGUTY on Windows Me.
   (2)Version of Frfmtw9x.exe is changed to 2.65.
      We fixed the following bug in the Frfmtw9x.exe for Windows Me/98/95.
      
      An error happens to VAIO PCs made by SONY with memory stick slot.



3.Caution when you update firmware 
  with Configuration utility version 1.4 or older 
-----------------------------------------------------------------------

   Before you update it, you have to delete the following files if older 
   configuration utility is installed in your hard drive.

   FRCFGUTY.EXE   ( FRCFGUTY )
   FRCFGLDR.SYS   ( Driver for the FRCFGUTY.EXE )
   FRCFGLDR.INF   ( INF file for the FRCFGLDR.SYS )
   FRCFGLDR.DLL   ( DLL for the FRCFGUTY.EXE )

   After deleting these files, double click on the SETUP.EXE.



4.FR Configuration
-------------------
      
   4-1. How to start/finish [FR Configuration] on Windows Me/98.

        (1)Click on the removal icon on the taskbar with left button.
        (2)When the message box saying [Stop IEEE1394....] shows up,
           select it.
        (3)When the message box saying [You can safely remove the FR1SX] shows up,
           click [OK] and remove the IEEE1394 cable from the FR1SX.
        (4)Click [Start] and select [Programs] - [RATOC FireWire Utility] -
           [FR Configuration]. FR Configuration starts up.
        (5)When the message box saying [Can't find FireREX1/FR1SX. Connect FireREX1
           /FR1SX now.] shows up, reconnect the IEEE1394 cable to the FR1SX.
           When you forgot to remove the IEEE1394 cable at the step (3),
           the message box saying [Now you should reconnect FireREX1/FR1SX] 
           shows up.
           In this case, remove the IEEE1394 cable from the FR1SX and reconnect
           the IEEE1394 cable. And click [OK].
        (6)The FR1SX main window will show up. Confirm the status line says
           Setting Success.
        (7)If you can find the Setting Success message, the FR1SX is ready to 
           work.

           For detailed information on this utility, refer to 4-3.Config Utility
           , 4-4.Advanced, 4-5.Firmware update utility.

        (8)After you finish configuration, click [Exit] to finish this utility.


   4-2. How to start/finish [FR Configuration] on Windows XP/2000.

        (1)Click on the removal icon on the taskbar with left button.
        (2)The message box saying [Stop RATOC Systems_Inc, IEEE1394-SCSI-3
           IEEE1394 SBP2 Device - Drive(X:)] will show up.
           Select it.
        (3)When the message box saying [You can safely remove the FR1SX] shows up,
           click [OK] and remove the IEEE1394 cable from the FR1SX.
        (4)Click [Start] and select [Programs] - [RATOC FireWire Utility] -
           [FR Configuration]. FR Configuration starts up.
        (5)When the message box saying [Can't find FireREX1/FR1SX. Connect FireREX1
           /FR1SX now.] shows up, reconnect the IEEE1394 cable to the FR1SX.
           When you forgot to remove the IEEE1394 cable at the step (3),
           the message box saying [Now you should reconnect FireREX1/FR1SX]
           shows up.
           In this case, remove the IEEE1394 cable from the FR1SX and reconnect
           the IEEE1394 cable. And click [OK].
        (6)When you start the FR Configuration utility for the first time,
           [Found New Hardware Wizard] will show up.
           In this case, go ahead by just clicking [Next] and click [Finish]
           at the last dialog box.

        (7)Click [Start] and select [Programs] - [RATOC FireWire Utility] -
           [FR Configuration] once again. The FR1SX main window will show up. 
           Confirm the status line says Setting Success.
        (8)If you can find the Setting Success message, the FR1SX is ready to 
           work.

           For detailed information on this utility, refer to 4-3.Config Utility
           , 4-4.Advanced, 4-5.Firmware update utility.

        (9)After you finish configuration, click [Exit] to finish this utility.
        (10)Restart Windows 2000.


   4-3. Config Utility
                
        (1)Select [Config Utility] on the main window.
        (2)You can configure [Transfer Mode] on this Config Utility dialog box.
           You can select the following values in the Transfer Mode.
        
           [Transfer Mode] <Default value:20MB/sec.>  
            You can select 20MB/sec., 10MB/sec., 5MB/sec., Async.
    
            If you need more detailed settings, you have to click [Advanced].
            In this case, refer to 4-4.Advanced.

        (3)After you selected new setting, click [Back] to go back to the main 
           window.
        (4)Click [Write] for your setting to take effect.


   4-4.Advanced

        (1)Select [Config Utility] on the main window.
        (2)Config Utility dialog box will show up. Click [Advanced].
           Advanced setting dialog box will show up.
        (3)After you finish configuration, click [BACK] to the main window.
        (4)Then, click [Write] for your setting to take effect.

           Advanced setting dialog box has the following settings.

           [Target SCSI ID] < Default value:AUTO >
             You can set target SCSI ID No.

           [Enable parity check] < Default value:Enable >
             You can set parity check enable or disable.

           [Delay time between power on and SCSI bus reset] 
           < Default value:0 sec >
             You can set delay time for some SCSI devices which
             hangs up if SCSI bus reset is issued right after the FR1SX gets 
             powered.

           [Delay time between SCSI bus reset and SCSI command] 
           < Default value:1 sec >
             You can set delay time for some SCSI devices which
             hangs up if SCSI command is issued right after SCSI bus resets.

           [Delay time until 1394 transaction start] < Default value:4 sec >
             You can delay time for some SCSI devices which
             will not receive any command if a next command is issued right 
             after Start/Stop Unit command is issued.

           [Enable SCSI bus reset] < Default value:Enable >
             You can set whether the FR1SX issues SCSI bus reset to a SCSI 
             device or not.

           [Enable START UNIT command] < Default value:Disable >
             You have to enable START UNIT command for some SCSI devices which
             will not work if they does not receive this START UNIT command.

           [Max Payload Size] <Default value:1024>
             You can set Max Payload Size on FireWire.
             If you connect IEEE1394 Hub ASB-H048 made by ADTX, set 1024 or 512.
             If you set 2048, an error happens.


   4-5.Firmware update utility

        (1)Select [Firmware update utility] on the main window.
        (2)Firmware update utility dialog box will show up.
           The top line shows firmware data and path.
        (3)If you want to change the data,click [Browse] to select another file.
        (4)If you selected new firmware data, click [Write] to write the new 
           firmware.


5.Caution when you connect the FR1SX in daisy-chain
----------------------------------------------------

   When you connect the FR1SX in daisy-chain, you have to connect
   another FR1SX or IEEE1394 cable in daisy-chain when the FR1SX is NOT
   being accessed. If you ignore this caution, we don't guarantee
   the FR1SX works fine.



6.RATOC Systems Technical Support
----------------------------------

 We have a Tech-support staff in USA. If you need our assistance,
 please contact us by e-mail or phone.

      RATOC Systems International, Inc. Tech-Support.
      2000 Wyatt drive
      Suite 9
      Santa Clara, CA 95054

      Open  9:30AM to 5:00PM(PST)  Monday through Friday.

      Phone : (408)986-9040
      Fax   : (408)986-9042
      E-mail: http://www.ratocsystems.com/english/contact/support.html
      URL   : http://www.ratocsystems.com/english

(NOTE)
  Please include the information below to help us to assist you
  in your Tech-Support Question

  * Our product name and product description
  * Host computer name
  * Application software/driver version

END OF FILE
