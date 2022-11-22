# Wemos Battery Monitor with OLED Display

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This is a little analog battery monitor for my sump pump system that has
a DC battery backup.  It uses a Wemos D1 ESP8266 dev board, OLED display,
breakout board for wiring.

I added a 1.5Mohm resistor in line with the analog input, the D1 already
has a 220k ohm resister in series with a 100k ohm resistor to divide
a 3.3V signal down to 0-1V.  The 1.5Mohm resistor increases the division 
so that a 15V input is around 0.9V at the A0 pin.

I use ESPHome with Home Assistant to link data from the esp8266 into HA. 
My ESPHome code is [here in my github](https://raw.githubusercontent.com/gx1400/homeassistant/main/esphome/sump-batt-mon.yaml).
For the sake of posterity I included it in the docs folder in this repo.

# Changelog
2022/11/22 - Initial upload

# Parts

[HiLetgo 0.66 inch OLED 0.66" OLED Mini OLED Shield with I2C/IIC 64x48 Pixels 3.3V](https://smile.amazon.com/dp/B01MZYYHHD)

[Ximimark 5Sets WeMos D1 Mini Prototype Board XD-08 ProtoBoard Shield Double Sided Perf Board for Arduino](https://smile.amazon.com/dp/B07L756KQS)

## Design

Autocad Fusion 360 

## Slicer

Ultimaker Cura 4.12.1

- Printer: Creality CR6 SE

- Layer Height: 0.2mm
- Infill Density: 20%
- Infill Pattern: Grid

- Filament: Inland PETG+ 1.75mm White
- Material: PETG
- Print Temperature: 235 degrees C