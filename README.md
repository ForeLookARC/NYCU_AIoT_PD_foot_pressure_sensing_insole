# AIoT PD Foot Pressure Sensing Insole
This application is designed to show how to diagnose whether the users have the tendancy of Parkinson's disease using embARC. **AIoT PD Foot Pressure Sensing Insole** can measure user's gait, and then judge if the user is in high risk of the disease by NN Model. Every components of the device are detachable which makes it superior in mobility and convenience. Also, it can be controlled by Android App. The connection between the device and the Smartphone is based on Wi-Fi.

* [Introduction](#introduction)
	* [System Architecture](#system-architecture)
	* [Android App](#android-app)
* [Hardware and Software Setup](#hardware-and-software-setup)
	* [Required Hardware](#required-hardware)
	* [Required Software](#required-software)
	* [Hardware Connection](#hardware-connection)
* [User Manual](#user-manual)
	* [Before Running This Application](#before-running-this-application)
	* [Run This Application](#run-this-application)

## Introduction

**AIoT PD Foot Pressure Sensing Insole**

AIoT PD Foot Pressure Sensing Insole is a smart device which can be used to monitor the high-risk populations of Parkinson's disease. By daily monitoring, users can get the warning before everything get worse and look for the treatment as soon as possible. For PD patients, our project can also be a severity reference.


### System Architecture

### Android App
Our device can be controlled by AIoT-PD Android App. You can start/stop the measurement, see your foot pressure destribution and the final result on the App.

![app pic][0]
## Hardware and Software Setup
### Required Hardware
- 1 Himax WE-I Plus EVB Endpoint AI Development Board
- 2 Raspberry Pi 3 Model B
- 2 8-Channel 12-Bit ADC for Raspberry Pi (STM32F030)
- 2 RPi UPSPack V3
- 2 4000mAh Lithium Battery
- 16 FlexiForce A301 Pressure Sensor (111N)

- **The physical picture shown below.**
![hardware_pic][1]({:height="100px" width="400px"}

- **The structure diagram shown below.**
![hardware_pic][2]
### Required Software
- Metaware or ARC GNU Toolset
- embARC Machine Learning Inference Library
- AIoT-PD Android App

### Hardware Connection

## User Manual
### Before Running This Application
- Download source code and AIoT-PD App from github
- Setup hardware connection
The hardware resources are allocated as following table.

|  Hardware Resource  |            Function                                           |
| ------------------- | ------------------------------------------------------------- |
|  FlexiForce A301    |        Pressure  sensor                                       |
|  STM32F030          |        ADC for Raspberry Pi                                   |
|  RPi UPSPack V3     |        Portable Power Supply                                  |
|  Raspberry Pi 3     |        Data Preprocessing, Provide WiFi Connection            |
### Run This Application


[0]: doc/screenshots/APP.png	"app_pic" 
[1]: hardware/photo.png	"hardware_pic"
[2]: hardware/Rpi_Himax.jpg	"hardware_pic"

