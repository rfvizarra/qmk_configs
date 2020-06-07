# My QMK Config files for config.gmk.fm

QMK Configuration files for https://config.qmk.fm/

# 60% Keyboards

## dz60
 * [dz60 keymap (querty) - LAYOUT_60_ansi_split_bs_rshift](./dz60/dz60_rfvizarra.json)

Flashing instructions

Plug the USB cable
Press the reset button or short the reset pads in the PCB

```bash
/usr/bin/dfu-programmer atmega32u4 erase
/usr/bin/dfu-programmer atmega32u4 flash dz60_rfvizarra.hex
/usr/bin/dfu-programmer atmega32u4 reset
```

## gh60 satan
* [gh60 satan keymap (querty) - LAYOUT_60_ansi_split_bs_rshift](./gh60_satan/gh60_satan_rfvizarra.json)

Flashing instructions

Plug the USB cable
Press the reset button or short the reset pads in the PCB

```bash
/usr/bin/dfu-programmer atmega32u4 erase
/usr/bin/dfu-programmer atmega32u4 flash gh60_satan_rfvizarra.hex
/usr/bin/dfu-programmer atmega32u4 reset
```

## playkbtw/pk60
* [pk60 keymap (querty) - LAYOUT_minila](./pk60/pk60_rfvizarra.json)

Flashing instructions

Plug the USB cable
Press the reset button or short the reset pads in the PCB

```bash
/usr/bin/dfu-programmer atmega32u4 erase
/usr/bin/dfu-programmer atmega32u4 flash pk60_rfvizarra.hex
/usr/bin/dfu-programmer atmega32u4 reset
```

# Split keyboards

Split keyboards

## Ergo

### Corne/crkbd

* [ckrbd keymap (query/custom)](./crkbd/crkbd_rfvizarra.json)

Flashing instructions

Plug the USB cable
Connect GND and RST pins for a bit or press the reset button (if available)
```bash
avrdude -p atmega32u4 -P /dev/ttyACM0 -c avr109 -U <crkbd_rfvizarra.hex>
```

## Ortho

## Let's split
TODO

Flashing instructions

Plug the USB cable
Connect GND and RST pins for a bit or press the reset button (if available)
```bash
avrdude -p atmega32u4 -P /dev/ttyACM0 -c avr109 -U <firmware.hex>
```
## Shark

TODO

Flashing instructions

```bash
dfu-util -a 0 -s 0x08000000 -D <firmware.bin>
```