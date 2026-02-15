# Hexapod Hardware

This repository contains the 3D-printed parts, BOM and assembly guide to replicate my hexapod robot. 

For a complete overview of the project, refer to the [main Hexapod repository](https://github.com/ggldnl/Hexapod). Additionally, you may want to check out the repositories containing the [Controller](https://github.com/ggldnl/Hexapod-Controller) and [Servo2040 firmware](https://github.com/ggldnl/Hexapod-Servo2040).

## 📋 Bill of Materials

Below is a summary of the components required to build the hexapod:

<div align="center">

| Category | Component | Quantity | Notes | Cost per part |
|----------|-----------|----------|-------|---------------|
| Mechanical Components | 3D-printed parts | | 6 x `tibia`, 6 x `femur`, ... (refer to the assembly instructions) | |
| | M3 Screw kit | 1 | Refer to the instructions to know precisely how many screws and nuts you will need. | About 12€ for an assorted 800pzs kit on Amazon |
| | F686ZZ Bearings | 18 | You will need one for the back of each motor | About 10€ for 20pzs on Amazon |
| | M3 Heat set inserts kit | 1 | Refer to the instructions to know precisely how many of them you will need. | About 10€ for 150pzs on Amazon |
| Electronics | MG996/MG996R Servo | 18 | MG996R are cheaper but less powerful than MG996, they will do nevertheless | About 70€ on Aliexpress |
| | Servo2040 | 1 | An equivalent board can be used instead e.g. 2x Pololu Mini Maestro | About 28€ on the Pimoroni website |
| | Raspberry Pi 5 | 1 | Other versions can be used instead (2/3/4) | About 100€ on Amazon |
| | Raspberry Pi camera | 1 | | About 3€ on Amazon |
| | 7.4V 2S LiPo Battery | 1 | They are often sold in pairs, so I ended up buying two of them for 50€ | About 25€ on Amazon |
| | 8A UBEC | 2 | You will need two of them, one for the servos and one for the electronics | About 20€ on Aliexpress |

</div>

Approximate total cost: around 280€.

The prices listed in this BOM reflect the costs at the time of purchase and may no longer be accurate. This BOM is provided for reference only and should not be considered a precise cost estimate.

All above components are mandatory. There are two supported assembly paths, depending on whether you choose to use a [custom PCB I designed](https://github.com/ggldnl/Hexapod-PCB) or not. Either way, you can refer to the [assembly instructions](TODO).

### Use the custom PCB

Using the custom PCB slightly increases cost (about 80€ more) but simplifies the build, keeps the body slim, acts as a rigid base plate and saves you from having to deal with manual wiring. Refer to the [Hexapod PCB repository](https://github.com/ggldnl/Hexapod-PCB) for more information.

The PCB is totally optional and you can skip it if you want to save a few bucks, but I highly recommend it.

### Don't use the custom PCB

If the PCB is not used, the electronics can still be assembled, but with additional compromises and parts.

- You will need to print the adapter plate to mount the Servo2040 and Raspberry Pi. The result will be bulkier and with wires all over the place.
- You will need to buy M2 heat-set inserts and M2 screws (Servo2040 mounting holes are 2.7 mm and do not accept M3 screws).
- You will need to sacrifice the current protection circuit on the PCB. You can use a relay to do the same job, but it doesn't fit the adapter plate.

## 🔨 Assembly Instructions

Assembly instructions are available [here](TODO).

## 🖨️ 3D Printing Profile

Print profiles and STL files for the robot parts are [hosted on MakerWorld](TODO).

Make sure to follow the recommended print settings for optimal strength and fitment.

## 📝 Notes

1. All the legs use the same basic components: `femur.stl`, `tibia.stl`, 3 x `bracket_A.stl` and 3 x `bracket_B.stl`.
2. `MG996.stl`, `battery.stl` and `electronics.stl` are used in the URDF and don't need to be printed.
3. Print the `mouting_plate.stl` only if you don't want to use the custom PCB.

## TODO

- [ ] Provide unified `electronics.stl` and `electronics_PCB.stl`
- [ ] Maybe a shield (?) to put above the electronics
- [ ] Update the assembly instructions PDF (check the TODOs in the README - there are many)
- [ ] Update the MakerWorld link with the correct URL.

## 🤝 Contribution

Feel free to raise issues or contribute improvements to this repository. For further information about the project, check out the [main Hexapod repository](https://github.com/ggldnl/Hexapod). Give a ⭐️ to this project if you liked the content.
