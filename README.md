# SensorTag
 sensor tag M2M network using atmega328p as a microcontroller and LORA RFM98 as a transmitter module to sense humidity and temperature.

Main Features
This module will sense the data and send it to the gateway at aa predefined interval.
Works on 3.7 li-Ion battery.
Power efficient sensor node with battery indication.
When antenna is connected to the module then the node can transmit upto a range of 1 kilometer.
Hardware
3.3V 16MHz (with ATmega328P)
3.3V RFM98 module
TI HDC2080 temperature and humidity sensor
ESP32
Materials
Arduino code with sleep mode and the rfm connections.
Similar ESP32 code with sleep mode and transmission btu it consumes more power as compared to Arduino328p.
Reciever code.
HDC2080 Datasheet.(http://www.ti.com/lit/ds/symlink/hdc2080.pdf)
Rfm98 datasheet.(https://cdn.sparkfun.com/assets/learn_tutorials/8/0/4/RFM95_96_97_98W.pdf)
Arduino 328p Datasheet.(http://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-7810-Automotive-Microcontrollers-ATmega328P_Datasheet.pdf)
ESP32 Datasheet.(https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)
Li-Ion battery->18650mAh battery.(https://www.banggood.in/buy/18650-battery.html)
Programs attached(Arduino IDE Code)
Project 1
Arduino with battery status contains the code for Arduino328p with rfm98 and HDC2080 which senses the temp and humidity and the battery status and send it to the esp32rfm gateway.
ESP32 receiver RFM is the gateway code for Arduino sensor node.
Project 2
BLE Sender is the ESP32 code to transmit data using inbuilt BLE in ESP32 to a BLE gateway
BLE Gateway is the BLE gateway program for esp32 BLE sender.
Software
Installation Instructions
Using Arduino IDE Boards Manager (preferred)
Instructions for Boards Manager
Using Arduino IDE with the development repository
Instructions for Windows
Instructions for Mac
Instructions for Debian/Ubuntu Linux
Instructions for Fedora
Instructions for openSUSE
Using PlatformIO
Building with make
Using as ESP-IDF component
Using OTAWebUpdater
Decoding exceptions
You can use EspExceptionDecoder to get meaningful call trace.

Issue/Bug report template
Before reporting an issue, make sure you've searched for similar one that was already created. Also make sure to go through all the issues labelled as for reference.

Finally, if you are sure no one else had the issue, follow the ISSUE_TEMPLATE while reporting any issue.

ALL connection:
ESP32Dev Board PINMAP
Pin Functions

Arduino uno PINMAP
Pin Functions

LORA RFM98 PINMAP
Pin Functions

ESP32 with RFM98 PINMAP
Pin Functions

Arduino with HDC2080 PINMAP
Pin Functions

Additional Installation on Arduino IDE 1.8+
Add the following URL to the Arduino Boards Manager (File->Preferences).

https://github.com/watterott/ATmega328PB-Testing/raw/master/package_m328pb_index.json
Update the Arduino AVR Boards to version 1.6.22 or higher via the Boards Manager (Tools->Boards->Boards Manager).

Install the ATmega328PB Boards via the Boards Manager (Tools->Boards->Boards Manager).
