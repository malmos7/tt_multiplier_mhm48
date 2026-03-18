<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works
A combinational 4-bit × 4-bit unsigned multiplier. The two 4-bit operands A and B are packed into the single 8-bit input ui_in (A in the upper nibble, B in the lower nibble). The 8-bit product P is driven directly to uo_out. Inputs are registered through a two-stage reset synchronizer and only latched when ena is asserted.

## How to test
Assert rst_n low for at least two clock cycles to reset, then bring it high.
Assert ena and place A in ui_in[7:4], B in ui_in[3:0].
After one clock edge, read the 8-bit product on uo_out.


## External hardware
LED
