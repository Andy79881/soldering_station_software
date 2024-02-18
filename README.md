# Software for soldering-station

Content description
----

This repository contains the source code to the [soldering_station](https://github.com/Andy79881/soldering_station) project including the required directory structure and files to setup a VSCode project using PlatformIO plugin. For detailed description about the project itself, please check out the main repository.  
 
The current software I'm using is release 2.8 with my modifications. 
Below you find the changes to the original design from [ArduinoHannover/Maiskolben](https://github.com/ArduinoHannover/Maiskolben)

Baseline:
---
- code is based on release 2.8, which is the latest code supporting TFT displays based on ST7735. Note: V3.x is based on a different display library (ILI9163C).

Changes to original design and code:
----

- TFT backlight output added (Arduino pin D0). Backlight can be adjusted via potentiometer (no PWM controlled TFT brightness)
- modified definitions.h to cope with customized key layout and adding pin definition of TFT backlight discrete output (TFT_BL)
- old fashioned ino file converted into cpp file format by following two steps (see [ino-to-cpp](https://docs.platformio.org/en/latest/faq/ino-to-cpp.html)).

Design decisions:
----
- software environment changed to VSCode using PlatformIO plugin (library dependencies added into platformio.ini)

Final Remarks:
---
- Code is provided **AS IS**, so no warranties.
- Code size is actually close to the limits. This may be also caused by using the latest library versions. Be aware of this if you make the build by yourself.

   
