# CMM2 Expansion System
<img src="Images/exp_board_3d.jpg" width="400">
Expansion system for CMM2 was created to add easy to use expansion system for CMM2

Schematic can be found here: [schematic REV A v02](/Schematic/exp_syst_REVA_v02.pdf)

# WARNING!
<img src="Images/champf.jpg" width="200">
Expansion card used with this system have to have edges champfered, using unchampfered card will result in slot dammage

# Assembly
1. Install protection diode D1. This diode prevent reversed polarity on 12V supply. Instead of diode You can also close jumper JP1, please remember that You will about risk of revers polarity on 12V line, reversed polarity will dammage expnasion system, expansion cards and Maximite unit.
2. If needed install smoothing capacitators (not included in kit) C1, C2, C3
3. Cut goldpin headers with pliers to correct length and install J6, J7, J8. J9
4. Instal DC connector J3
5. Install IDC connectors J1, J2, J4, J5, for correct orientation check chapter **"Old vs GEN2 expansion build"**
6. Install edge connector slots, be carefull to allign 8 and 60 pin slot in each row
7. Install jumpers accordingly to chapter **"Power supply selector and power supply daisy chain"**

# Old vs GEN2 expansion build
Since IDC40 pin layout have been changed durring GEN2 introduction You have to double check pin layout before connecting. In case of assempling expnasion for GEN2 consoles install idc connectors as shown below:

<img src="Images/idc_layout.png" width="800">

# Power supply selector and power supply daisy chain
<img src="Images/pow_jump.png" width="800">
J6, J7, J8. J9 are used to decide if varrious power lines shoud be daisy chained between expansions or Maximite and expansions

| Jumper | Desc. | Remarks |
| --- | --- | --- |
| J6, J7 | 12V | 12V line from external 12 power supply connected to Maximite Deluxe or Expansion |
| J6, J7 | 5V, 3V3 | high efficient 5V and 3,3V from power expansion card |
| J6, J7 | p3, p4 | additional power lines currently not used |
| J8, J9 | 5V, 3V3 | 5V and 3,3V line from Maximite power line |

## Example ##
Lets assume following setup: Maximite Deluxe GEN2 >>> 1st Expansion >>> 2nd Expansion
and jumpers on 2st Expansion set as below:
<img src="Images/pow_jump_exam.png" width="800">
12V power from Maximite 12v power supply will be connected to first and 2nd expansion. 5V and 3,3V from internal power supply of Maximite will be connected to first expansion but will not to 2nd. 2nd Expansion will receive 3.3V, 5V power cards on 1st expansion.

# How to make expansion card #
<img src="Images/card_footp.jpg" width="400">
<img src="Images/card_symb.jpg" width="400">
Everything needed to start creating Your own expansion cards can be found

[here](../Kicad/exp_card/)

