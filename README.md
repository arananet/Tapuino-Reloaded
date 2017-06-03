# Tapuino-Reloaded

By @edu_arana in collaboration with @groovydrifter & @jgilcas. Based on the original design of Peter Edwards.

This new version has completely reworked with smd components. Also change the distribution and connection orientation. Now, you just plug the Tapuino Reloaded on the back of your C64 (Breadbox & C) and that's it. This design also allows to use every type of i2c LCD or OLED Screen, by soldering a 1x4 row pin and taking out the lcd to a better viewable area, for example on computers like the Commodore PET.

# Images

<img src="https://github.com/arananet/Tapuino-Reloaded/blob/master/images/tapuinoreloaded.png?raw=true" width="700">

<img src="https://github.com/arananet/Tapuino-Reloaded/blob/master/images/TapuinoReloadedreal.jpg?raw=true" width="700">

# Instructions
 
1. Download the official Tapuino code from the Peter Edwards repository https://github.com/sweetlilmre/tapuino 
2. Set the display hardware address on the config-user.h depending on what kind of display have. If does not work, use a i2c scanner in order to get the exact hardware address from the display.
3. Use a serial TTL programmer and the Arduino IDE to upload the code into the ATMEGA.
4. Plug an MicroSD card with all the taps and enjoy the power of the Tapuino!

# Updates

03/06/2017: Add DTR signal on the TTL programming port.

24/05/2017: If your Atmega328 is blank without bootloader you can take advantage by upload the bootloader and firmware directly to the atmega using an ISP like the USBASP. On the ISP folder there is a hex file that include the bootloader plus the firmware (tapuino) for oled screens.

 

# Bill of materials

| Part          | Value                   | Package                        |
| ------------- | ----------------------- | ------------------------------ | 
| C1            | 10uF/10V                | A/3216-18R                     |
| C2            | 0.1uF                   | C0805                          |
| C3            | 100nF                   | C0805                          |
| C13           | 22p                     | C0805                          |
| C14           | 22p                     | C0805                          |
| CON1          | CONECTOR_C64_DATASSETTE | 2x6 C64_CONNECTOR (pin version)|
| IC1           | 4050D                   | SO16                           |
| IC2           | AVR-ATMEGA328p-TQP32    | QFP32                          |
| IC3           | LP298XS                 | SOT23-5L                       |
| ISP           | AVR_SPI_PRG_6PTH        | 2X3                            |
| TTL           | PINHD_1X03              | 1X03                           |
| JP1           |                         | OLED CONNECTOR                 |
| ACT           | RED                     | CHIP-LED0805                   |
| LED1          | WHITE                   | CHIP-LED0805                   |
| LED2          | BLUE                    | CHIP-LED0805                   |
| POWER         | GREEN                   | CHIP-LED0805                   |
| OK1           | 4N25                    | DIP06 optocoupler              |    
| Q1            | 2N2222                  | SOT-23 Transistor              |    
| Q2            | 2N2222                  | SOT-23 Transistor              |   
| Q3            | 16MHZ                   | QS                             |
| R1            | 1K                      | R0805                          |
| R2            | 1K                      | R0805                          |
| R3            | 220                     | R0805                          |
| R4            | 220                     | R0805                          |
| R5            | 330                     | R0805                          |
| R6            | 10k                     | R0805                          |
| R7            | 120                     | R0805                          |
| R8            | 1M                      | R0805                          |
| R9            | 1K                      | R0805                          |
| ABORT1        | PUSH BUTTON             | RIGHT ANGLE PUSH BUTTON        |
| NEXT1         | PUSH BUTTON             | RIGHT ANGLE PUSH BUTTON        |
| PREV1         | PUSH BUTTON             | RIGHT ANGLE PUSH BUTTON        |
| S1            | PUSH BUTTON             | PUSH BUTTON                    |
| SELECT1       | PUSH BUTTON             | RIGHT ANGLE PUSH BUTTON        |
| SD1           | TF-HOLDER               | TF-PULL                        |

# Changes
v1.1 Fixed drill holes on the gerbers files because some gerber viewers do not show them correctly.
