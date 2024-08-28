# WackyMXter
my custom keyboard.

<img src="https://github.com/user-attachments/assets/92aabbbd-c5f9-47da-8a6e-8b23993bd66b" height="250">

<img src="https://github.com/user-attachments/assets/4d612e4a-11ab-43f6-9708-688bf1b574e6" height="250">

<img src="https://github.com/user-attachments/assets/c8f8a93b-82ec-4d33-b132-0cdb13695e21" height="250">


## Features
- Wireless (bluetooth)
- Split (two halves can also be independent)
- Supports Choc and MX hotswap switches
- Ergonomic (for my hands at least)
- ZMK Support

## Project Format
- `gerber/`: Gerber files for the left and right side (includes BOM and placement files for assembly of shift register and diodes)
- `layout-editor/`: Layout of the keyboard for use at [keyboard layout editor](http://www.keyboard-layout-editor.com/)
- `pcb/`: KiCad files
- `zmk-firmware/`: Links to the ZMK firmware repo: [WackyMXter-zmk-firmware](https://github.com/willwng/WackyMXter-zmk-config)

## Materials
| **Item**              | **Quantity Required (per set)** |
|-----------------------|---------------------------------|
| PCBs                  |                               2 |
| [Xiao BLE](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html)              |                               2 |
| Rotary Encoder        |                               2 |
| Encoder Knob          |                               2 |
| Hotswap Sockets       |                              68 |
| Choc Switches         |                              68 |
| Power Switch          |                               2 |
| JST Battery Connector |                               2 |
| LiPo Battery          |                               2 |
| Keycaps               |                              68 |

The power switch, JST connector, and LiPo battery are optional if you want the board to be wired (but this requires powering both halves)

## Notes
- Unless you update the footprint, be sure to get EC11(E) rotary encoder <- "E" being the key. I got an EC11(R) encoder and the legs didn't fit, causing me to clip them.
- I messed up the placement of the JST connector - it stands higher than the hotswap sockets, so for a caseless build it is unfortunately too tall to be on the bottom. I ended up mounting it on the front, but backward (to not interfere with the power switch), so this required reversing the polarity of the batteries
