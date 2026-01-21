# Hexapod Hardware

This repository contains the 3D-printed parts, BOM and assembly guide to replicate my hexapod robot. 

For a complete overview of the project, refer to the [main Hexapod repository](https://github.com/ggldnl/Hexapod). Additionally, you may want to check out the repositories containing the [Controller](https://github.com/ggldnl/Hexapod-Controller) and [Operator](https://github.com/ggldnl/Hexapod-Operator) code.

## 📋 Bill of Materials

Below is a summary of the components required to build the hexapod:

| **Category**           | **Component**                           | **Quantity** | **Notes**                                                                                       | **Cost per part**                                 |
|------------------------|-----------------------------------------|--------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------|
| Mechanical Components  | 3D-printed parts                        |              |                                                                                                 |                                                   |
|                        | M3 Screw kit                            | 1            | Refer to the instructions to know precisely how many screws and nuts you will need.             | About 12€ for an assorted 800pzs kit on Amazon    |
|                        | F686ZZ Bearings                         | 18           | You will need one for the back of each motor                                                    | About 10€ for 20pzs on Amazon                     |
|                        | M3 Heat set inserts kit                 | 1            | Refer to the instructions to know precisely how many of them you will need.                     | About 10€ for 150pzs on Amazon                    |
| Electronics            | MG996/MG996R Servo                           | 18           | MG996R are cheaper but less powerfull than MG996, they will do nevertheless                             | About 70€ on Aliexpress                           | 
|                        | Servo2040                               | 1            | An equivalent board can be used instead e.g. 2x Pololu Mini Maestro                             | About 28€ on the Pimoroni website                             |
|                        | Raspberry pi 5                          | 1            | Other versions can be used instead (2/3/4)                                                      | About 100€ on Amazon                              |
|                        | Raspberry pi camera                     | 1            |                                                                             | About 3€ on Amazon                                |
|                        | 7.4V 2S LiPo Battery                    | 1            | They are often sold in pairs, so I ended up buying two of them for 50€                          | About 25€ on Amazon                               |
|                        | 8A UBEC                    | 2            | You will need two of them, one for the servos and one for the electronics                          | About 20€ on Aliexpress                               |
|                        | Custom PCB                    | 1            | Alternatively, you can wire up the electronics following the instructions. Check out the [PCB section](#PCB) | About 20€ on JLCPCB                               |

Approximate total cost: around 300€

The prices listed in this BOM reflect the costs at the time of purchase and may no longer be accurate. This BOM is provided for reference only and should not be considered a precise cost estimate.

## 🔌 PCB

The PCB is totally optional and you can skip it if you want to save a few bucks, but I highly recommend it: it acts as a rigid base plate, keeps the body slim and avoids having to deal with manual wiring. Refer to the [Hexapod PCB repository](https://github.com/ggldnl/Hexapod-PCB) for more information. If you don't want to use the PCB, you can follow the [manual wiring instructions](TODO). In this case you will have to replace the SMD components on the PCB with a stand-alone relay module. You can find them on amazon for around 1.5€ each.

## 🔨 Assembly Instructions

Assembly instructions are available [here](TODO).

## 🖨️ 3D Printing Profile

Print profiles and STL files for the robot parts are [hosted on MakerWorld](TODO).

Make sure to follow the recommended print settings for optimal strength and fitment.

## 📝 Notes

1. The `MG996.stl` is used in the URDF, we won't need it to build the actual robot so you don't have to print it. Check out the [simulation repository](https://github.com/ggldnl/Hexapod-Simulation).

## TODO

- [ ] Update the assembly instructions PDF.
- [ ] Update the MakerWorld link with the correct URL.

## Contribution

Feel free to raise issues or contribute improvements to this repository. For further information about the project, check out the [main Hexapod repository](https://github.com/ggldnl/Hexapod). Give a ⭐️ to this project if you liked the content.
