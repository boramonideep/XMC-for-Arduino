## Documentation
Documentation of the core libraries is to be found on [this page](https://github.com/Infineon/InfineonDoxyGenerator).

## Radar Library

The radar library added in v1.2.0 replaces the old BGT library. 
### XMC1300 Sense2GoL
The library can compile on other boards than the original Sense2GoL board, if you redirect analog I/Q data by connecting the I/Q pins on the Sense2GoL board to the analog pins of another board.

## I2S Library

This library has been tested for the [Adafruit MEMS microphone breakout](https://learn.adafruit.com/adafruit-i2s-mems-microphone-breakout) with both XMC4700 relax kit and XMC1100 XMC2Go.
It also support´s Infineon's XENSIV MEMS microphone. Please refer to documentation for pin connections.

### Limitations
With XMC2Go (possibly also with other XMC1000 family devices), you might see many glitches in the sampled data. This is due to the lower speed of the microcontrollers, and you should try to reduce the I2S sampling rate.

