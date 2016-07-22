# ticalc
General repository of ti calculator programs. Likely to mostly be in z80 assembly.

includes/ti83plus.inc is provided here: http://wikiti.brandonw.net/index.php?title=83Plus:OS:ti83plus.inc

These projects are likely to primarily be assembled with the SPASM assembler, which can be found here: https://wabbit.codeplex.com/

## Current programs

- src/flame.z80 Produces a flame demo effect on the calculator screen. CLEAR will quit the program, and the UP and DOWN keys should increase, and decrease the contrast, resepectively. This relies on port 30h in models TI-83 Plus Silver Edition, TI-84 Plus, and TI-84 Plus Silver Edition to access hardware timers.

	This project can be assembled from the root of this repository with in Linux: spasm -I includes src/flame.z80 flame.8xp

	OR in windows

	spasm -I includes src\flame.z80 flame.8xp
