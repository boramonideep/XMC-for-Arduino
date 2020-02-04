## wiring_analog after V1.2.1
Analog functions like analogRead and 
analogWrite etc. have changed after V1.2.1 to have extra safety measures to ensure invalid settings cannot be done and report errors.

Additionally extra getter functions have been added so other libraries can access the resolution of read and write functions as number of bits and current maximum value possible.

## Extra functions
These functions return the analog resolution as number of bits
* uint8_t getAnalogReadBits( ) - range 8 to 12
* uint8_t getAnalogWriteBits( ) - range 8 to 16

These functions return the analog resolution as its maximum value
* uint16_t getAnalogReadMaximum( ) - range 255 to 4095
* uint16_t getAnalogWriteMaximum( ) - range 255 to 65535

## Default Values
Read resolution default is 10 bits (0 to 1023)

Write resolution default is 8 bits (0 to 255)
## Error and Return Codes by Function
Where possible functions do **NOT** action invalid parameters passed in.

Functions return error codes or valid values so be sure which error code you are looking for as some functions can return 0 as a valid value (e.g. analogRead) so an out of range value is returned instead.
<table align=centre border=0>
 <tr>
  <td><b>Function</b></td>
  <td><b>Valid Return</b></td>
  <td><b>Errors</b></td>
 </tr>
 <tr>
  <td>analogReadResolution</td>
  <td>8 to 12<br>as passed in</td>
  <td>255</td>
 </tr>
 <tr>
  <td>getAnalogReadBits</td>
  <td>8 to 12</td>
  <td> none</td>
 </tr>
 <tr>
  <td>getanalogReadMaximum</td>
  <td>255 to 4095</td>
  <td>none</td>
 </tr>
 <tr>
  <td>analogWriteResolution</td>
  <td>8 to 16<br>as passed in</td>
  <td>255</td>
 </tr>
 <tr>
  <td>getAnalogWriteBits</td>
  <td>8 to 16</td>
  <td> none</td>
 </tr>
 <tr>
  <td>getanalogWriteMaximum</td>
  <td>255 to 65535</td>
  <td>none</td>
 </tr>
 <tr>
  <td>analogRead</td>
  <td>0 to Maximum for Resolution </td>
  <td>0xFFFFFFFF usually invalid channel</td>
 </tr>
 <tr>
  <td>analogWrite</td>
  <td>0 success </td>
  <td>-1 = invalid value<br>
      -2 = wrong pin</td>
 </tr>
 <tr>
  <td>setAnalogWriteFrequency</td>
  <td>0 success </td>
  <td>-1 = invalid frequency<br>
      -2 = wrong pin</td>
 </tr>
</table>
This should enable checks in software for valid operation and debugging problem code.

[Home](https://github.com/Infineon/XMC-for-Arduino/wiki)