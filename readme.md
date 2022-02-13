## Description

[OnStep](https://onstep.groups.io/g/main/wiki) is an open source project to control a telescope mount (goto). 



Essential board is an hardware solution which use OnStep with the essential parts only :

- ESP32 to run OnStep
- 3 axis controller (DE, RA and focuser)
- GPS (time and location)
- Humidity, barometric pressure and ambient temperature sensors



This project provides :

- Design of the Essential board
- Updated OnStep project for this board



## Main components ##

- (x1) **Essential board** (this project)

- (x1) **ESP32-WROOM DEVKIT**

- (x1) **ATGM336H** gps

- (x1) **BME208** sensor

- (x3) **Nema17** motor (DE, RA and focuser)

  ```
  Manufacturer Part Number: 17HS4401 (42BYGH)
  Motor Type: Bipolar Stepper
  Step Angle: 0.9 deg.
  Step : 400
  Holding Torque: 280 mM.m
  Rated Current/phase: 1.3A
  Shaft Diameter: 5mm
  Number of Leads: 4
  Weight: 280g
  ```
  
- (x3) **TMC2225** stepper motor driver

  ```
  Manufacturer Part Number: TMC2225
  Motor voltage: 4.75V-36V DC
  Max output current (RMS): 1.4A
  Max output current (peak): 2.0A
  ```



**//////////// ADD PICTURES HERE ////////////**



## Installation

This project use ARDUINO environment, install it before to start.

Then, follow these steps :

**//////////// ADD STEPS HERE ////////////**



## How to flash the board

**//////////// ADD STEPS HERE ////////////**



## Validation

This project was tested with these parts :

- Bresser EQ3 mount, with custom goto addon : [stl files](https://cults3d.com/fr/modèle-3d/divers/bresser-eq3-motor-addon)
- Telescope application (OSX)









## TODO ##





```shell
git remote add upstream https://github.com/hjd1964/OnStep
```







- Select *File>Preferences* "Additional Boards Manager URLs" and add: **https://dl.espressif.com/dl/package_esp32_index.json**
- Install support for this board from within the menu *Tools>Board>Boards Manager*
  - Use ESP32 version **1.0.4 only**

Configuration

 [**Online Configuration Generator**](http://o.baheyeldin.com:1111/) 

In the **Arduino IDE Tools menu** select the correct **board** and **port**.

 The ESP32 comes in many types but the ESP32 Dev Module using its default settings generally seems to work for the variants we use.



- To test onstep 
  -  **:GVP#**





next step : https://onstep.groups.io/g/main/wiki/3862



dependencies 

Rtc by Makuna

Adafruit BMP280
