# ArduinoTerminalShield
Basic terminal shield for Arduino UNO based boards. Provide protection against ESD, fuses for 3V3 and 5V supply and analog input filtering.

## PCB manufacturing
Schematics, gerbers and Bill of Materials (BOM) are available under *Electronic Design* directory. PCBs can be oredered on JLCPCB or any other PCB manufacturer. It is recommended to buy components from reliable sources like Mouse, Farnell, Digikey, TME. All symbols and footprints on the schematics was acquired from mouser page.

## Bill of Materials
Available under *Electronic Design* directory.
Please ensure to use TVS SMAJ5.0A or SMAJ5.0CA for all applications, as there is an issue with the schematic where some TVS are incorrectly listed as SMAJ60CA instead of SMAJ5.0.

### IMPORTANT NOTICE ABOUT USAGE TVS/ZENER DIODES
The board contains TVS protection diodes to guard against ESD damage - SMAJ5.0A. However, they have significant capacitance. If the pin is intended for communication or PWM, it’s advisable to replace them with diodes of minimal capacitance or omit their installation.

### Usage of A0-A6 as digital outputs
If you would like to use analog pins A0-A6 as digital, please replace resistors R2-R7 with 0-ohm (0R) resistors or simply short them with solder and remove capacitors C1-C6.

## TODO
- [ ] Fix incorrect diode in some designators (SMAJ60CA instead of SMAJ5.0A)
- [ ] Find TVS with lower internal capacitance to be more suitable with PWM or communication (I2C, SPI)
## Images
![Image 1](https://github.com/TestDuino/ArduinoTerminalShield/blob/main/Images/3X8_TERMINAL_BLOCK_TopView.png)
![Image 2](https://github.com/TestDuino/ArduinoTerminalShield/blob/main/Images/3X8_TERMINAL_BLOCK_LeftSide.png)
![Image 3](https://github.com/TestDuino/ArduinoTerminalShield/blob/main/Images/3X8_TERMINAL_BLOCK_Front.png)
![Image 4](https://github.com/TestDuino/ArduinoTerminalShield/blob/main/Images/3X8_TERMINAL_BLOCK_LeftSide.png)
![Image 5](https://github.com/TestDuino/ArduinoTerminalShield/blob/main/Images/3X8_TERMINAL_BLOCK_Front.png)

### Contributions
If you find any bugs, have suggestions, or would like to contribute to the development of this project, feel free to contact me or submit a pull request (PR). Your contributions are greatly appreciated, and I am always open to feedback and collaboration. Thank you for helping to improve this project!

### Links
SMAJ Series | https://www.mouser.pl/datasheet/2/240/media-3319430.pdf  