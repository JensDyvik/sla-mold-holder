# SLA mold holder
*A system for supporting SLA 3D printed injection molds with milled aluminum shells. By Jens Dyvik, for Folkeverkstedet, Deichman public library, Oslo, Norway, June 2024*

![](/img/the-two-halves.JPG)

### Files for making SLA 3D printed molds

- [Mold blank - STL mesh](https://github.com/JensDyvik/sla-mold-holder/blob/main/stl-files/sla-mold-holder-mold-blank.stl)
- [Mold blank - Step solid](https://github.com/JensDyvik/sla-mold-holder/blob/main/step-files/sla-mold-holder-mold-blank.step)

### Why

SLA 3D printers can make fast and detailed molds for injection molding small series of plastic parts. But the high pressure of injection molding can crack the brittle SLA molds. We have made a simple design for CNC milled two aluminium halves that suppoert the molds during injection to keep them from cracking. These mold holders allows you to use less plastic when 3D printing your molds and inject with higher pressure.

[Folkervekstedet](https://deichman.no/vi-tilbyr/folkeverkstedet_1e2de21d-0716-40b3-a605-43b17ee48b6e) at Deichman has equipment from [Plasticpreneur](https://plasticpreneur.com/) of the Precious Plastic project for recycling plastic and making new parts. They commisioned Jens Dyvik to design these mold holders so that staff and users of the makerspace can use their Formlabs SLA 3D printer to makes modls, and much easier get started meking their own design with the avaiable equipment or plastic recycling.

### How

Download the mold lanks in [STL mesh](https://github.com/JensDyvik/sla-mold-holder/blob/main/stl-files/sla-mold-holder-mold-blank.stl) or [Step solid](https://github.com/JensDyvik/sla-mold-holder/blob/main/step-files/sla-mold-holder-mold-blank.step) format. Import the mold blank into your CAD program and position your design in the mold blank and make a mirror of the mold blank along the XY plane. Make boolean subtractions of the mold blanks minus your design. This should leave a hollow cavity in the mold blanks. You also need to add a "sprue" by subtraction a cylindrical shape where the plastic flows into the mold. Be mindful of "draft angles" and that you need to be able to get the design out of the mold when it has cooled down after injection. Export the two mold halves to your 3D printer program *(PreForm or other)* and print with your SLA 3D printer. Be mindful of resin choice. "Tough" or "High temperature" can make good options, but standard resin can work surprinsgly well too.

OMce you have cured and reomved supports fom your mold, place the in the alumnium mold holders and close up with the four finger nuts and carriage bolts

### Tests

![](/img/test-mold.jpg)
**

### The making

![](/img/)
**

![](/img/)
**

![](/img/)
**

![](/img/)
**

![](/img/)
**

![](/img/)
**

![](/img/)
**

![](/img/)
**

![](/img/)
**

![](/img/)
**

![](/img/)
**

![](/img/)
**

### Source file

- [FreeCAD design file](https://github.com/JensDyvik/sla-mold-holder/blob/main/freecad-source-files/sla-mold-holder.FCStd)
- [Download link for FreeCAD, free and open source and runs on Linux, Windows and MacOS](https://www.freecad.org/)

### BOM

- 2 pcs: aluminium blanks 40mm x 70mm x 127mm or larger
- 4 pcs: M8 carraige bolt 80mm
- 4 pcs: M8 wing nuts
- SLA 3D printed molds

#### Further reading

- https://formlabs.com/eu/applications/injection-molding/
