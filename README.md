# device_driver_robosys2018
![Alt](https://github.com/Ashi96/device_driver_robosys2018/blob/master/docs/images/displays_number_4.JPG)

## Overview
Device driver that displays numbers using LEDs

## Demo
https://www.youtube.com/watch?v=jmppEoof3j4&t=2s

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
