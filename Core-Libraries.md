## Documentation
Documentation of the core libraries is to be found on [this page](https://github.com/Infineon/InfineonDoxyGenerator).

## Radar Library

The radar library added in v1.2.0 replaces the old BGT library. 
### XMC1300 Sense2GoL
The library can compile on other boards than the original Sense2GoL board, if you redirect analog I/Q data by connecting the I/Q pins on the Sense2GoL board to the analog pins of another board.

## I2S Library

This library has been tested for the [Adafruit MEMS microphone breakout](https://learn.adafruit.com/adafruit-i2s-mems-microphone-breakout) with both XMC4700 relax kit and XMC1100 XMC2Go.
It will also support Infineon's XENSIV MEMS microphone. Please refer to documentation for pin connections.

### Limitations
As a preliminary version, it works well with the XMC4700 relax kit; with XMC2Go, however, if conditions need to be added in order to filter out the glitches in the raw data.

