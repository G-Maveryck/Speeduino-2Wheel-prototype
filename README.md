# What is this ?
This project aim to build an Open-Source Engine Control Unit (aka ECU), fully programmable, accessible and modifiable, specificaly designed for motorcycles. It is still in "protoype" stage.
The goal is to end with a solution suited retro-fit purposes : Lowering fuel consumption, pollution, and incearing performances.

It's build around the DIY-EFI's CORE4 board, with a custom "Daughter board", and use the Speeduino firmware.
The CORE4 board is current choice for it's compact footprint, and fully featured board.
The Speeduino firmware can be found on it's own repo (See Licenses part for more informations.

# Electronics and Hardware parts
As the CORE4 is kind of a "all-in-one" solution, this current project focuses on building a "Daughter board" to "host" the CORE4.
The CORE4 board implement the Arduino and the speeduino board, in the same board and a compact form factor.

The goal of the Daughter-Board is to implement all the electronics needed to work correctly, and to be mounted easily on a bike.
It include a proper automotive connector, routing the sensors signals to the pin of the CORE4, and implement the essential electronics directly on the board (see the "Specific parts" section for more informations).

In this early state (v0.1), the ignitions drivers, VR Conditionner and MAP Sensor are mounted directly on the board.

# Workflow & Tools
The electronics parts (PCB and Schematics) are designed using KiCad EDA 8.0.
The other CAD parts (eg. enclosure, boxes, etc..) are designed using Solidworks 2023, and additionnaly distributed in .STEP file format.

# Specific parts
For the purposes of this project, some parts have been selected as "default" part. This includes :
- Main I/O connector : Molex CMC 48way  - Black (500762-0481 PCB Header / 64320-3311 Female connector)
- MAP Sensor : MPXHZ6250-AC6T1 from Freescale
- Ignition Coil Driver : build around FGP3440G2-F085 IGBT transistor from On-Semi.
- VR Conditionners : Based on the "Dual VR Conditionner" from the official Speeduino project, with the MAX9926 chip. In this case, the circuit is directly welded on the board.

# Licenses
This project is distributed under the terms of the "CERN Open Hardware Licence Version 2 - Strongly Reciprocal" License.
See LICENSE.md for more information.

It is based on many open-source contributions, mainly the Speeduino Project (github :  https://github.com/noisymime/speeduino / https://github.com/speeduino/Hardware) wich is distributed under CERN Open Hardware License v2 Strong (CERN-OHL-S) for hardware, and GPL-2.0 for the firmware.
All informations about the DIY-EFI's CORE4 can be found here : https://diy-efi.co.uk/knowledge-base/core4-universal-getting-started

# Support and Contribution
If you want to get involved in this project, feel free to contribute, clone or fork this repo. Feel free to submit a pull request if you have any contribution.
To join the developpement, please contact me at : wulveryck.gabriel@gmail.com (more information on my Github profile)
A lot of work still need to be done. This include building, testing, and building the best and also cheaper solution for specific uses !
All help is welcome !
