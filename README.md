# PFM keyboard

This repo contains the hardware design for the PFM (Perfect For Me) keyboard.
This is a 38 key split keyboard which - as hinted by the name - is designed specifically for me, 
my hands, my typing habits and so on. 

![Pic](/assets/pic-v4.jpg "My keyboard")

**Outline**

![Shape](/assets/shape.svg "Outline")

In particular: 
- it has a relatively strong stagger
- the inner most index finger colum has only two keys
- the top most keys of the pinky column are actually used with the ring fingers (those keys are 
spaced a little further up)
- the outer most columns have only one key for the pinky to find.  

Together this reduces overstretching leading to better comfort and reduces the need for hand movement and my tendency to loose my home position when I do so.
Despite the name, it is still not perfect.

The keyboard is based on the [frood microcontroller](https://42keebs.eu/shop/parts/controllers/frood-rp2040-pro-micro-controller/) which allows the use of 38 keys without any diodes.

The board uses MX keys both with hot-swap sockets or directly soldered.

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
