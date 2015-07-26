##########
grbl-laser
##########

grbl is a no-compromise, high performance, low cost alternative to parallel-port-based motion control for CNC milling. It will run on a vanilla Arduino (Duemillanove/Uno) as long as it sports an Atmega 328.

This fork modifies only ``config.h`` file to suit using it with (in)famous chinese laser cutters.

`Licensing <https://github.com/grbl/grbl/wiki/Licensing>`_: Grbl is free software, released under the GPLv3 license.

Warning
-------

Mains and laser PSU are deadly, for real! Laser can make you parmanently blind.

You really should find a safer hobby.

The Arduino bootloader toggles the D13 pin when it powers up. This is the pin that enables the laser!
If you flash Grbl with a programmer (you can use a spare Arduino as "Arduino as ISP". Search the web on how to wire this.), this D13 LED toggling should go away. We haven't tested this though. Please report how it goes!

Disclaimers
-----------

Instruction provided here are incomplete and not accurate, they are shared in the hope that it will be useful,
but WITHOUT ANY WARRANTY, without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

