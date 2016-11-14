# ESP8266----web_Socket

This code was developed for the ESP8266 dorkbotpdx class for November 13, 2016.
https://dorkbotpdx.org/esp8266_2016

We'll be programming the ESP8266 wifi chip. We used the NodeMCU development board although most ESP8266 boards will work(not sparkfun.. see memory issues below).

The NodeMcu's for the class are pre-programmed as wifi hot spots. Try connecting to your board with your phone and trying these pages: http://192.168.4.1/index.html this controls the blue onboard LED

Install Arduino 1.6.11 or 1.6.12 from here: https://www.arduino.cc/en/Main/OldSoftwareReleases#previous

Follow the directions by sparkfun to add the json board files from the Arduino Board Manager menu: https://learn.sparkfun.com/tutorials/esp8266-thing-development-board-hookup-guide/setting-up-arduino

Create a directory in your My Documnets called Arduino. Add the esp8266fs.jar file to the directory Arduino/tools/ESP8266FS/tool/esp8266fs.jar This file allows you to upload html and js data files to your Arduino. There are no folders though. The file is here:https://github.com/esp8266/arduino-esp8266fs-plugin/releases/tag/0.2.0

The 192.168.4.1/index.html file contains a websocket connection between the NodeMCU Access Point server and your client device.

Small is important as there are memory constraints. Here is a description of how the memory is allocated for FS file systems: https://github.com/esp8266/Arduino/blob/master/doc/filesystem.md

There is a list of micro javascript libraries here: http://microjs.com/#

Here are some Arduino Learning resources: http://www.pcc.edu/staff/index.cfm/1514,13821,30,html
