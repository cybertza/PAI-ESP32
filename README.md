# PAI-ESP32
ESp32 Eg for Serial -> wifi
Add main.cpp to platform.io or make it INI for Arduino

for Esphome you just need:

the esphome yaml

More info to be found on https://github.com/ParadoxAlarmInterface/pai/wiki/Connection-methods#serial-over-ip-esp32

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
