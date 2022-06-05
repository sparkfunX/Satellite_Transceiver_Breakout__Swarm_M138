# Satellite Transceiver Breakout - Swarm M138

[![Satellite Transceiver Breakout - Swarm M138](https://cdn.sparkfun.com//assets/parts/1/8/8/6/3/19236-Satellite_Transceiver_Breakout_-_Swarm_M138-05_HRc.jpg)](https://www.sparkfun.com/products/19236)

[*Satellite Transceiver Breakout - Swarm M138*](https://www.sparkfun.com/products/19236)

A breakout for the Swarm M138 satellite transceiver.

This breakout allows you to power and communicate with the Swarm M138 using USB 3 or USB-C, or breakout pins.

We've written a Python3 PyQt5 GUI to let you communicate with the modem. You will find the Python code in the [**Tools**](./Tools/Swarm_M138_GUI) folder.

We've created executables for Windows and Raspberry Pi:
* On Windows:
  * Follow [this link](https://github.com/sparkfunX/Satellite_Transceiver_Breakout__Swarm_M138/raw/main/Tools/Swarm_M138_GUI/Windows%20exe/Swarm_M138_GUI.exe) to download the executable
  * Run Swarm_M138_GUI.exe from File Explorer or a Command Prompt window
* On Raspberry Pi:
  * Follow [this link](https://github.com/sparkfunX/Satellite_Transceiver_Breakout__Swarm_M138/raw/main/Tools/Swarm_M138_GUI/Raspberry%20Pi%20exe/Swarm_M138_GUI) to download the executable
  * Open a terminal window
  * cd Downloads
  * sudo chmod 755 Swarm_M138_GUI
  * ./Swarm_M138_GUI

Don't panic! The GUI will take a few seconds to open. Select the correct port from the drop-down list, click Open Port and away you go!

Click any of the pre-defined message buttons to send that message to the modem. Or enter your own message in the Message window and click Send Message to send it.
The $, * and checksum are added automatically. You do not need to include those.

You will find the modem manual in the [**Documents**](./Documents) folder. It contains the full list of modem commands and messages.

You can also integrate the satellite transceiver directly into your project; the breakout pads can be used to provide power and access the 3.3V UART TX and RX signals.

Open the two split jumper pads on the bottom of the PCB first, located between the TXO/CH340_RXI and RXI/CH340_TXO pads. Then connect:
* GND to GND on your Arduino board
* VIN to 5V/V_USB on your Arduino board
* TXO to RX on your Arduino board (3.3V only!)
* RXI to TX on your Arduino board (3.3V only!)

Our [Swarm Satellite Arduino Library](https://github.com/sparkfun/SparkFun_Swarm_Satellite_Arduino_Library) makes communicating with the modem really easy.

## Repository Contents

- [**/Hardware**](./Hardware) - contains the Eagle PCB, SCH and LBR design files
- [**/Documents**](./Documents) - contains the datasheet etc. for the Swarm M138
- [**/Tools**](./Tools) - contains the Python3 PyQt5 Swarm_M138_GUI
- [**LICENSE.md**](./LICENSE.md) - contains the licence information

## Product Versions

- [SPX-19236](https://www.sparkfun.com/products/19236) - Original SparkX Release.

## License Information

This product is _**open source**_!

Please review the LICENSE.md file for license information.

If you have any questions or concerns on licensing, please contact technical support on our [SparkFun forums](https://forum.sparkfun.com/viewforum.php?f=123).

Distributed as-is; no warranty is given.

- Your friends at SparkFun.
