# Sonnet-Tempo-Dual-SATA-6Gbps </br>

FW Upgrade procedure for:  </br>
https://www.sonnettech.com/product/tempossd.html </br>
http://ableconn.com/support_1.php?gid=120 </br>
https://www.startech.com/en-us/cards-adapters/10p6g-pcie-sata-card </br>

Latest Firmware [220916_00_00_00 A23](http://ableconn.com/upload/ASM1062-FW_220916-RE1062.A23.zip)
[Original Firmware 160120... (2019)](https://www.sonnettech.com/support/downloads/software/tempossdfwupdater100.zip) </br>
older 190... Firmware had problems booting with Dosdude OSX Catalina installer, when SSD was installed in 1 machine and moved to another </br>
installed in: MacMini 2014 and SSD moved to a MacPro 5,1 2010 with latest FW 144.0.0.0.0 </br>

Original installer is a FreeDOS compressed image in a .iso </br>

There are Options: </br>

Option A) </br>
Burn .iso to a CD-R or CD-RW, will Boot OK. </br>
Remove SSDs Before doing the Upgrade. </br>

Option B)  </br>
Download [rufus.ie](https://rufus.ie) </br>
open .iso with WinRAR </br>
Extract .img file, </br>
Burn IMG file to empty USB pen drive. </br>
USB Pen Drive will be NOT Bootable. </br>
after reboot will allow to see the files. </br>

Option C)  </br>
create an Empty Bootable DOS USB pen drive. </br>
Rufus creates a Windows Millenium DOS disk </br>
if want FreeDos or MS-DOS 6.22 requires to [download .img](https://www.allbootdisks.com/download/dos.html)  </br>
move / copy files from Non-Bootable to Bootable USB. </br>

Original Firmware 2019 displayed on a PC, </br>
Not displayed on a MacPro5,1 Apple Boot, maybe in Verbose Mode Boot. </br>
```
Asmedia 106x SATA Controller Ver 1.50 AHCI Mode </br>
Copyright (C) Asmedia Technologies, Inc. All Right reserved. </br>
S.M.A.R.T. Supported </br>
Using PCIE Gen 2 x2 </br>
Firmware version: 160120_10_4E_01 </br>
```

------

Firmware 2021: </br>
```
Asmedia 106x SATA Controller Ver 1.80 AHCI Mode </br>
Copyright (C) Asmedia Technologies, Inc. All Right reserved. </br>
S.M.A.R.T. Supported </br>
Using PCIE Gen 2 x2 </br>
Firmware version: 210906_00_76_01 </br>
```

-----

Firmware 2022: </br>
```
Asmedia 106x SATA Controller Ver 1.80 AHCI Mode </br>
Copyright (C) Asmedia Technologies, Inc. All Right reserved. </br>
S.M.A.R.T. Supported </br>
Using PCIE Gen 2 x2 </br>
Firmware version: 220916_00_00_00 </br>
```

-----

https://www.station-drivers.com/index.php/en/outils/Drivers/Asmedia/ASM-106x-Sata-6G-Controller/Firmwares/Asmedia-ASM-106x-R-Sata-6G-Controller-Firmware-Version-210906.00.76.01/lang,en-gb/ </br>

RAID Manager: </br>
https://www.station-drivers.com/index.php/en/driverss/Drivers/Asmedia/ASM-106x-Sata-6G-Controller/Utilities/lang,en-gb/ </br>

Drivers: </br>
https://www.station-drivers.com/index.php/en/outils/Drivers/Asmedia/ASM-106x-Sata-6G-Controller/Drivers/Asmedia-ASM-1x6x-Sata-6G-controller-Drivers-Version-3.3.5.0-WHQL/lang,en-gb/ </br>

Asmedia Station-Drivers page: </br>
https://www.station-drivers.com/index.php/en/driverss/Drivers/Asmedia/ASM-106x-Sata-6G-Controller/lang,en-gb/ </br>

Option D) </br>
Extract the 210906.zip </br>
copy files to Bootable FreeDOS USB pen drive, </br>
type AHCI.bat </br>
or  </br>
> spiupd.exe /U 0076_01.ROM </br>

### WARNING #1: </br>
Upgrade cannot be done in Windows. </br>

### WARNING #2: </br>
Unscrew & Remove SSDs BEFORE doing the FW Upgrade. </br>

### WARNING #3: </br>
Booting UEFI-CSM OS MBR, sometimes works, most of the times do Not. </br>

Upgrade works so far. </br>
Feels much faster in Windows8.1x64 </br>

No driver install needed. </br>
With Original FW had a strange Hiccup with Crucial Tech MX500 2TB SSD. </br>

Why Sonnet Tempo Dual SATA PCIe card? </br>
economic version of the Dual U.2 </br>

8TB QLC SSD from Samsung or Micron or Intel are almost half the price$ of 8TB M.2 NVMe </br>
Dual M.2 is Faster. but... also More $$ than Dual SATA. </br>
The advantage of M.2 PCIe is that there are 8xM.2 PCIe cards, but are $1k usd. </br>
HighPoint PCIe v4.0, PCIe v3.0,  </br>
Sonnet 4xM.2 PCIe, </br>
Adwits 4xM2, </br>
Startech or Ableconn 2xM.2 PCIe </br>
OWC 8xM.2 dont have Hardware RAID Controller, thats why has lower price. </br>

2xSSD 6Gbps 8TB each, is the cheapest option for Solid State drive storage, with 16TB capacity. </br>
M.2 is Faster but current price is double or more for the same 16TB QLC. </br>
for storage: near 500MB/s is good enough. </br>
Large 18TB HDD Seagate Exos are 250MB/s for lower price. </br>
U.2 is Top of the Line, Cutting Edge Technology, High End $$$. </br>

IF drives are Turned-On 24/7, SSD is much more power efficient. </br>
vs. 3.5" Mechanic HDD. </br>
HDD require Spin-Down every 30min, </br>
and each Spin-Up requires 12v 3A-5A Peak. </br>
Multiple HDDs when Spin-Up all at same time its a very Big Peak load for the PSU. </br>
Large HDD arrays require 80 Plus Titanium to be cost effective. </br>
https://en.wikipedia.org/wiki/80_Plus </br>

IF you spin-down / up too often, will wear and damage everything, the PSU, the HDD motor, power cables if does Not have enough AWG, etc... </br>
IF you dont spin down HDDs enough time, bearings will wear & fail sooner, will overheat, electronics will fail, etc... </br>

All require proper cooling. </br>
