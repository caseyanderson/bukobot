# 3D Printing Overview

## Overview

In order to print objects (referred to as `parts`) on the a 3D Printer one needs an `STL` file and a `slicing` application. The MDP/Making lab recommends using [Cura](https://ultimaker.com/en/products/cura-software) to control the MAKEiT Pro-L and configure settings. When used in conjunction with `PronterfaceUI`, `Cura` can both issue commands to the machine (referred to as `hosting`) and divide one's file into printable layers (referred to as `slicing`).

After configuring `Cura` for the appropriate material type and print resolution the part must be `sliced`. 3D Printers use an additive technology called `Fused Deposition Modeling` (`FDM`) in which layers of material are laid down to create the part. Slicing cuts the part into a series of layers that are extruded onto the printer platform (frequently called the `bed`), one at a time, building the part from bottom to top.


### Parts are Usually Hollow

To save material, and print faster, the interior of a part is printed in an efficient geometric pattern (referred to as the `infill`), resulting in a predominantly hollow object.


## Printing Materials

The MAKEiT Pro-L can print with a variety of types of filaments, including composites, but we most frequently use `PLA` or `ABS`. If this is your first time using the MAKEiT Pro-L we recommend starting with `PLA`. A comprehensive list of filaments compatible with the MAKEiT Pro-L can be found [here](https://docs.google.com/document/d/1sQOWlWHHhXkFBV1JvaBUknFijHSoFLpVIfs02uuHX50/edit?usp=sharing).

### PLA vs ABS:
* `PLA` – Made from plants, is more environmentally friendly, and easier to work with than `ABS`. `PLA` is more rigid, but also more brittle than `ABS`, and does not require the printer platform to be heated.
* `ABS` – Petroleum based, higher melting point, and easier to finish (e.g. sanding, machining, etc.) after the part is printed. More pliable than `PLA`, but not as strong. Incidentally, `ABS` is the same type of plastic used in Legos.


## Creating / Acquiring a Part

3D Printers get information regarding a particular design via `STL` files. In order to print something, one must get an `STL` file via one of two possible methods:

* **Creating a Part** via some 3D Modeling application
* **Acquiring a Part** via some online repository


### Creating a Part

Recommended 3D Modeling applications:
* [TinkerCad](https://www.tinkercad.com/): free, in-the-browser, widget-based modeling application. An excellent introduction to 3D Modeling. Virtually no learning curve.
* [OpenSCAD](http://www.openscad.org/): free, scripting-oriented developer environment. Particularly good for parametric design work. An excellent intermediate modeling application. Mild learning curve.
* [Blender](https://www.blender.org/): professional, free, open-source 3D computer graphics software application for creating animated films, visual effects, art, 3D printed models, interactive 3D applications and video games. Moderate learning curve.
* [SolidWorks](http://www.solidworks.com/): $$$, professional, solid modeling computer-aided design/computer-aided engineering application that (ONLY) runs on Windows. If you fall in love with 3D modeling this is considered one of the standard tools. Moderate-to-heavy learning curve. Note that this application is on most PCs on campus at ArtCenter.


### Acquiring a Part:

Recommended sources for pre-existing model files:
* [Thingiverse](https://www.thingiverse.com/): free 3D objects made to share amongst the community.
* [Youmagine](https://www.youmagine.com/): free 3D objects made to share amongst the community.
* [Shapeways](http://www.shapeways.com/): $$$, a marketplace for objects and downloadable models.
* [3D Warehouse](https://3dwarehouse.sketchup.com/index.html): an open source library where SketchUp users can upload and download 3D models to share. Predominantly architectural and interior design models.
