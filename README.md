# Nova-FRAM-32kw-full-board
Schematics and PCB for a 32 kw FRAM board, Nova 800/1200 series. EasyEDA project, Gerber production files, and PDF schematic. Use ideally 1.4 mm board thickness. 1.2 mm will also probably work (does for me), while 1.6 mm is probably too thick. Produce with ENIG, and gold fingers.

Jumper settings:

For 32 kw operation, do not install any jumpers on H1 nor H2.

For 16 kw operation, do not install any jumper on H2. On H1, install the A1# (A1=0) jumper for mapping to the 0-16 kw range, or the A1 (A1=1) jumper for the 16-32 kw range.

For 8 kw operation, install jumpers on both H1 and H2. Select the combination of A1 and A2 for the desired 8 kw block within the 32 kw address space. E.g. inserting the jumpers A1 (A1=1) and A2# (A2=0) will select the 16-24 kw range.

Parts:

U1-U4:   74LS155 (4x)

U5-U12:  74LS38  (8x)

U13-U20: 74LS74  (8x)

U21-U22: 74LS373 (2x)

U23:     74LS122

U24:     74LS04

U25+U37: 74LS08  (2x)

U26+U31+U33+U34+U36: 74LS00 (5x)

U27:     74LS10

U28:     74LS11

U29+U30: FM1808B-SG (2x)

U32+U35: 74LS244

C1:      10 pF

C2-C11:  100 pF (10x)

C12-C24: 47 nF (13x)

C25-C32: 10 uF (8x)

R1-R7, R9-R10: 10 kOhm (9x)

R8:    470 Ohm

2x3-pin headers for jumpers
