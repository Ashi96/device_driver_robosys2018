# device_driver_robosys2018
![Alt](https://github.com/Ashi96/device_driver_robosys2018/blob/master/docs/images/displays_number_4.JPG)

## Overview
Device driver that displays numbers using 11 LEDs on Raspberry Pi 3 Model B+. 

## Description
7-segment LED is a device to display numbers using LEDs. I did the same thing with the device driver.

## Demo
https://www.youtube.com/watch?v=jmppEoof3j4&t=2s

## Requirement
- Computer  
  - Raspberry Pi 3 Model B+
- Operation System  
  - Raspbian
- Rebuilding a linux kernel
  - https://github.com/ryuichiueda/raspberry_pi_kernel_build_scripts
- Parts
  - LEDs
    - red http://akizukidenshi.com/catalog/g/gI-06245/
    - green http://akizukidenshi.com/catalog/g/gI-06246/
    - yellow http://akizukidenshi.com/catalog/g/gI-06248/
  - Bread Board http://akizukidenshi.com/catalog/g/gP-05294/
  - jumper wire
    - male-male http://akizukidenshi.com/catalog/g/gC-05371/
    - male-female http://akizukidenshi.com/catalog/g/gC-08933/

## Circuit
![Alt](https://github.com/Ashi96/device_driver_robosys2018/blob/master/docs/images/circuit%20diagram.png)  
A resistor is connected to the inside of this LED.

## Install
~~~
$ git clone https://github.com/Ashi96/device_driver_robosys2018.git
~~~

## Usage
~~~
$ make
$ sudo insmod myled.ko  
$ sudo chmod 666 /dev/myled0  
ex) when you want to display "0"  
$ echo 0 > /dev/myled0
~~~

## License
GNU GENERAL PUBLIC LICENSE　Version3  
https://www.gnu.org/gnu/gnu.html
