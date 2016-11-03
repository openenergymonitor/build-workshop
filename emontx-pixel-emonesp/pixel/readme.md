# EmonESP Pixel

**WiFi connected ESP8266**

1. Takes serial input string from emonTx e.g. `ct1:30,vrms:40.75`
2. Display visual power value from `ct1` sensor
3. Post to [Emoncms.org](https://emoncms.org) via WiFi

## Connections

Connect serial input from emonTx:

![01](images/build016.jpg)

![01](images/build017.jpg)

![01](images/build000.jpg)

![01](images/build001.jpg)

## Firmware

- Pre-loaded due to time constraints but can be loaded in the same way as emonTx firmware using PlatformIO. See `firmware/EmonESP` folder for instructions
- Running adapted [EmonESP](github.com/openenergymonitor/EmonESP) firmware
- Firmware upload / serial output must be done using UART pins, micro-USB is for power only

## LED Visual power reading

<photos> 

## Post data online to Emoncms cloud

https://emoncms.org

### 1. Create account on Emoncms.org

### 2. EmonESP Pixel Config

![01](images/wifi.png)

![01](images/wifi-connected.png)
