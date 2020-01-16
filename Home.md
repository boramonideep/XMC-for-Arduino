# Welcome
Welcome to the XMC-for-Arduino wiki! You'll find information about the currently supported boards ([XMC1100 XMC2Go](https://github.com/Infineon/XMC-for-Arduino/wiki/XMC-2Go), [XMC1100 H-Bridge 2Go](https://github.com/Infineon/XMC-for-Arduino/wiki/XMC1100-H%E2%80%90Bridge-2Go), [XMC1100 Boot Kit](https://github.com/Infineon/XMC-for-Arduino/wiki/XMC1100-Boot-Kit), [XMC1300 Boot Kit](https://github.com/Infineon/XMC-for-Arduino/wiki/XMC1300-Boot-Kit), [XMC1300 Sense2GoL](https://github.com/Infineon/XMC-for-Arduino/wiki/XMC1300-Sense2GoL), [XMC4700 Relax Kit](https://github.com/Infineon/XMC-for-Arduino/wiki/XMC4700-Relax-Kit), and [DEMO Radar BB XMC4700](https://github.com/Infineon/XMC-for-Arduino/wiki/DEMO-Radar-BB-XMC4700)) as well as additional information. 
Please have a look on the sidebar to find the related information and visit our site for makers [here](www.infineon.com/4makers) with additional information about other boards.

## Current Status
* Basic features comparable to Arduino implemented
* Additional underlying features implemented
  - RTC library
  - DMA library (beta, in development)
  - Device Control Library
* Special variants and boards implemented, e.g. XMC1300 Boot Kit or XMC1100 H-Bridge 2Go

## The XMC Microcontroller Family
Infineon has designed the XMC microcontrollers for real-time critical applications with an industry-standard core. The microcontroller family based on ARM® Cortex®-M cores is dedicated to applications in the segments of power conversion, factory and building automation, transportation and home appliances. 
Find out more on the respective homepage of the XMC family:

[https://www.infineon.com/XMC](https://www.infineon.com/XMC)

We strongly encourage you to extend the list of applications by your support. If you feel like, please share your ideas, projects as well as software examples with the community to see what the XMC is capable to do.

### XMC1000 Key Features
* ARM® Cortex®-M0 core, up to 48MHz and 80 CoreMark
* Control peripherals like PWM timers run on up to 96MHz
* The MATH co-processor boosts standard Cortex®-M0 computing performance enabling divisions and trigonometric operations like SIN and COS
* The BCCU eases digital LED dimming and color control applications
30ns comparators enable AC-DC and low voltage DC-DC SMPS control e.g. up to 4 channel buck converters
* The ERU is a programmable hardware interconnect matrix that provides on-chip connectivity for real-time control and offloads the CPU
* The CCU PWM-timers feature rich and application oriented configurability like for motor control, SMPS or combustion engine control
* Hall sensors and optical encoders can be connected to POSIF, a position interface for motor position control
* With a 1Msps 12-bit ADC, XMC1000 microcontrollers are outstanding in their price / performance class
MultiCAN provides connectivity with 2 nodes and 32 message objects

### XMC4000 Key Features
* ARM® Cortex®-M4 with floating point unit (FPU), single-cycle DSP MAC, 80-144MHz CPU frequency
* Up to 2MB embedded Flash with 22ns access time and error correction unit
* Up to 352kB embedded RAM
* EtherCAT ® node
* 12-channel DMA (XMC4500), 8-channel DMA (XMC4400, XMC4200, XMC4100)
* Comprehensive set of timers, Delta sigma Demodulator, Position Interface, PWM with emergency shutdown and ADC trigger, Quadrature Encoder Interface
* 4-channel high-resolution, PWM (150ps) (XMC4400, XMC4200, XMC4100)
* Up to 4x 12-bit ADC achieving 4 Mega samples per second (interleaved mode
* 2x 12-bit DAC
* Up to 6 multi-functional serial interface modules configurable to SPI, I2C, I2S, UART
Up to 6xCAN
* External bus interface supporting SDRAM, SRAM, NOR-/NAND-Flash and memory-mapped IO devices (e.g. LCD)
* SD/MMC interface
* Touch interface and LED Matrix
* Battery-backed real-time clock with calendar function and time-based or external wake-up capabilities
* Extended temperature range up to 125°C ambient temperature

