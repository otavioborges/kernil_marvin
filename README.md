# Marvin Development Board

Marvin is a open-source open-hardware development board using KE02 MCU as target and a KL26 as programmer/debbuger.

## Project Details

The programmer is a MKL26ZVFM4 with a SWD header for programming, using a J-Link probe or similar. The programming/debugging hardware is based on OpenSDA projects (Freesacale FRDM boards were used as base project).

The programmer output is routted to a MKE02Z64VLD4. The KE02 family from the former Freescale uses +5V as input voltage, so the voltage range of the target would be similar to an Arduino Uno, making projects migration and shield usage simpler and straightforward.

Target breakout is similar to Arduino Uno and can be muxed so every pin have the same function as an Arduino.

## Reference files

* [KL26 Datasheet](http://www.nxp.com/assets/documents/data/en/data-sheets/KL26P121M48SF4.pdf);
* [KL26 Reference Manual](http://cache.freescale.com/files/microcontrollers/doc/ref_manual/KL26P121M48SF4RM.pdf);
* [KE02 Datasheet](http://www.nxp.com/assets/documents/data/en/data-sheets/MKE02P64M20SF0.pdf);
* [KE02 Reference Manual](http://www.nxp.com/assets/documents/data/en/reference-manuals/MKE02Z64M20SF0RM.pdf);
* [OpenSDA Project](http://www.nxp.com/products/software-and-tools/run-time-software/kinetis-software-and-tools/ides-for-kinetis-mcus/opensda-serial-and-debug-adapter:OPENSDA);
* [FRDM-KE02Z Details](http://www.nxp.com/products/software-and-tools/hardware-development-tools/freedom-development-boards/kinetis-e-series-freedom-development-platform:FRDM-KE02Z);

## Project Goals

Marvin was develop to create a pin-to-pin arduino compatible board. So hardware projects and commercial shields could be used without adaptations.

Using an ARM target the user could develop the firmware on more complete IDE (like [Kinetis Design Studio](http://www.nxp.com/products/software-and-tools/software-development-tools/kinetis-design-studio-integrated-development-environment-ide:KDS_IDE)) with debugging capabilities.

Also, all project was developed to have low production cost to keep competitive final price.
