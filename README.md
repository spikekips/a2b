<!--<div align="center">-->

# a2b - Audio & Power to Breadboard Interface

[![GitHub stars](https://img.shields.io/github/stars/spikekips/a2b?style=for-the-badge)](https://github.com/spikekips/a2b/stargazers)

[![GitHub forks](https://img.shields.io/github/forks/spikekips/a2b?style=for-the-badge)](https://github.com/spikekips/a2b/network)

[![GitHub issues](https://img.shields.io/github/issues/spikekips/a2b?style=for-the-badge)](https://github.com/spikekips/a2b/issues)

[![GitHub license](https://img.shields.io/github/license/spikekips/a2b?style=for-the-badge)](LICENSE)

**A convenient open-source hardware interface board for integrating 1/4" audio and 9V DC power with breadboard projects.**

<!-- </div> -->

## Overview

The `a2b_u_d` project provides an open-source hardware solution for seamlessly integrating common audio and power sources directly into your breadboard experiments. This board is designed to take standard 1/4" audio input jacks and a 9V DC power input, breaking them out into breadboard-friendly header pins.

Whether you're prototyping audio circuits, experimenting with effects pedals, or simply need a stable power supply for your digital or analog breadboard designs, `a2b_u_d` simplifies the connection process, reducing clutter and the need for awkward jumper wire setups. It's ideal for hobbyists, educators, and professional engineers working on audio electronics and general prototyping.

## Features

-   **1/4" Audio Input Jacks**: Standard stereo 1/4" (6.35mm) jacks for easy connection of audio sources.
-   **9V DC Power Input**: A dedicated 9V DC jack for powering the board and providing a stable voltage to your breadboard.
-   **Breadboard-Friendly Output**: Standard 0.1" (2.54mm) header pins for direct connection into a breadboard.
-   **Comprehensive KiCad Design**: Full schematic and PCB layout files provided for transparency, customization, and learning.
-   **Ready-to-Manufacture Files**: Includes Gerber files and a Bill of Materials (BOM) for easy PCB fabrication and component sourcing.
-   **Open Hardware**: Licensed under CERN-OHL-S-2.0, promoting collaboration and reuse.

## Renders & Photos
[<img width="882" height="825" alt="image" src="https://github.com/user-attachments/assets/38faa650-aca6-4a1a-9365-aff10bbd1636" />](https://github.com/spikekips/a2b/blob/u_d/My_Library/Pictures/a2b_back.png?raw=true)

[<img width="882" height="825" alt="image" src="https://github.com/user-attachments/assets/414d04e8-8e45-4a31-9c5c-b4d51fab0f2f" />](https://github.com/spikekips/a2b/blob/u_d/My_Library/Pictures/a2b_front.png?raw=true)


[<img width="882" height="825" alt="image" src="https://github.com/spikekips/a2b/blob/u_d/My_Library/Pictures/a2b_side.png?raw=true" />](https://github.com/spikekips/a2b/blob/u_d/My_Library/Pictures/a2b_side.png?raw=true)



<!-- TODO: Add actual 3D renders or photos of the physical PCB/assembled board here. -->
<!-- Example:

![PCB Top View Render](path-to-top-view.png)
_3D Render: Top View of the a2b board_

![PCB Bottom View Render](path-to-bottom-view.png)
_3D Render: Bottom View with component outlines_

![Assembled Board Photo](path-to-assembled-board.jpg)
_Photo: An assembled a2b board connected to a breadboard_
-->

## Tech Stack

**ECAD Software:**

![KiCad](https://img.shields.io/badge/KiCad-EDA%20Suite-00A99C?style=for-the-badge&logo=kicad&logoColor=white)

Ver. 10.0 or greater

## Getting Started (Building & Ordering)

This project is hardware-focused, meaning "getting started" involves either reviewing the design files in KiCad or preparing the files for manufacturing.

### Prerequisites

-   **KiCad EDA Suite**: To view, modify, or export the design files. You can download it from [kicad.org](https://www.kicad.org/).

### Design Files

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/spikekips/a2b.git
    cd a2b
    ```

2.  **Open in KiCad**:
    *   Launch KiCad.
    *   Open the project file `a2b.kicad_pro`.
    *   You can then open `a2b.kicad_sch` for the schematic and `a2b.kicad_pcb` for the PCB layout.

### Manufacturing Your Own Board

The repository includes all necessary files to order the `a2b` PCB and assemble it yourself.

1.  **Gerber Files**:
    *   The `gerber.zip` archive contains all the necessary files for PCB fabrication (e.g., copper layers, solder mask, silkscreen, drill files).
    *   You can upload this `.zip` file directly to most PCB manufacturers (e.g., JLCPCB, PCBWay, OSH Park).
    *   An unzipped `gerber` directory is also provided for review.

2.  **Bill of Materials (BOM)**:
    *   The `bom/` directory should contain the list of electronic components required for assembly.
    <!--*-->   <!-- TODO: Confirm the exact format and location of the BOM file (e.g., bom/a2b_bom.csv) and provide instructions. -->
    *   You can use this BOM to source components from distributors like Digi-Key, Mouser, or LCSC.

3.  **Assembly**:
    *   Once you receive the PCBs and components, assemble them by soldering the components onto the board according to the schematic (`a2b.kicad_sch`) and the PCB layout (`a2b.kicad_pcb`).
    *   Refer to the silkscreen markings on the PCB for component placement.

<!--
## Project Structure

```
a2b/
├── .history/               # Internal historical data (can be ignored)
├── My_Library/             # Custom KiCad footprints or symbols
├── a2b-backups/            # Backups of KiCad design files
├── a2b.kicad_pcb           # Main PCB layout file
├── a2b.kicad_prl           # KiCad project local settings
├── a2b.kicad_pro           # Main KiCad project file
├── a2b.kicad_sch           # Main schematic file
├── a2b.zip                 # Archive of the project (or specific output)
├── bom/                    # Directory for Bill of Materials files
├── customHeaders.bak       # Backup file, likely related to KiCad headers
├── fp-lib-table            # KiCad footprint library table configuration
├── gerber/                 # Unzipped Gerber files for PCB manufacturing
├── gerber.zip              # Zipped Gerber files for PCB manufacturing
├── license.md              # CERN Open Hardware Licence file
├── README.md               # This README file
└── sym-lib-table           # KiCad symbol library table configuration
```
-->

## Usage & Pinout

The a2b board is designed to be plugged directly into a breadboard. The output header provides audio input and output along with 9V in.

T R S is your audio signal if you plug in a 1/4" jack into the plugs you can output the signal to your bread board or jump them to make a passthrough.

Your voltage outputs are determined by the polarity of your power supply. Wether or not you have a positive or negative center pin on your powersupply is determined by the LEDs. Determine the polarity from which light is on. The polarity symbol on the lit up side will be your reference for your Vout.

<!-- TODO: Add a clear diagram or table explaining the pinout of the breadboard headers and how to connect audio/power inputs. -->
<!-- Example:
### Connecting to a Breadboard

The `a2b` board is designed to be plugged directly into a breadboard. The output header provides:

| Pin | Description            |

|-----|------------------------|

| VCC | 9V DC regulated output |

| GND | Ground                 |

| L_A | Left Audio Channel     |

| R_A | Right Audio Channel    |

Connect your 1/4" audio source to the input jacks and a 9V DC power supply to the barrel jack.
-->

## Contributing

This is an open-source hardware project, and we welcome contributions! If you have suggestions for improvements, find errors in the design, or want to contribute to documentation:

1.  **Fork the repository.**
2.  **Create your feature branch:** `git checkout -b feature/AmazingFeature`
3.  **Make your changes.**
4.  **Commit your changes:** `git commit -m 'Add some AmazingFeature'`
5.  **Push to the branch:** `git push origin feature/AmazingFeature`
6.  **Open a Pull Request.**

Please ensure your contributions adhere to the [CERN Open Hardware Licence Version 2 - Strongly Reciprocal](license.md).

### Development Setup for Contributors
To contribute to the design files, you'll need the KiCad( > 10.0) EDA Suite installed. After cloning, simply open the `a2b.kicad_pro` file in KiCad.

## License

This project is licensed under the [CERN Open Hardware Licence Version 2 - Strongly Reciprocal](license.md) - see the `license.md` file for full details.

## Acknowledgments

-   **KiCad Community**: For providing an excellent open-source ECAD suite that makes projects like this possible.

## Support & Contact

-   Issues: [GitHub Issues](https://github.com/spikekips/a2b/issues)
-   Feel free to reach out to the repository owner, [spikekips](https://github.com/spikekips), for questions or support.

---

<div align="center">

**Star this repo if you find it helpful!**

Made by me, [spikekips](https://github.com/spikekips)

</div>

