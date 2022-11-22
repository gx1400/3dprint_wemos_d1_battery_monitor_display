# Wemos Battery Monitor with OLED Display

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