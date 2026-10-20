# Ultimate Weather

7 inch touchscreen desk for one US town. Lightning within 25 miles, today's earthquakes, radar, the clock, the night sky, rocket launches, and the space station.

Board: Waveshare ESP32-S3-Touch-LCD-7, 800 by 480.

Version on the desk: 1.0

## Folders

`ota` is what the desk downloads.
CHECK reads `ota/version.txt`.
INSTALL reads `ota/sky_7in.bin`.

`sketch` is `ultimate_weather.ino`, `usa_map.h`, and `iss_world.h`.
Open that folder in the Arduino IDE. The folder name matches the sketch name.

`libraries` has three folders.
GFX Library for Arduino 1.6.8.
TJpg_Decoder 1.1.0.
ArduinoJson 7.4.2 by Benoit Blanchon. That is the library kept for these desks. It is not Arduino_JSON.
Copy those folders into your Arduino libraries folder.

`ARDUINO-IDE.txt` is the Tools menu from the compile that made this firmware.

`Ultimate-Weather-User-Manual.pdf` is the printed manual.

## Update from the desk

SET, then ABOUT, then CHECK FOR UPDATES.
If `ota/version.txt` is a higher number than the version on the desk, tap INSTALL.
Leave the desk plugged in until it restarts.

A desk already on 1.0 says the newest firmware is already installed.
Raise the version in the sketch and in `ota/version.txt` together when you ship a newer bin.

The desk looks at this repo:

https://github.com/stefi01/Ultimate-Weather-Station-Earthquake-Lightning-ISS
