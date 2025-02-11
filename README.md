# Hexapod Hardware

This repository contains the 3D-printed parts, BOM and assembly guide to replicate my hexapod robot. 

For a complete overview of the project, refer to the [main Hexapod repository](https://github.com/ggldnl/Hexapod). Additionally, you may want to check out the repositories containing the [Controller](https://github.com/ggldnl/Hexapod-Controller) and [Operator](https://github.com/ggldnl/Hexapod-Operator) code.

## 📋 Bill of Materials (BOM)

Below is a summary of the components required to build the hexapod:

| **Category**           | **Component**                           | **Quantity** | **Notes**                                                                                       | **Cost per part**                                 |
|------------------------|-----------------------------------------|--------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------|
| Mechanical Components  | 3D-printed parts                        |              |                                                                                                 |                                                   |
|                        | M2 Screw kit                            | 1            | You just need 4 M2x6 screws for the Raspberry pi and 4 M2x6 for the Servo2040, each with a nut. | Less than 8€ for an assorted 225pzs kit on Amazon |
|                        | M3 Screw kit                            | 1            | Refer to the instructions to know precisely how many screws and nuts you will need.             | About 12€ for an assorted 800pzs kit on Amazon    |
|                        | F686ZZ Bearings                         | 18           | You will need one for the back of each motor                                                    | About 10€ for 20pzs on Amazon                     |
|                        | M3 Heat set inserts kit                 | 1            | Refer to the instructions to know precisely how many of them you will need.                     | About 10€ for 150pzs on Amazon                    |
| Electronics            | Servos MG996R                           | 18           | MG996R are cheaper than MG996, you can buy these instead if you can                             | About 70€ on Aliexpress                           | 
|                        | Servo2040                               | 1            | An equivalent board can be used instead e.g. 2x Pololu Mini Maestro                             | About 28€ on Pimoroni                             |
|                        | Single channel relay module             | 1            |                                                                                                 | Usually cost around 1.5€ each                     |
|                        | Raspberry pi 5                          | 1            | Other versions can be used instead (2/3/4)                                                      | About 100€ on Amazon                              |
|                        | Raspberry pi camera                     | 1            | I had a v1.3 already                                                                            | About 3€ on Amazon                                |
|                        | 7.4V 2S LiPo Battery                    | 1            | They are often sold in pairs, so I ended up buying two of them for 50€                          | About 25€ on Amazon                               |

Approximate total cost: 270€

The prices listed in this BOM reflect the costs at the time of purchase and may no longer be accurate. This BOM is provided for reference only and should not be considered a precise cost estimate.

## 🔨 Assembly Instructions

Assembly instructions are available [here]().

## 3D Printing Profile

Print profiles and STL files for the robot parts are [hosted on MakerWorld](https://makerworld.com/en/models/).

Make sure to follow the recommended print settings for optimal strength and fitment.

## 📝 Notes

1. The `MG996.stl` is used in the URDF, we won't need it to build the actual robot. Check out the [simulation repository](https://github.com/ggldnl/Hexapod-Simulation).

2. I just found this [amazing web-based urdf visualizer](https://gkjohnson.github.io/urdf-loaders/javascript/example/bundle/). You can just drag and drop a urdf file and the `CAD` folder and it will display the robot. This was quite handy during development.  

## TODO

- [ ] Update the assembly instructions PDF.
- [ ] Update the MakerWorld link with the correct URL.

## Contribution

Feel free to raise issues or contribute improvements to this repository. For further information about the project, check out the [main Hexapod repository](https://github.com/ggldnl/Hexapod). Give a ⭐️ to this project if you liked the content.
