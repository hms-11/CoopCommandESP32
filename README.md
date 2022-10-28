# CoopCommandESP32
Next generation Coop Command using an ESP32 as the MCU
## This is the next generation of the original, ATMEGA328P based CoopCommand found here: https://github.com/hms-11/CoopCommand

Chickens are simple animals with lots of benefits. The downside? Humans are not the only creatures that find chickens tasty and chickens themselves require some basic maintenance and care to keep happy and healthy. 

CoopCommand aims to reduce the daily labour of looking after chickens, improve their well-being as well as allow hobby-farmers the ability to go out for the night without worrying if their chickens are in danger from wandering predators. 

Contributors always welcome, I could use people smarter than myself to keep improving this project. 

You can also support this project through "Buy me a Coffee": 

<a href="https://www.buymeacoffee.com/AutoHobbyFarm" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>


# GOALS:

- Ease of installation and configuration for non-technical individuals. 

- Multiple Power Options (wall wart mains power or 12-24V off-grid solar/wind/battery systems).

- Wi-Fi connectivity for remote monitoring and overriding of coop door.


# FEATURES:

## TACO CHICKEN COOP COMMAND MAIN BOARD:

- Hardware debouncing on door limit switches.

- Pluggable Terminal Block connectors for all user-installed inputs/outputs.

- DHT22 Input (requires 10k pullup on DHT22) for interior coop temperature.

- DS18B20 Input (Pullup resistor already on board) for water temperature.

- GL5539 Photoresistor Input (requires GL5539 with 10K resistor as voltage divider) for daylight sensor.

- Efficient SMPS for off-grid operation @ 12-24V DC.

- TI DRV8871 Motor Driver IC w/3.6A current cabilitity & voltages up to maximimum working voltage of CoopCommand.

- LayLight MOSFET for controlling LED lights for supplementing daylight hours to keep chickens laying even with less than 14 hours of Daylight.

- Ventilation Fan MOSFET for controlling a fan for cooling the coop in the summer.

- Water Heat MOSFET for controlling a heater for heating the water in the winter. 

- USB-UART CH340 chip wirth auto-reset for ease of programming (just plug in a USB cable and go!)



## BLYNK:

- Override door open or closed.

- Monitor coop overall status (coop temperature, water temperature, fan and heat and light status).

- Monitor door status (Open, Closed, Opening/Closing).

- Adjust settings for all coop operations.

# Getting Started:

All files are included in this git-repository to get CoopCommand up and running. To get started, use the Gerber files and BOM to get the PCB's coming. The pic n place files can be used if your board house supports assembly. These boards were designed to use JLCPCB's assembly service. 

Once you have the board in hand and assembled, program can be easily loaded in using the Arduino IDE (or your preffered IDE) and a USB cable.

Once the board is programmed, see the BlynkInfo file for setting up your app. 

# CURRENT KNOWN ISSUES:

- Loss of wifi can result in the system getting stuck in a blocked loop, resulting in no Coop control operations happening until wifi is restored.   

