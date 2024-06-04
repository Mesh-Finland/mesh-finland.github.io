# hardware guide for beginners


* Goal of this guide:
  * present a limited list of devices
    * plusses and minus
  * other consideration

* The Meshtastic Documentation pages have good technical info about supported devices


## how many do I need or want at the start

* 1 or 2 depending on if you want to experiment familiarize yourself with the technology
  * 1 device with you
  * 2nd at home or with a family member
  * are there other nodes near you that you want to communicate with.

* 3+ 
  * ok, but don't go overboard before getting famility, do consider the features you need

## cases

* 3d print, ready, library, tupperware, icecream, box it came in, pictures?

## Batteries

* It's very important to underdand safety when using any kind of batteries
  * especially Lithium
    * LIPOs
	* 18650
	* other
* You may need to buy and install your own battery for a device

## Antenna
* Make sure an antenna is connected to the device when it is powered.

## Features to consider

* power consumption / efficiency
  * Consider how you will power the device
    * USB port / charger
	* USB power bank
	* Own battery
* Frequency 
  * 868 MHz 
  * Use of 433MHz is very limited
* GPS
  * GPS model, antenna size.
  * A device can also use position data from your phone
* Screen
   * OLED
   * ePaper
   * no screen
* Processor
  * ESP32 vs ESP32s3 vs nRF52840
* GPIO 

## devices to consider

* heltec
  * more afforable
    * unless you start to think about powering with batteries or solar
  * a bit power hungry, very inefficient use of batteries (own lipo and power bank)
  * ok for desk use and occasional portable use
  * devices normally come with a battery connector that needs to be connected to a battery

* lilygo
  * Efficent power management. 
  * Good for a portable node that will run for a day or more without recharging
  * Models typically have an 18650 holder on the back
    * when installing the battery put a piece of ribbon around it so it is easy to pull the battery out

* RAK
  * low power
  * ideal for solar
