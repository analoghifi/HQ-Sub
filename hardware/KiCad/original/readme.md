this is not the original Thel PCB but it's very like\* the original with the following exceptions:  
* more massive ground and power supply PCB tracks  
* using the 2mm gold-plated (lathe made) brass solder pins (the same ones used on the more expensive Thel modules)
* swapped positions for C1<->C5 and C2<->C6
* using a special footprint for the 1µF MKS foil caps (C8,C10,C12,C14,C16), so that you can use bigger (better) MKP axial caps in upright position (in this case: omit C9,C11,C13,C15 and C17)
  
\*(same schematic / same board dimensions / same 1-layer\** layout THT / same THT components in the same places on the board)  
\**(strictly speaking, this KiCad PCB is a two-layer PCB with plated-through holes, but you can also (let) produce it as a classic 1-layer PCB with non-plated holes if you wish, since all the tracks are on the bottom side only)  
    
----  
  
### remarks:  
#### U1:  
instead of MC33078 you can use OPA1602,  
with slightly better technical data regarding noise an THD.
  
----  
  
these are KiCad 6.x projects  
see how to get the proper 3D-Models from here: https://github.com/analoghifi/KiCad-3D-Models


  
----  
  
use kicanvas.org to view this KiCad project in your browser:  
https://kicanvas.org/?github=https%3A%2F%2Fgithub.com%2Fanaloghifi%2FHQ-Sub%2Ftree%2Fmain%2Fhardware%2FKiCad%2Foriginal  
