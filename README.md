# Sonnet-Tempo-Dual-SATA-6Gbps
FW Upgrade procedure for:  
https://www.sonnettech.com/product/tempossd.html

Original Firmware 2019:
https://www.sonnettech.com/support/downloads/software/tempossdfwupdater100.zip

installer is a FreeDOS compressed image in a .iso
There are 2 options:
Option A)
Burn .iso to a CD-R or CD-RW, will Boot OK.

Option B) 
Download Rufus,
open .iso with WinRAR,
Extract .img file,
Burn IMG file to empty USB pen drive.
USB Pen Drive will be NOT Bootable.
after reboot will allow to see the files.

create another Empty Bootable FreeDOS USB pen drive.
move / copy files from Non-Bootable to Bootable USB.

Original Firmware 2019:

Asmedia 106x SATA Controller Ver 1.50 AHCI Mode

Copyright (C) Asmedia Technologies, Inc. All Right reserved.

S.M.A.R.T. Supported

Using PCIE Gen 2 x2

Firmware version: 160120_10_4E_01

------

Latest Firmware i could find 2021:

Asmedia 106x SATA Controller Ver 1.80 AHCI Mode

Copyright (C) Asmedia Technologies, Inc. All Right reserved.

S.M.A.R.T. Supported

Using PCIE Gen 2 x2

Firmware version: 210906_00_76_01

https://www.station-drivers.com/index.php/en/outils/Drivers/Asmedia/ASM-106x-Sata-6G-Controller/Firmwares/Asmedia-ASM-106x-R-Sata-6G-Controller-Firmware-Version-210906.00.76.01/lang,en-gb/

RAID Manager:
https://www.station-drivers.com/index.php/en/driverss/Drivers/Asmedia/ASM-106x-Sata-6G-Controller/Utilities/lang,en-gb/

Drivers:
https://www.station-drivers.com/index.php/en/outils/Drivers/Asmedia/ASM-106x-Sata-6G-Controller/Drivers/Asmedia-ASM-1x6x-Sata-6G-controller-Drivers-Version-3.3.5.0-WHQL/lang,en-gb/

Asmedia Station-Drivers page:
https://www.station-drivers.com/index.php/en/driverss/Drivers/Asmedia/ASM-106x-Sata-6G-Controller/lang,en-gb/

Option C)
Extract the 210906.zip
copy files to Bootable FreeDOS USB pen drive,
type AHCI.bat
or 
spiupd.exe /U 0076_01.ROM

WARNING 1:
Upgrade cannot be done in Windows.

WARNING 2:
Unscrew & Remove SSDs BEFORE doing the FW Upgrade.

Upgrade works ok so far.
Feels much faster in Windows8.1x64

No driver install needed.

With Original FW had a strange Hiccup.

Why Sonnet Tempo Dual SATA PCIe card?
its a poor man Dual U.2

8TB QLC SSD from Samsung or Micron are almost half the $ of 8TB M.2
Dual M.2 is More $$ than Dual SATA.
The only advantage of M.2 is that there is 8xM.2 PCIe cards, but are very $$$$... 
HighPoint PCIe v4.0, PCIe v3.0, 
Sonnet 4xM.2 PCIe,
OWC 8xM.2 dont have Hardware RAID Controller, thats why the lower price.

2xSSD 6Gbps 8TB is the cheapest option for Solid State drive with 16TB total capacity.
M.2 tech is a lot Faster but price is double or more for same 16TB.
U.2 is Top of the Line, Cutting Edge Technology, High End $$$.
