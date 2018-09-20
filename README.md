# Arduino-WS2811-rotary-RGB-led-strip

### Libraries
- NeoPixelBus by Makuna (https://github.com/Makuna/NeoPixelBus/wiki)
- Encoder (https://www.pjrc.com/teensy/td_libs_Encoder.html)
- (MemoryUsage (https://github.com/Locoduino/MemoryUsage))

Fast HSV -> RGB: http://www.vagrearg.org/content/hsvrgb

Can't use assembler version:
```
error: r28 cannot be used in asm here
error: r29 cannot be used in asm here
```
Google says that works with optimization level 1, but I don't know easy way to change optimization level.

### Usage
- Rotate to change brightness.
- Click and after that rotate to change color/temperature.
- 1s click saves parameters.
- 2s click goes to rainbowmode, where you can change brightness and after click speed.

![Image](https://github.com/mcgurk/Arduino-WS2811-rotary-RGB-led-strip/raw/master/Arduino_UNO_WS2811-ledstrip_with_rotaryencoder.jpg)

- Databus to pin2

- 150pcs WS2811 leds with 1/2 brightness and rainbow-colors takes 5V/3A
- 150pcs WS2811 leds with 1/4 brightness and rainbow-colors takes 5V/2A

- ATmega32u4 SRAM: 2560B (~600 RGB leds)
- ATmega328p SRAM: 2048B (~? RGB leds)
