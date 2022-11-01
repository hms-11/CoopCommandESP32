# CoopCommandESP32

Next generation Coop Command using an ESP32 as the MCU

#### This is the next generation of the original, ATMEGA328P based CoopCommand found [HERE](https://github.com/hms-11/CoopCommand).

# Overview

Chickens are simple animals with lots of benefits. The downside? Humans are not the only creatures that find chickens tasty and chickens themselves require some basic maintenance and care to keep happy and healthy. 

CoopCommand aims to reduce the daily labour of looking after chickens, improve their well-being as well as allow hobby-farmers the ability to go out for the night without worrying if their chickens are in danger from wandering predators. 

[![CoopCommand Picture](https://github.com/hms-11/CoopCommandESP32/blob/main/CoopCommandImages/PXL_20221015_171228559.jpg)](https://github.com)

Contributors always welcome, I could use people smarter than myself to keep improving this project. 

You can also support this project @ 
<a href="https://www.buymeacoffee.com/AutoHobbyFarm" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>


# GOALS:

- Allow Backyard Chicken owners the ability to increase the security and productivity of their flock while reducing the daily labour costs of chicken ownership. 

- Automatic Coop Door controlled by daylight in order to more closely track chicken behaviour. 

- Monitor and control coop and water temperatures to prevent overheating of the coop and freezing of the water.

- "LayLight" which monitors daylight light levels and ensures chickens receive at least 14 hours of daylight to maintain laying throughout winter months.

- Ease of installation and configuration for non-technical individuals. 

- Designed for Off Grid Operation (12-24v DC), can also be powered by a suitably sized 12-24V DC Power Supply from an AC source.



# FEATURES:

## TACO CHICKEN COOP COMMAND MAIN BOARD:

- Hardware debouncing on door limit switches. [Example Limit Switches](https://www.amazon.ca/SpeedDa-Magnetic-Switch-Normally-Security/dp/B076GZDYD2/ref=sr_1_11?crid=1FTS5IZLOU1AM&keywords=magnetic+door+switch&qid=1667011161&qu=eyJxc2MiOiI0LjYxIiwicXNhIjoiNC4xMSIsInFzcCI6IjMuODAifQ%3D%3D&sprefix=magnetic+door+swi%2Caps%2C431&sr=8-11)

- Pluggable Terminal Block connectors for all user-installed inputs/outputs.

- DHT22 Input (requires 10k pullup on DHT22) for interior coop temperature. [Example DHT22](https://universal-solder.ca/product/dht22-temperature-humidity-sensor-16bit-digital-interface/)

- DS18B20 Input (Pullup resistor already on board TACO CHICKEN board) for water temperature. [Example DS18B20](https://universal-solder.ca/product/digital-temperature-sensor-ds18b20-watertight-1-wire-interface-3-meter-wire/)

- GL5539 Photoresistor Input (requires GL5539 with 10K resistor as voltage divider) for daylight sensor. [Example GL5539](https://universal-solder.ca/product/50-pcs-photo-resistor-5-different-types-10-each-gl55xx-series/)

- Efficient SMPS for off-grid operation @ 12-24V DC.

- TI DRV8870 Motor Driver IC w/3.6A current cabilitity & voltages up to maximimum working voltage of CoopCommand.

- LayLight MOSFET for controlling LED lights for supplementing daylight hours to keep chickens laying even with less than 14 hours of Daylight.

- Ventilation Fan MOSFET for controlling a fan for cooling the coop in the summer. [Example Ventilation Fan](https://www.amazon.ca/MACHSWON-Cooling-Exhaust-Ventilation-Motorhome/dp/B08FMNZH5T/ref=sr_1_8?keywords=12v+ventilation+fan&qid=1667011330&qu=eyJxc2MiOiIzLjM1IiwicXNhIjoiMi4wMCIsInFzcCI6IjAuMDAifQ%3D%3D&sprefix=12v+ventilat%2Caps%2C151&sr=8-8)

- Water Heat MOSFET for controlling a heater for heating the water in the winter. [Example Water Heater](https://www.amazon.ca/Dernord-Immersion-Submersible-Element-Stainless/dp/B0761L2Q8M/ref=sr_1_25?crid=V2QPTYX224KK&keywords=12v+water+heater&qid=1667011500&qu=eyJxc2MiOiI1LjIwIiwicXNhIjoiNC42NiIsInFzcCI6IjIuNTIifQ%3D%3D&sprefix=12v+water+heate%2Caps%2C149&sr=8-25)

- USB-UART CH340 chip wirth auto-reset for ease of programming (just plug in a [USB A - USB A cable](https://www.amazon.ca/DTECH-Type-Cable-Speed-Black/dp/B079GV2F5W/ref=sr_1_12?crid=FD392ACYKISH&keywords=usb+a+usb+a&qid=1667011638&qu=eyJxc2MiOiIyLjI1IiwicXNhIjoiMi4wMCIsInFzcCI6IjEuNTgifQ%3D%3D&refinements=p_n_availability%3A12035748011&sprefix=usb+a+usb+a%2Caps%2C162&sr=8-12) and go!)

[![CoopCommand Picture](https://github.com/hms-11/CoopCommandESP32/blob/main/CoopCommandImages/PXL_20221029_195134568.jpg)](https://github.com)


## BLYNK:

- Override door open or closed.

- Monitor coop overall status (coop temperature, water temperature, fan and heat and light status).

- Monitor door status (Open, Closed, Opening/Closing).

- Adjust settings for all coop operations.

[![CoopCommand Picture](https://github.com/hms-11/CoopCommandESP32/blob/main/CoopCommandImages/Screenshot_20221029-083134.png)](https://github.com)
[![CoopCommand Picture](https://github.com/hms-11/CoopCommandESP32/blob/main/CoopCommandImages/Screenshot_20221029-083106.png)](https://github.com)

# THE BOARD:

CoopCommand uses the TacoChicken control board. Currently the board is on Rev1. The board is 100% Open Source and all files can be found [HERE](https://oshwlab.com/coreyearl1985/tacochickenrev1-dc_copy)

If you want to purchase the pre-assembled board, I have them for sale [HERE](https://www.tindie.com/products/hms-11/taco-chicken-esp32-based-control-board/)


# Getting Started:

All files are included in this git-repository to get CoopCommand up and running. To get started, either create/modify your own based on this [OPEN SOURCE](https://oshwlab.com/coreyearl1985/tacochickenrev1-dc_copy) board or buy the board [HERE](https://www.tindie.com/products/hms-11/taco-chicken-esp32-based-control-board/).

Once you have the board in hand and assembled, program can be easily loaded in using the Arduino IDE (or your preffered IDE) and a USB A - USB A cable.

First, follow the instructions in the [BlynkInfo](https://github.com/hms-11/CoopCommandESP32/blob/main/BlynkInfo) file. This will setup the needed steps to get the app going and generate a required Template ID and Device Name to be added to your program to be uploaded to the board.

Secondly, download all code files [HERE](https://github.com/hms-11/CoopCommandESP32/archive/refs/heads/main.zip). Extract all files in the CoopCommand folder into a folder all together. If you open the .ino file using Arduino IDE all other files will be loaded at same time. Insert the Template ID and Device Name into the appropriate location at the top of the sketch.  Select your board (ESP32 Dev Module), select your Com Port and click upload!

 

# CURRENT KNOWN ISSUES:

- Loss of wifi can result in the system getting stuck in a blocked loop, resulting in no Coop control operations happening until wifi is restored.   

# THANKS

There is an incredible reddit community dedicated to reviewing PCB schematics and layouts. This project, and many others of mine would not be possible without the amazing individuals present in this community. The subreddit is https://www.reddit.com/r/PrintedCircuitBoard/ .

