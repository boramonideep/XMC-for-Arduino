# Notes: XMC 2Go

The XMC microcontroller series has implemented the [USIC](https://www.infineon.com/dgdl/Infineon-USIC-XMC1000_XMC4000-AP32303-AN-v01_00-EN.pdf?fileId=5546d4624e765da5014ed93960ae3391) module for communication peripherals, e.g. I²C, UART, SPI, etc.

Flexibly by software running on the microcontroller, you are able to configure it almost arbitrarily regarding these interfaces.
However, different series of the XMC microcontrollers have different amount of USIC modules, e.g. the XMC1100 has one USIC module while the XMC4700 series has many more. 
As every USIC module supports two independent sub-modules, one module can provide two independent channels, e.g. I²C mixed with UART or two independent I²C channels.

# Notes for XMC 2Go
The XMC 2Go has the XMC1100 microcontroller implemented. More information related to the board can be found in the [XMC 2Go](https://www.infineon.com/dgdl/Board_Users_Manual_XMC_2Go_Kit_with_XMC1100_R1.0.pdf?fileId=db3a3043444ee5dc014453d6c75078c6).

Not all interfaces (SPI, I²C, UART) shown in the picture of the [XMC 2Go pinout](https://github.com/Infineon/Assets/raw/master/Pictures/XMC%202Go_PO.jpg) can be used simultaneously. Especially, the USB UART is designed to other pins as the PCB pins, i.e. it's not possible to connect external UART to the board via any pin and forward it to the USB shared UART (it's a J-Link enabled UART port by the[XMC4200 based debugger](https://www.infineon.com/dgdl/Infineon-XMC_Link_Board_Users_Manual.pdf-UM-v01_00-EN.pdf?fileId=5546d462518ffd850152451695e45edc)). 
Therefore, one needs to set up a software bridge between both channels which makes use of other communication interfaces impossible (XMC1100 has one USIC interface with two channels, i.e. only I²C and UART can be used simultenaeosly by peripheral hardware). 
However, you are able to switch between both UART interfaces by hardcoding as shown below, but please keep in mind that you will not receive anything via the PC console as everything is handled by the on-board UX/RX UART interface. 
If you need help, please rise an issue and we will help you directly.    

- By default serial communication (UART) uses pin P2.1 and P2.2, which enables the connection to the host PC. (Serial Monitor)
If you want to use the on-board Rx and Tx Pins (P2.6 and P2.0), you have to change the "pins_arduino.h" file under:

XMC-for-Arduino / arm / variants / XMC1100 / config / XMC1100_XMC2GO /

In this file you have to uncomment line 186 and comment line 185, which will change the configuration of the UART Pins.

Be Aware, that you can only use either the on-board Pins or the Pins connected to the Host PC.

BR