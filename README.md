# Wave <!-- omit from toc -->

![Wave v0.0.1 + MBK Blank Keycaps Image](/resources/images/built_wave_1.jpeg) <sub>Wave v0.0.1 + MBK Blank Keycaps</sub>

<span>
    <a href="https://github.com/etiennecollin/wave/commits">
        <img src="https://img.shields.io/github/last-commit/etiennecollin/wave">
    </a>
    <a href="https://github.com/etiennecollin/wave/releases/latest">
        <img src="https://img.shields.io/github/v/release/etiennecollin/wave?include_prereleases&color=success">
    </a>
    <a href="https://github.com/etiennecollin/wave/blob/main/LICENSE">
        <img src="https://img.shields.io/static/v1?label=license&message=GPL-3.0&color=success">
    </a>
    <a href="https://github.com/qmk/qmk_firmware/tree/master/keyboards/etiennecollin/wave">
        <img src="https://img.shields.io/static/v1?label=firmware&message=QMK&color=orange">
    </a>
</span>

---

- [What Is It](#what-is-it)
- [Features](#features)
- [Components List](#components-list)
    - [Keyboard](#keyboard)
    - [Plates Kit](#plates-kit)
- [Ordering the PCBs](#ordering-the-pcbs)
    - [Keyboard](#keyboard-1)
    - [Plates kit](#plates-kit-1)
        - [Switch Plates](#switch-plates)
        - [Back Plates](#back-plates)
- [QMK Firmware](#qmk-firmware)

## What Is It

The Wave is a small, reversible keyboard inspired by the [Ferris](https://github.com/pierrechevalier83/ferris), the [Ferris Sweep](https://github.com/davidphilipbarr/Sweep), the [Swoop](https://github.com/jimmerricks/swoop) and the [Sweep36](https://github.com/sadekbaroudi/sweep36). It aims to solve a few issues I found with the keyboards (see [Features](#features)).

## Features

-   Choc V1 switches
    -   The switches can be soldered, or hot swapped using either Mill-Max or Kailh hot swap sockets
-   Choc spacing (supports MBK keycaps)
-   1.5u thumb key support
-   Diode-less build
-   Reversible PCB
-   USB-C
-   Mini DIN 4 (S-Video) connector used to connect both halves of the keyboard
    -   The issue with TRRS connectors is that [they are not hot swap](https://docs.qmk.fm/#/feature_split_keyboard?id=considerations); disconnecting the cable while the keyboard is powered via usb risks damaging/breaking the controller by shorting the VCC pin to a GND or data pin.
    -   The Mini DIN 4 connector solves this issue and is readily available on the market, being the cable used for S-Video.
-   Switch plate and back plate available

## Components List

### Keyboard

Here are the **required** components to build the Wave:

-   2x Keyboard PCBs (PCB manufacturers usually sell them in multiples of 5)
-   2x Elite-C V4 controllers
-   36x Choc V1 switches
-   36x MBK compatible keycaps
-   2x Mini DIN 4 Jack ([MDJ-004-FS](https://www.digikey.ca/en/products/detail/adam-tech/MDJ-004-FS/9832525))
-   1x Mini DIN 4 (S-Video) cable
-   1x USB-C Cable to connect to computer

Here are the **optional** components to build the Wave:

-   Hot swap sockets, either:
    -   36x Kailh hot swap sockets for Choc switches
    -   72x Mill-Max hot swap sockets (preferably [3305](https://www.digikey.ca/en/products/detail/mill-max-manufacturing-corp/3305-1-15-15-47-27-10-0/13901953) or [7305](https://www.digikey.ca/en/products/detail/mill-max-manufacturing-corp/7305-0-15-15-47-27-10-0/1765737) sockets as they have a thinner profile)
-   2x reset switches ([B3U-1000P-B](https://www.digikey.ca/en/products/detail/omron-electronics-inc-emc-div/B3U-1000P-B/1811777))
    -   The B3U-1000PM, B3U-1000P-B and B3U-1000PM-B variants will work as they have the same footprint.
-   10x Rubber feet/bumpers (I like these [RBS-12BK](https://www.digikey.ca/en/products/detail/essentra-components/RBS-12BK/3814603))

### Plates Kit

-   2x Switch plate PCBs (PCB manufacturers usually sell them in multiples of 5)
    -   The switch plates may be used without back plates.
-   2x Back plate PCBs (PCB manufacturers usually sell them in multiples of 5)
    -   The back plates **require** switch plates to screw into.
-   5x M2 6mm spacer ([970060244](https://www.digikey.ca/en/products/detail/w%C3%BCrth-elektronik/970060244/9488532))
-   10x M2 3mm screws ([I like these torx screws](https://www.ebay.ca/itm/154354213469?var=454428568064))

## Ordering the PCBs

### Keyboard

![Wave PCB Image](/resources/images/wave_pcb_rounded.svg)

<sub>Wave PCB</sub>

To order the keyboard PCB, the following settings are recommended[^1]:

| Detail                  | Value                     |
| ----------------------- | ------------------------- |
| Gerber file             | `Wave_0.0.1.zip`          |
| Base material           | FR-4                      |
| Layers                  | 2                         |
| Different design        | 1                         |
| Delivery format         | Single PCB                |
| PCB thickness           | **1.6mm**                 |
| PCB color               | (Personal preference)     |
| Silkscreen              | (Personal preference)     |
| Surface finish          | (Personal preference)[^2] |
| Outer copper weight     | 1oz                       |
| Via Covering            | Tented                    |
| Board Outline Tolerance | ±0.2mm(Regular)           |
| Confirm production file | No                        |
| Remove order number     | Yes                       |
| Gold Fingers            | No                        |
| Castellated holes       | No                        |

### Plates kit

You will need to order two different PCBs; the switch plate one and the back plate one.

#### Switch Plates

![Wave Switch Plate PCB Image](/resources/images/switch_plate_pcb.svg)

<sub>Wave Switch Plate PCB</sub>

![Wave v0.0.1 Switch Plate Image](/resources/images/built_wave_2.jpeg) <sub>Wave v0.0.1 Switch Plate</sub>

To order the switch plate PCB, the following settings are recommended[^1]:

| Detail                  | Value                         |
| ----------------------- | ----------------------------- |
| Gerber file             | `Wave_Switch_Plate_0.0.1.zip` |
| Base material           | FR-4                          |
| Different design        | 1                             |
| Layers                  | 2                             |
| Delivery format         | Single PCB                    |
| PCB thickness           | **1.2mm**                     |
| PCB color               | (Personal preference)         |
| Silkscreen              | (Personal preference)         |
| Surface finish          | (Personal preference)[^2]     |
| Outer copper weight     | 1oz                           |
| Via Covering            | Tented                        |
| Board Outline Tolerance | ±0.2mm(Regular)               |
| Confirm production file | No                            |
| Remove order number     | Yes                           |
| Gold Fingers            | No                            |
| Castellated holes       | No                            |

#### Back Plates

![Wave Back Plate PCB Image](/resources/images/back_plate_pcb.svg)

<sub>Wave Back Plate PCB</sub>

![Wave v0.0.1 Back Plate Image](/resources/images/built_wave_3.jpeg) <sub>Wave v0.0.1 Back Plate</sub>

To order the back plate PCB, the following settings are recommended[^1]:

| Detail                  | Value                       |
| ----------------------- | --------------------------- |
| Gerber file             | `Wave_Back_Plate_0.0.1.zip` |
| Base material           | FR-4                        |
| Different design        | 1                           |
| Layers                  | 2                           |
| Delivery format         | Single PCB                  |
| PCB thickness           | **1.6mm**                   |
| PCB color               | (Personal preference)       |
| Silkscreen              | (Personal preference)       |
| Surface finish          | (Personal preference)[^2]   |
| Outer copper weight     | 1oz                         |
| Via Covering            | Tented                      |
| Board Outline Tolerance | ±0.2mm(Regular)             |
| Confirm production file | No                          |
| Remove order number     | Yes                         |
| Gold Fingers            | No                          |
| Castellated holes       | No                          |

## QMK Firmware

The [latest firmware](https://github.com/qmk/qmk_firmware/tree/master/keyboards/etiennecollin/wave) can be found on the official [QMK](https://github.com/qmk/qmk_firmware/tree/master) repository.

<a href="(https://github.com/qmk/qmk_firmware/tree/master/keyboards/etiennecollin/wave">
    <img width=33% src="resources/icons/qmk_badge_dark.png">
</a>

[^1]: Settings are for [JLCPCB](https://jlcpcb.com/), but should be similar with other manufacturers.
[^2]: ROHS or lead-free options should be preferred (LeadFree HASL).
