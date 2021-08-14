# rand0m / lcdproc / i2c
ldcproc and LCDd config files ready to work with affordable i2c LCD (2x40) and Raspberry Pi.

New driver has been added that allows pin configuration via "LCDd.conf", move "hd44780.so" to "/usr/lib/arm-linux-gnueabihf/lcdproc/", also make sure to set "Port" and "Device" properly before use (sudo i2cdetect -y 1, use 0 for older RPi 1).

Original driver: https://github.com/wilberforce/lcdproc (big thanks!)

Tested on Raspberry Pi 4

## alternative wiring example


```

   PCF8574AP: P0 P1 P2 P3 P4 P5 P6 P7
              |  |  |  |  |  |  |  |
   HD44780:   RS RW EN BL D4 D5 D6 D7

```
