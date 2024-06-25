# SLA mold holder
*A system for supporting SLA 3D printed injection molds with milled aluminum shells. By Jens Dyvik, for Folkeverkstedet, Deichman public library, Oslo, Norway, June 2024*

![](/img/the-two-halves.JPG)

### Files for making SLA 3D printed molds

- [Mold blank - STL mesh](https://github.com/JensDyvik/sla-mold-holder/blob/main/stl-files/sla-mold-holder-mold-blank.stl)
- [Mold blank - Step solid](https://github.com/JensDyvik/sla-mold-holder/blob/main/step-files/sla-mold-holder-mold-blank.step)

### Why

SLA 3D printers can make fast and detailed molds for injection molding small series of plastic parts. But the high pressure of injection molding can crack the brittle SLA molds. We have made a simple design for CNC milled two aluminum halves that support the molds during injection to keep them from cracking. These mold holders allows you to use less plastic when 3D printing your molds and inject with higher pressure.

[Folkervekstedet](https://deichman.no/vi-tilbyr/folkeverkstedet_1e2de21d-0716-40b3-a605-43b17ee48b6e) at Deichman has equipment from [Plasticpreneur](https://plasticpreneur.com/) inspired by the [Precious Plastic](https://www.preciousplastic.com/) project for recycling plastic and making new parts. They commissioned Jens Dyvik to design these mold holders so that staff and users of the makerspace can use their Formlabs SLA 3D printer to makes molds, and thereby much easier get started making their own designs with the available equipment or plastic recycling.

We hope that this will inspire more awareness and technical knowhow around plastics recycling in Oslo. And hopefully the 3D printed molds will help recycle more grams of plastic than what is used to resin print the molds.

### How

Download the mold blanks in [STL mesh](https://github.com/JensDyvik/sla-mold-holder/blob/main/stl-files/sla-mold-holder-mold-blank.stl) or [Step solid](https://github.com/JensDyvik/sla-mold-holder/blob/main/step-files/sla-mold-holder-mold-blank.step) format. Import the mold blank into your CAD program and position your design in the mold blank and make a mirror of the mold blank along the XY plane. Make boolean subtractions of the mold blanks minus your design. This should leave a hollow cavity in the mold blanks. You also need to add a "sprue" by subtraction a cylindrical shape where the plastic flows into the mold. Be mindful of "draft angles" and that you need to be able to get the design out of the mold when it has cooled down after injection. Export the two mold halves to your 3D printer program *(PreForm or other)* and print with your SLA 3D printer. Be mindful of resin choice. "Tough" or "High temperature" can make good options, but standard resin can work surprisingly well too.

Once you have cured and removed supports from your mold, place the in the aluminum mold holders and close up with the four finger nuts and carriage bolts. If the fit is too loose you can fill up the gaps with tape or paper. If the fit is too tight you can sand down the molds with sand paper. You can also adjust the tolerance parameters in FreeCAD and 3D print again *(image bellow)* Happy injection molding!

![](/img/freecad-design-with-parameters.JPG)
*The parameters in FreeCAD*

### Pro tips

- Be mindful of shrinkage. Massive volumes of injection molded plastic tends to shrink unevenly when cooling down.
- Be mindful of air gaps. It can be nice to add small channel for air to escape from the molds.
- Be mindful of reducing material use of the molds themselves with shelling and ribs. Example FreeCAD and stl files are in this repo.

![](/img/spinning-top-and-test-mold.JPG)
*And example mold for a spinning top*

![](/img/material-use-optimization-example.JPG)
*The underside of the example mold, optimized for using less resin material thanks to shelling and ribs*

### Tests

![](/img/test-mold.jpg)

*The printed spinning top test mold and test injection. We made the tolerances for the files for the printed molds tighter to reduce the gaps after this test*

### The making

![](/img/adpative-clearing-toolpaths-in-freecad.JPG)
*Adaptive clearing toolpath for CNC milling, made with FreeCAD*

![](/img/milling-top.JPG)
*3 axis milling of the topside done*

![](/img/milling-bottom.JPG)
*3 axis milling of the bottom side done*

![](/img/closed-with-carriage-bolts-and-wing-nuts.jpg)
*The tow mold holders locked together*

![](/img/printing-with-preform.JPG)
*First test print of a test mold in PreForm*


### Source file

- [FreeCAD design file](https://github.com/JensDyvik/sla-mold-holder/blob/main/freecad-source-files/sla-mold-holder.FCStd)
- [Download link for FreeCAD, free and open source and runs on Linux, Windows and MacOS](https://www.freecad.org/)

### BOM

- 2 pcs: aluminium blanks 40mm x 70mm x 127mm or larger
- 4 pcs: M8 carraige bolt 80mm
- 4 pcs: M8 wing nuts
- SLA 3D printed molds

### Toughts

- The system seems to work well
- Milling the tow mold holders is a lot of work *(30+ different toolpaths, four different milling bits and two sided setup)*
- Sourcing the aluminum blanks from 70mm x 40mm extrusion took some time
- Getting the right tolerance for the resin printed mold sides and bottoms is tricky
- A project like this is at risk of having a negative overall impact on the environment despite its sustainability goal *(lots of aluminum used and lots resin used for printing molds that might not see a lot of use)*
- I hope that the educational and inspirational impact at the Folkeverkstedet makerspace will be large

#### Further reading

- https://formlabs.com/eu/applications/injection-molding/
