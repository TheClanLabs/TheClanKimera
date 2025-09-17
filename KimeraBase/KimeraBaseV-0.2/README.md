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

The circuit diagram would be:


![Scheme v-0.2](https://github.com/TheClanLabs/TheClanKimera/blob/main/KimeraBase/KimeraBaseV-0.2/Scheme_Kimera_V-0.2.png)

And the appearance would be:

![3D-Top](https://github.com/TheClanLabs/Kimera_Base/blob/main/Kimera_1.png)
![3d-Bak](https://github.com/TheClanLabs/Kimera_Base/blob/main/Kimera_2.png)

## Project status

> 5/8/2025 Request to JLCPCB for 5 boards for the Kimera V-0.2 prototype. (7.22€)

> 6/8/2025 The component E22-900M30S was ordered from Aliexpress. (8.09€)

> 7/8/2025 The board ESP32-DevKitC with ESP32-WROOM-32U was ordered from Aliexpress. (3.79€)

> 19/8/2025 Received from Aliexpress the board ESP32-DevKitC and the component E22-900M30S

> 19/8/2025 Testing Meshtastic firmware installation on ESP32-WROOM-32U successfully.

> 30/8/2025 The components were welded and integrated into the Madrid mesh for testing.

## To be kept in mind for the following versions

> The E22-900M30S documentation recommends avoiding PCB traces from passing under the component. In version 0.2, some traces do not meet this recommendation, so future versions will require this recommendation, even if it means increasing the board width.

> When the kit is connected via USB, the 5V pin outputs less than 5 volts, as it is a 5V USB connection that passes through a Schottky diode with its corresponding voltage drop. Although the RF module can operate with less than 5V, the recommendation is to get as close to 5V as possible. The solution may be to use a different socket for the power supply and reserve the USB socket for the firmware update.

## Disclaimer

Regardless of the status of the Kimera project described on this site, the authors are not responsible for its proper functioning or misuse, nor for any physical or moral damage that may be suffered by anyone who uses the information provided here.
