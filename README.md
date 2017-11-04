# B171A-Slicing-Assignment

Vaším dnešním úkolem bude naslicovat několik modelů v aplikaci Slic3r.
Abyste ale nezačínali s prázdnou máme pro vás jako dárek config bundle,
který si importujte do Slic3ru. Ve Slic3ru používáme Expert mód.
File -> Preferences -> Mode.

  * [config_bundle](slic3r_config_bundle.ini)
  
Tiskárnu mějte nastavenou RebeliX a filament ABS Esun 1.75mm z config bundelu.
Po jednotlivých vygenerováních gcodu prozkoumejte výstup jednotlivých nastavení
v panelu Preview (dole ve Slic3ru).


První z modelů je [bulbasaur.stl](bulbasaur.stl)
  (CC BY-NC-SA 3.0 [FLOWALISTIK](https://www.thingiverse.com/thing:327753)) s parametry

  * 5 perimetrů vertikálního shellu, 4 plné dolní vrstvy a 3 dolní
  * Rychlost tisku perimetrů je 45 mm/s
  * Raft o 3 vrstvách
  * Infill typu Honeycomb s hustotou 15%
  * Teplota Bedu je při první vrstvě 79°C

Druhý je držák na tužky Darth Vadera -[vader_cup_v03.stl](vader_cup_v03.stl)
  (CC BY-NC 3.0 [tmasantos](https://www.thingiverse.com/thing:1396307))
  * Výška jedné vrstvy je 35mm z toho první vrstva je 36mm
  * Rychlost tisku infillu je 50mm/s, perimetry tiskneme s rychlostí 40mm/s
  * Chceme nechat vygenerovat support
  * Perimetry nám stačí jen dva
  * Infill stačí 10% a pattern necháme "Line"
  * Minimum Loops u skirt změníme na 3
  * Teplota extruderu na první vrstvu je 228 a na ostatní 323

Na závěr něco praktického a to otvírák na pivo -[bottle_opener](bottle_opener.stl) 
  (CC BY-SA 3.0 [leemes](https://www.thingiverse.com/thing:132632))
  * 30% infill se vzorem 3D Honeycombu
  * 3mm brim + 2 vrstvy raftu
  * Infill se tiskne s rychlostí 40mm/s
  * Zpomalte tisk, pokud je rychlost výtisku jedné vrstvy vytisklý
  za méně než 15 s
  * Větráček bude permanentně zaplý s minimální rychlostí 10%
  * Retrakce o 2mm osy Z, když se přechází na další vrstvu

Do repozitáře vytvořeného na odkazu ODKAZ
dejte soubory `bulbasaur.gcode`, `vader_cup_v03.gcode`, `bottle_opener.gcode`.
Doporučujeme si jednotlivé configurace Slic3eru ukládat.

