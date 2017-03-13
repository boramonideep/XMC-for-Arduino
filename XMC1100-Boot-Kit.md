# Overview
This pages summarizes information about the XMC1100 Boot Kit evaluation board and its implementation for the Arduino IDE. The XMC1100 Boot Kit board consists of a XMC1100 microcontroller with a debugger implemented by a XMC4200 microcontroller. The Infineon homepage of the board can be found [here](https://www.infineon.com/cms/en/product/evaluation-boards/KIT_XMC11_BOOT_001/productType.html?productType=db3a30443b360d0e013b8f5163c46f62#ispnTab1).

# Arduino Pin Out
The pin layout of the XMC 2Go for the Arduino IDE is as follows (the original file can be found [here](https://github.com/Infineon/Assets/blob/master/Pictures/XMC%201100_BootKit_PO.jpg)):

![XMC 2Go Pin Out for Arduino](https://github.com/Infineon/Assets/blob/master/Pictures/XMC%201100_BootKit_PO.jpg)

# Key Features
* XMC1100 Microcontroller (ARM® Cortex™-M0 based) in TSSOP-38 with 64 KB Flash and full peripheral set of XMC1100 series
* Detachable Segger J-Link (implemented with XMC4200)
* Board shape & power supply for Arduino shields: [Shield List](http://shieldlist.org).
* [Infineon shields](https://www.infineon.com/cms/en/product/microcontroller/32-bit-industrial-microcontroller-based-on-arm-registered-cortex-tm-m/xmc-development-tools-kits-and-boards/boards-and-shields-for-arduino/channel.html?channel=5546d4614b0b239c014ba1e6c4a73098) - Hardware compatible with Arduino

# PCB Design Data
In case you want to change the design or reuse it for your own projects, please find the XMC 2Go board design for EAGLE under the following link:

[XMC1100 Boot Kit PCB Design Data](https://www.infineon.com/dgdl/PCB_XMC1100_CPU_Card_V2.zip?fileId=db3a30433da119ff013da23921f61425&sd=t)

# Board Information, Datasheet and Additional Information
A PDF summarizing the features and layout of the XMC 2Go board is stored on the Infineon homepage [here](https://www.infineon.com/dgdl/Board_Users_Manual_XMC1100_CPU_Card_R2.pdf?fileId=db3a30433da119ff013da232476b1416).
The datasheet for the XMC1100 can be found here [XMC1100 Datasheet](https://www.infineon.com/dgdl/Infineon-xmc1100-DS-v01_04-EN.pdf?fileId=5546d46255dd933d0155e31763e577dc) while the respective reference manual is located here [XMC1100 Reference Manual](https://www.infineon.com/dgdl/Infineon-xmc1100-AA_rm-UM-v01_01-EN.pdf?fileId=5546d46255dd933d0155e31753b077af).

