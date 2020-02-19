# JCR 1541-II 1 - Hybrid Commodore 1541 Disk Drive Emulator with RetroPie Support

## Optional: Adding RetroPie Support

### Install RetroPie

Obtain SD card and flash it with [RetroPie (v4.0.2 or later)](https://retropie.org.uk/)

### Configure OLED Display Support

Install and configure RetroPie OLED: https://github.com/zzeromin/RetroPie-OLED

Note that if you want to use retropie in parallel to pi1541, your PI1541 hat
must be in bus 1 mode to maintain pinout compatibility:

| pin             | PI1541 Hat (Bus 0) | PI1541 Hat (Bus 1) | RetroPie OLED |
|-----------------|--------------------|--------------------|---------------|
| GND             | (any gnd pin)      | (any gnd pin)      | pin 6         |
| 5V              | (any 5V pin)       | (any 5V pin)       | pin 4         |
| SDA             | pin 27             | pin 3              | pin 3         |
| SDL             | pin 28             | pin 5              | pin 5         |
