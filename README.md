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
3. Cut goldpin headers with pliers to correct length and install jumpers J6, J7, J8. J9
4. Instal DC connector J3
5. Install IDC connectors J1, J2, J4, J5, for correct orientation check chapter **"Old vs GEN2 expansion build"**

# Old vs GEN2 expansion build
Since pin layout have been changed durring GEN2 introduction You have to double check pin layout before connecting. In case of assempling expnasion for GEN2 consoles install idc connectors as shown below:

<img src="Images/idc_layout.png" width="800">