# Nederman Exhaust System Control Panel Replacement
|Original|Replacement|
|:-:|:-:|
|<img src="images/Original Control Panel.jpg" alt="Original Nederman Control Panel" width="300"/>|<img src="images/Replacement Panel.jpg" alt="Replacement Control Panel" width="300"/> TODO: add replacement panel image|


As our Nederman Exhaust Extraction System had more and more faults with the digital control panel, a replacement was needed. The original control panel had a display, multiple buttons and a complete control menu.
The protection circuits like the fan motor current "measurement?" and the exhaust air flow measurement had more and more false alarms and made using the exhaust system impossible.
The control system consists of the aforementioned intelligent control panel and an "I/O" PCB in the control cabinet, next to power contactors, power supply and other stuff.

The [images](images/) folder contains more photos of the control cabinet and the I/O Basis PCB.

So a new VERY basic control panel was developed. We thought about building something intelligent with an Arduino or ESP32, analog measurement of the currents and air flow, but this was quickly pushed aside, as we needed the exhaust system ASAP.

The new control panel has only two switches and four LEDs:
* Fan motor on/off switch with LED
* Filter cleaning motor on/off switch with LED
* A power LED
* A dust container sensor LED

This repo contains a reverse engineered circuit of the I/O Basis PCB where the "digital" control stuff was reverse engineered. Enough to switch all functions in the exhause system. The analog motor current measurement and air flow sensor stuff was omitted, as it was not very interesting. Sure, omitting protections is not the best habbit, but this is hobby stuff and needed as fast as possible. And the fan motor gets a proper motor protection switch, so it has an independent protection where the intelligent control panel is not needed.


# License
The content of this whole repository is licensed under [CERN-OHL-W v2](License/cern_ohl_w_v2.txt) or later by Jonas Eberhard
