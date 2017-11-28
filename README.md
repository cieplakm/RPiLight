# RPiLight

Lamp control via Raspberry Pi B+ and Android smartphone 

## Getting Started

I've startet from install Raspbian on RaspberryPi (instructions-> https://www.raspberrypi.org/downloads/)

Then I instaled nesesary libs and Java:

Java
```
https://www.raspberrypi.org/blog/oracle-java-on-raspberry-pi/
```

Pi4J 
```
http://pi4j.com/install.html#EasyPreferred
```

WiringPi (Pi4J needs it)
```
http://wiringpi.com/download-and-install/
```


### Used hardware

![RaspberryPi B+](https://github.com/cieplakm/RPiLight/tree/master/imgs/rpi0.jpg) (85PLN)

![Relay](https://github.com/cieplakm/RPiLight/tree/master/imgs/przekaznik.jpg) (~5PLN)

Some wire (~5PLN)

Wire for RPi (40 pins)

Plug and socket(~10PLN)

WiFi Dongle


### Hardware connection

Connection like in ![SCHEMA](https://github.com/cieplakm/RPiLight/blob/master/imgs/schema.jpg?raw=true)

## Software


Here you find my lib for this project. There are client and server objects

```
https://github.com/cieplakm/rpilight-communication-lib
```


### Server

I write lib to create simple server and client.

```
https://github.com/cieplakm/rpi-light-server
```

### Client

My client is a Android app - RPiLight

```
https://github.com/cieplakm/rpilight-android-app
```

### RaspberryPi configure

To start Server at boot I edited
```
/etc/rc.local
````
and added before 'exit 0'

```
sudo java -cp .:classes:/home/pi/share/rpi-light/libs/'*':/home/pi/share/rpi-light: RPiServer 
```

## Demo

```
https://youtu.be/Et3TMCKdom8
```

