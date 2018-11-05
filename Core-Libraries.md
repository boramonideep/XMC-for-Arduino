## Documentation
Documentation of the core libraries is to be found on [this page](https://github.com/Infineon/InfineonDoxyGenerator).

## Radar Library

The radar library added in v1.2.0 replaces the old BGT library. 
### XMC1300 Sense2GoL
The library can compile on other boards than the original Sense2GoL board, if you redirect analog I/Q data by connecting the I/Q pins on the Sense2GoL board to the analog pins of another board.

## I2S Library

This library has been tested with the IM69D130 Microphone Shield2Go with both XMC4700 Relax Kit and XMC1100 XMC2Go. Please refer to the [README.md](https://github.com/Infineon/XMC-for-Arduino/blob/master/arm/libraries/I2S/README.md) of the I2S library for pin connections.

### Limitations
With XMC 2Go (possibly also with other XMC1000 family devices), you might easily overflow the I2S buffer and you should try to reduce the I2S sampling rate if so.

