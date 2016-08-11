[![Bare Conductive](http://bareconductive.com/assets/images/LOGO_256x106.png)](http://www.bareconductive.com/)

# Bare Conductive Touch MP3 and LED Demo Code

Touch-to-MP3 code including a separate pin for each electrode / track which goes high while that track is playing. That pin can be used to drive a LED by connecting the anode (positive leg of the LED) to the relevant pin and the cathode (negative leg) to ground. A larger load (LED strip, motor etc.) can be driven with an appropriate transistor driver circuit. 

Written for the [Bare Conductive Touch Board](http://www.bareconductive.com/shop/touch-board/).

The mapping between electrodes and the pins which go high in response is:

* E0 -  D0
* E1 -  D1
* E2 -  D10
* E3 -  D11
* E4 -  D12
* E5 -  D13 (which has an onboard LED connected to it)
* E6 -  A0  (analogue inputs can be used as digital outputs too)
* E7 -  A1
* E8 -  A2
* E9 -  A3
* E10 - A4
* E11 - A5 

You need twelve MP3 files named TRACK000.mp3 to TRACK011.mp3 in the root of the microSD card. 
 
When you touch electrode E0, TRACK000.mp3 will play. When you touch electrode E1, TRACK001.mp3 will play, and so on.

    SD card    
    │
      TRACK000.mp3  
      TRACK001.mp3  
      TRACK002.mp3  
      TRACK003.mp3  
      TRACK004.mp3  
      TRACK005.mp3  
      TRACK006.mp3  
      TRACK007.mp3  
      TRACK008.mp3  
      TRACK009.mp3  
      TRACK010.mp3  
      TRACK011.mp3  

## Requirements
* You should make sure that you have followed our [Setting up Arduino with your Touch Board](http://www.bareconductive.com/make/setting-up-arduino-with-your-touch-board/) tutorial before using this (or any other) of our code examples


## Install

1. Close the Arduino IDE if you have it open.
1. Download the [.zip](https://github.com/BareConductive/touch_mp3_with_leds/archive/public.zip) or clone the repository to your local machine - if downloading the .zip, extract the contents somewhere that suits you.
1. Take the **touch_mp3_with_leds** folder and move it to **Arduino Sketchbook Folder**. This will be different for each operating system: 

	**Windows**
	
	Libraries\\Documents\\Arduino
	
	or
	
	My Documents\\Arduino	
	
	**Mac**
	
	Documents/Arduino
	
	**Linux (Ubuntu)**
	
	Home/Arduino


	If this folder does not exist, create it first.
1. Reopen the Arduino IDE - you should now be able to open the sketch in the **File -> Sketchbook** menu.
