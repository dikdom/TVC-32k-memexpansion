# TVC 32k extender

## Magyar
Ez a repó Videoton TVC 32k bővítő modul terveit tartalmazza. A bővítőmodul arra való, hogy a 32k TVC gép memóriáját +32kB-al, 64k-ra bővítse. 64kB-os TVC gépek memóriáját nem változtatja.
Lehet rá egy LED-et is tenni, de nem muszáj.
Sőt, ha szeretsz tákolni, akkor azt is lehet, hogy ezen a kártyán legyen a TVC új reset gombja is. Sajnos a /RESET jel nincs kivezetve a felső bővítőn (illetve van, csak outputként, kívülről nem lehet a felső bővítőn resetelni a gépet), ezért bogarászni kell gép belsejét és a megfelelő helyre oda kell vinni a lap /RESET jelét. Ha ilyet szeretnél, annak neked kell utánajárnod, hogy hol van az inputnak való /RESET jel a TVC belsejében. A kapcsolási rajzok elérhetőek. 
Mi kell memóriabővítő kártyához:
- 1db 62256 SRAM
- 1db 74LS156 (vagy 74HCT156)
- 2db 100nF, 1# kondenzátor
- 1db 10k, 2# ellenállás
- OPCIONÁLIS
-- 1db 1k, 2# ellenállás, 5mm LED a visszajelzéshez
-- 1db tact kapcsoló, némi drót a külső reset gombhoz
-- foglalatok az ICkhez (DIP-28 6#, DIP-16)

## English
This repository is about a 32kB expansion module for a 32k TVC machine. This board would not change a 64k or 64k+ TVC machine.
Optionally you can attach an LED for checking if the +5V is available in the computer (the PSU when is already warmed up may not turn on again).
Optionally (#2) you can create a new reset switch to the computer, but you have to make your hands dirty in this case. The /RESET line is not exposed on the upper slot, only as an output. If you want to make the TVC reset on the tack switch then you have to route the exposed reset line from the card to the TVC 32k internal RESET line. Where is that point? You have to figure out based on the publicly available schematics of the TVC 32k machines. 
BOM:
- 1x 62256 SRAM
- 1x 74LS156 (or 74HCT156)
- 2x 100nF, 1# capacitors
- 1x 10k 2# resistor
- OPTIONALLY
-- 1x 1k 2# resistor, 5mm LED
-- 1x tact switch, some wire for the extarnal reset
-- sockets for the ICs (DIP-28 6#, DIP-16)

# License: GNU GPL v3
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)    

