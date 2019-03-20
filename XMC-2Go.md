# Overview
This pages summarizes information about the XMC 2Go evaluation board and its implementation for the Arduino IDE. The XMC 2Go board consists of a XMC1100 microcontroller with a debugger implemented by a XMC4200 microcontroller. The Infineon homepage of the board can be found [here](https://www.infineon.com/cms/de/product/evaluation-boards/KIT_XMC_2GO_XMC1100_V1/productType.html?productType=db3a304443537c4e01436ccecb5d154f#ispnTab9).

# Changes
The release V1.1.0 changed the pin out: MISO and MOSI have been swapped to ensure compatibility with additional existing boards, please compare pin out diagram for changes.
* MISO is now pin 0
* MOSI is now pin 1

# Arduino Pin Out
The pin layout of the XMC 2Go for the Arduino IDE is as follows (the original file can be found [here](https://github.com/Infineon/Assets/blob/master/Pictures/XMC%202Go_PO.jpg)):

![XMC 2Go Pin Out for Arduino](https://github.com/Infineon/Assets/blob/master/Pictures/XMC%202Go_PO.jpg)

# Key Features
* XMC1100 (ARM® Cortex™-M0 based)
* On-board J-Link Lite Debugger (implemented with XMC4200)
* Power over USB (Micro USB) or 3.3 V pin possible
* ESD and reverse current protection
* 2 user LEDs
* Pin Header 2x8 Pins suitable for Breadbord
* Ultra-small evaluation board (38,5 mm x 14 mm)

# PCB Design Data
In case you want to change the design or reuse it for your own projects, please find the XMC 2Go board design for EAGLE under the following link:

[XMC 2Go PCB Design Data](https://www.infineon.com/dgdl/PCB_Sources_XMC_2Go_Kit_with_XMC1100-V1.zip?fileId=db3a3043444ee5dc014453d9d14f78cb&sd=t)

# Board Information, Datasheet and Additional Information
A PDF summarizing the features and layout of the XMC 2Go board is stored on the Infineon homepage [here](https://www.infineon.com/dgdl/Board_Users_Manual_XMC_2Go_Kit_with_XMC1100_R1.0.pdf?fileId=db3a3043444ee5dc014453d6c75078c6).
The datasheet for the XMC1100 can be found here [XMC1100 Datasheet](https://www.infineon.com/dgdl/Infineon-xmc1100_AB-DS-v01_08-EN.pdf?fileId=5546d4624a0bf290014a4bdaff9325bd) while the respective reference manual is located here [XMC1100 Reference Manual](https://www.infineon.com/dgdl/Infineon-xmc1100-AA_rm-UM-v01_01-EN.pdf?fileId=5546d46255dd933d0155e31753b077af).

