# PAI-ESP32

This in its most basic form is just a ESP32 Serial to WIFI bridge, there is a more comprehensive writeup for 
more info to be found on https://github.com/ParadoxAlarmInterface/pai/wiki/Connection-methods#serial-over-ip-esp32

You can also just use the prebaked egsamples on most IDE's
ESp32 Eg for Serial -> wifi

Add main.cpp to platform.io or make it INI for Arduino

for Esphome you just need:
You need to create a new device in esphome, and then use the details from the yaml in the esphome folder



This is a work in progress
```
Serial on Panel         LM2956            ESP32
┌───────┐               
│ Rx   ┌╵   == > == > == > == > == > == > TX2 
│ Tx   │    == > == > == > == > == > == > RX2 
│ GND  │    == > IN(-)   ->   OUT(-) == > USB GND 
│ AUX+ └╷   == > IN(+)   ->   OUT(+) == > USB 5V
└───────┘
```

If there is a lot of interest we can add an Failback with config, and release a bin for easy use.
