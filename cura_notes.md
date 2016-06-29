# Printing on the Bukobot

Relevant Links:
* [Bukobot Instructions and Docs](http://bukobot.com/Bukobot%203D%20Printer)
* [Cura Documentation](https://ultimaker.com/en/products/cura-software)


## Overview

In order to print objects (referred to as "parts") on the `Bukobot` you need an `STL` file and a `slicing` application. Deezmaker and the MDP/Making lab both recommend [Cura](https://ultimaker.com/en/products/cura-software) for slicing. When used in conjunction with `PronterfaceUI`, `Cura` can both issue commands to the machine (referred to as `hosting`) and divide one's file into small layers (referred to as `slicing`).

After configuring `Cura` for the appropriate material type and print resolution the part must be `sliced`. The Bukobot uses an additive technology called `Fused Deposition Modeling` (`FDM`) in which layers of material are laid down to create the part. Slicing cuts the part into a series of layers that are extruded onto the printer platform (frequently called the `bed`), one at a time, building the part from bottom to top.


### Parts are Usually Hollow

To save material, and print faster, the interior of a part is printed in an efficient geometric pattern (referred to as the `infill`), resulting in a predominantly hollow object.


## Printing Materials

The Bukobot can print with either `PLA` or `ABS` material. If this is your first time using the Bukobot we recommend starting with `PLA`.

### PLA vs ABS:
* `PLA` – Made from plants, is more environmentally friendly, and easier to work with than `ABS`. `PLA` is more rigid, but also more brittle than `ABS`, and does not require the printer platform to be heated.
* `ABS` – Petroleum based, higher melting point, and easier to finish (e.g. sanding, machining, etc.) after the part is printed. More pliable than `PLA`, but not as strong. Incidentally, `ABS` is the same type of plastic used in Legos.


## Creating / Acquiring a Part

3D Printers get information regarding a particular design via STL files. In order to print something, one must get an STL file via one of two possible methods:

* creating one via some 3D Modeling application
* locating one via some online repository


### Creating a Part

Recommended 3D Modeling applications:
* [TinkerCad](https://www.tinkercad.com/): free, in-the-browser, widget-based modeling application. An excellent introduction to 3D Modeling. Virtually no learning curve.
* [OpenSCAD](http://www.openscad.org/): free, scripting-oriented developer environment. Particularly good for parametric design work. An excellent intermediate modeling application. Mild learning curve.
* [Blender](https://www.blender.org/): professional free, open-source 3D computer graphics software application for creating animated films, visual effects, art, 3D printed models, interactive 3D applications and video games. Moderate learning curve.
* [SolidWorks](http://www.solidworks.com/): $$$, solid modeling computer-aided design/computer-aided engineering computer program that runs on Microsoft Windows (only). If you fall in love with 3D modeling this is considered one of the standard platforms. Moderate-to-heavy learning curve.


## misc notes

## switching views

switching views: `Expert` > `Switch to quickprint` or `Switch to full settings`

`File` > `Preferences` > `Printing Window Type` > `Pronterface UI`

Then click ` Ok`

Sometimes the nozzle gets really, really jammed!
