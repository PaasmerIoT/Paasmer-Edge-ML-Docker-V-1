# Paasmer-Edge-ML-Docker-V-1
**Paasmer-Edge-ML-Docker-V-1** for Raspberry-pi Running **Paasmer OS**.

## Overview

The **Paasmer-Edge-ML-Docker-V-1** for Raspberry-pi Running **Paasmer OS** is a collection of Docker containers with a sample **Machine Learning Docker** model that monitors the Health condition based on the Blood Pressure and Blood Sugar level sent from an sample Android App. 

## Paasmer OS
**Paasmer OS** is an attempt to make container-based services available for Machine learning with SBC's. Currently, we only support the Raspberry-Pi. Support for other devices coming soon.

## Machine Learning in Paasmer
**Machine Learning** in Paasmer is now possible. **Paasmer-Edge-ML-Docker-V-1** consists of a sample POC which monitors the Health condition, predicting the Health fall rate of a person from Andriod Application with Blood Pressure and Blood Sugar level based on your Breakfast timings.

### Andriod App
Paasmer Machine Learning POC is done with help of **PAASMER ML** App. This is a sample application that generates random readings of Blood Pressure, Blood Sugar Level and Breakfast time for performing ML. 

#### Usage 
Provide the IP address of the Paasmer Gateway, Patients Name and Time interval of send values from App to the ML Docker.

**Note- The Mobile phone must be connected to the local network same as that of your Gateway.**

## Pre Requisites
Registration on the [PAASMER portal](http://developers.paasmer.co) is necessary to connect the devices to the **Paasmer IoT Platform**. A Raspberry-Pi board with SD card.


# Installation

### OS Image Downloading

#### For Windows
* Download the zip file [click here](https://github.com/PaasmerIoT/Paasmer-Edge-ML-Docker-V-1/releases/download/1.0/paasmerOS.zip) and extract it.

#### For Linux
* Download the run file.[click here](https://github.com/PaasmerIoT/Paasmer-Edge-ML-Docker-V-1/releases/download/1.0/paasmerOS) to download.

* Run the file using the command.
```
$ sh paasmerOS
```
This will extract the customized Paasmer OS image to your home directory.

### Docker Initialization

* Flash the SD card with the ISO image.

* Insert the card into the Raspberry-Pi and boot it. Login with `Username: pi` and `Password: raspberry`

* Get started with RaspberryPi and [click here](https://thepihut.com/blogs/raspberry-pi-tutorials/83502916-how-to-setup-wifi-on-raspbian-jessie-lite) to setup WiFi connection.

* Navigate to the paasmer-docker folder using the command.
```
cd /home/pi/
```

* Run the paasmer-docker.run
```
$ sh paasmer-docker.run
```
* This will install and build the necessary dockers
* Enter a UserName and DeviceName. The UserName is what you used in developers.paasmer.co for registration and give a unique DeviceName for your device and that must be alphanumeric without any spaces[a-z A-Z 0-9].

* Wohooo! That's all. Your device should be connected to the Paasmer platform.

## Support

The support forum is hosted on the GitHub, issues can be identified by users and the Team from Paasmer would be taking up requests and resolving them. You could also send a mail to support@paasmer.co with the issue details for a quick resolution.

## Note

* The Paasmer OS utilizes the features provided by Raspbian OS and Docker engine.


