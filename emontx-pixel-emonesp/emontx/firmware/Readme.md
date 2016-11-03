# emonTx Firmware

The emonTx firmware uses the C++ Arduino framework.

## Compile * Upload Using PlatfomIO

We will use [PlatformIO](https://platformio.org) to compile and upload the firmware. Arduino IDE can also be but PlatformIO is easier to setup since all required libraries and tool chains are automatically downloaded.

#### Install platformIO

PlatformIO (pio) works great from the commandline, follow these instructions to install and run platformIO from the commandline. See the excellent [PlatformIO Quick Start Guide](http://docs.platformio.org/en/latest/quickstart.html) for more info. Platform IO has also got a GUI interface based on the Atom text editor. See PlatformIO website for install guide

The easiest way to install if running Mac / Linux is to use the install script, this installs pio via python pip and installs pip if not present. See [PlatformIO installation docs](http://docs.platformio.org/en/latest/installation.html#installer-script):

`$ sudo python -c "$(curl -fsSL https://raw.githubusercontent.com/platformio/platformio/master/scripts/get-platformio.py)"`

See PlatformIO website for [Windwows install guide](http://docs.platformio.org/en/latest/installation.html#local-download-mac-linux-windows)

### Compile

Enter project dir and run platfomio (pio):

```
$ cd build-workshop/emontx-pixel-emonesp/emontx/firmware
$ pio run
```

### Upload

Connect emonTx via USB to UART cable:

![usb-uart](imags/build014.jpg)

Then run:

`$ pio run -t upload`

*This may require `sudo`*

### View serial output

PlatformIO can also be used to view the serial output from the emonTx:

`$ pio device monitor -b115200`

You shuuld see serial output of:
