# Kimera_Base
Open-source hardware project consisting of the creation of a device capable of connecting to the Meshtastic network, compatible with the Hydra project, but simplifying its construction.

## Features

The goal of this project is to create a device that facilitates the installation of powerful, stationary meshtastic nodes.

The following starting parameters are established:

> 1.- It will have a permanent connection to an external power source via USB-C, so no additional electronics will be required to connect it to batteries or solar panels.

> 2.- The radio frequency module will have sufficient power reserves, although it will later be adjusted to meet the legal limits of the country where it is deployed.

> 3.- The design is for a stationary node and does not require GPS hardware.

> 4.- The design will focus on supporting node interconnection, so any type of hardware that adds additional telemetry is ruled out.

> 5.- It must be compatible with a recognized firmware.

> 6.- It must be accessible by both BLE and Wifi.

The firmware that best fits the stated objective is the one developed by the Hydra project (https://github.com/Hydra-Designs/project-hydra-meshtastic-pcb) and is the one we are planning to use.

The elements used in the project would be:

> 1.- PBC developed by the project whose Gerber files will be published on this same site.

> 2.- E22-900M30S as a radio module.

> 3.- ESP32-DevKitC with ESP32-WROOM-32D or ESP32-WROOM-32U as controller.

Starting with version 0.4, the RF element is separated into a plug-in module called the Kimera E22, and a 5V boost is added to power this module.

Latest version tested: https://github.com/TheClanLabs/TheClanKimera/tree/main/KimeraBase/KimeraBaseV-0.2

Current version in development: https://github.com/TheClanLabs/TheClanKimera/tree/main/KimeraBase/KimeraBaseV-0.4

## Disclaimer

Regardless of the status of the Kimera project described on this site, the authors are not responsible for its proper functioning or misuse, nor for any physical or moral damage that may be suffered by anyone who uses the information provided here.
