Marlin configuration for V1CNC LowRider V3 for MKS GEN L V2.1 + TMC2209 Standalone + MKS MINI 12864 V3 Display

Just replace Configuration.h in Marlin_V1CNC_Ramps_DualLR_2.0.9.2_513-src

At least in my case polarity of Z1 motor wires must be inverted (this can also be done in the firmware, but I was too lazy to figure it out).

Wiring:
| Motor | Driver | Endstop |
| ------ | ------ | ------ |
| X | X | Xmin |
| Y1 | Y | Ymin |
| Y2 | E0 | Ymax |
| Z1 | Z | Zmax |
| Z2 | E1 | Xmax |

source https://docs.v1engineering.com/electronics/dual-lr/

Steps configuration:

see line 933 comment
