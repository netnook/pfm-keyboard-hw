# PFM keyboard

This repo contains the hardware design for the PFM (Perfect For Me) keyboard.  This is a 38 key split keyboard which - as hinted by the name - is designed specifically for me, my hands, my typing habits and so on.  Despite the name, it is not perfect.


![Shape](/assets/shape.svg)

The keyboard is based on the [frood microcontroller](https://42keebs.eu/shop/parts/controllers/frood-rp2040-pro-micro-controller/) which allows the use of 38 keys without any diodes.

QMK based firmware for this board is available in the [pfm-keyboard-fw](https://github.com/netnook/pfm-keyboard-fw) repo.

## Schematic

![Schematic](/assets/schematic.svg)

[Schematic as PDF](/assets/schematic.pdf)

## Parts

- 2x [frood microcontroller](https://42keebs.eu/shop/parts/controllers/frood-rp2040-pro-micro-controller/)
- sockets for MCU (optional)
- OLED display (link ?)
- sockets for display (this also allows bridging the distance required to allow the display to lay above the mcu - long pins could be used instead)
- 38x MX switches and keycaps of choice 
- 38x MX sockets - (optional - PCB can be used with or without sockets)
- 1 or 2 reset switches such as [this](https://42keebs.eu/shop/parts/components/reset-switch/?attribute_type=Through-hole%202-pin%206x3&attribute_pa_colour=black) - (optional - right hand side only needs programming once and the tiny reset switch on the mcu does the job, for the left hand side which is re-programmed with every layout change the switch is convenient to have)
- piezo buzzer (source ?)
- 2x TRRS socket such as [this](https://42keebs.eu/shop/parts/components/pj-320-trrs-socket/?attribute_type=PJ-320A%20(Through-Hole)&attribute_pa_colour=black)
- 1x TRRS or TRS cable
- USB cable for connection to PC
- rubber feet (8mm diameter, at least 2mm thick - preferably 3mm thick)
