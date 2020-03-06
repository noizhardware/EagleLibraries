# E A G L E   libraries    <img src="eaglelogo.jpg" alt="eagle icon" width="50"/>
## Cadsoft Eagle Libraries - mostly for audio applications

**bao.lbr** is the main library
 * now all the devices have the attribute "POPULATE" as a boolean value, so for example for a resistor it's "TRUE", for a test pad it's "FALSE". It lets you also create multiple BOMs for mounting variations of the same board.
 * also, every component is unique now, so for example, there is a package variant for each resistor value, so that is easier to track them with inventory software. Each one has a unique "NHPREF" attribute, you can change the name and value of this one as you wish for use in your inventory system. All Legacy up to _bao12.lbr_ DOESN'T use this system.

**baoPanel.lbr** is mostly intended for creating panel cutout layouts to be exported to .dxf for cnc punching/lasercut. Probably not a good idea, but worked for me so far.

**baoUtil** contains utilities for component placement like rulers, grids...

### the "Legacy" folder contains previous versions of the libraries, for backward compatibility.

---

_Up to bao09.lbr the libraries were made with Eagle 7.6.0
From that one on everything is made in Eagle 9.0.1_

---

I created most of the footprints, some of them are edited versions of footprints from other sources.

### TODO: 
 * Transfer all footprints intended for home-etching-only to a separate library, like baoHomeEtch.lbr.
   I stopped home-etching, but someone could find them useful.
   
* split library into categories? like baoCONN for connectors, baoUI for user interface components, etc..

* I'm adding schematic symbols to packages, hopefully all packages are going to be complete devices one day.
