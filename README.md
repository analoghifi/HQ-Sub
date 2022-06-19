# HQ-Sub  
adjustable 5th order (30 dB/oct.) subsonic filter  
  
https://web.archive.org/web/20160324051200/http://thel-audioworld.de/module/Filterzone/HQ-Sub.htm

----
### A note on the capacitors used in the original design  
The basic problem is:  
to get meaningful (= not too high) resistance values in this 5th order filter design we want to use 1µF capacitors.  
However, 1µF capacitors are generally not available in the KP film/foil version,  
at least not with a 1% tolerance and/or in suitable small dimensions for this small PCB.  
  
regarding C8-C17 in the original design:  
the 1µF MKS capacitors are paralleled with 22nF KP capacitors  
to compensate the very bad (=very high) dissipation factor (tanδ) of the MKS capacitors  
originally equipped with:  
WIMA MKS4    1µF/63V 10% (metallized Polyester)    tanδ=8x10  
WIMA FKP2 0,022µF/63V 5%  (film/foil Polypropylene) tanδ=5x10  
aonther problem is:  
You have to do a lot of component selection work (matching) when using 10% capacitors because:  
Even while it is not so important that the 5 filter capacitors have exactly 1.00 µF,  
they should at least all have the same value (±1%) among each other  
in this 5th order filter arrangement.  
  
#### better alternative (better tolerance & better tanδ):  
use good MKP 1% capacitors (with no additional parallel capacitors = omit C9,C11,C13,C15 and C17)  
for example:  
Vishay MKP1839 [MKP1839510161] 1µF/160V 1% axial (metallized Polypropylene) tanδ=4x10   
my KiCad PCB (<a href="/hardware/KiCad">/hardware/KiCad</a>) is prepared for using this big axial capacitors (10.5mm x 26.5mm) in upright position.  
