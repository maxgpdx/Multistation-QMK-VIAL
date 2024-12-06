# Multistation QMK VIAL Firmware

![keyboard](https://i.imgur.com/Vkb3qoN.jpeg)

This is the firmware I used for my IBM 5556 Multistation Keyboard to convert it to USB using QMK/VIAL. This is done through the MCU swap method, replacing the keyboard controller with a Raspberry Pi Pico wired into the keyboard matrix.

* Keyboard Maintainer: maxgpdx
* Hardware Supported: IBM 5556 Multistation keyboards with first gen PCB, Raspberry Pi Pico
* Hardware Availability: Good luck

Wiring:

| Row:     | GPIO:   |  COL:   |  GPIO:  |      
| -------- | ------- | ------- | ------- |
| 0 | gp27 | 0 | gp6  |
| 1 | gp28 | 1 | gp7  |
| 2 | gp26 | 2 | gp8  |
| 3 | gp22 | 3 | gp9  |
| 4 | gp21 | 4 | gp10 |
| 5 | gp20 | 5 | gp11 |
| 6 | gp19 | 6 | gp12 |
| 7 | gp18 | 7 | gp13 |
|  |  | 8 | gp14 |
|  |  | 9 | gp15 |
|  |  | 10 | gp5 |
|  |  | 11 | gp0 |
|  |  | 12 | gp1 |
|  |  | 13 | gp2 |
|  |  | 14 | gp3 |
|  |  | 15 | gp4 |


![wiring](https://i.imgur.com/7PAu3PK.jpeg)
