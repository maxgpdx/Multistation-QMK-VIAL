# Multistation QMK VIAL Firmware

![keyboard](https://i.imgur.com/Vkb3qoN.jpeg)

This is the firmware I used for my IBM 5556 Multistation Keyboard to convert it to USB using QMK/VIAL. This is done through the MCU swap method, replacing the keyboard controller with a Raspberry Pi Pico wired into the keyboard matrix. This is untested, but unlikely to work with the later 2nd gen PCBs found on keyboards with PBT cylindrical keycaps. Note: buzzer is not implemented.

* Keyboard Maintainer: maxgpdx
* Hardware Supported: IBM 5556 Multistation keyboards with first gen PCB, Raspberry Pi Pico
* Hardware Availability: Yahoo Auctions JP

Instructions:

* Desolder all components (resistors, capactiors, MCU, etc.) from original logic section of the keyboard
* Wire pins of Pi Pico to the matrix pins shown in the below table and matrix map
* Flash and test firmware


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
