# JCR 1541-II 1 - Hybrid Commodore 1541 Disk Drive Emulator with RetroPie Support

## Software Setup: PI1541

TODO

## Optional: Adding RetroPie Support

### Install RetroPie

Obtain SD card and flash it with [RetroPie (v4.0.2 or later)](https://retropie.org.uk/)

### Configure OLED Display Support

For hardware pinout compatibility, make sure your PI1541 Hat is configured to use bus 1 (see table above).

| pin             | PI1541 Hat (Bus 0) | PI1541 Hat (Bus 1) | RetroPie OLED |
|-----------------|--------------------|--------------------|---------------|
| GND             | (any gnd pin)      | (any gnd pin)      | pin 6         |
| 5V              | (any 5V pin)       | (any 5V pin)       | pin 4         |
| SDA             | pin 27             | pin 3              | pin 3         |
| SDL             | pin 28             | pin 5              | pin 5         |

#### Using SSD1306 OLED 128x64

Install and configure RetroPie OLED (https://github.com/zzeromin/RetroPie-OLED):

    sudo apt-get update
    cd /home/pi
    git clone https://github.com/losernator/RetroPie-OLED.git
    cd RetroPie-OLED
    chmod 755 11.OLED.sh
    sudo ./11.OLED.sh

#### Using SSD1306 OLED 128x32

TODO
