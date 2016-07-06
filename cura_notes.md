# Printing on the Bukobot

Relevant Links:
* [Bukobot Instructions and Docs](http://bukobot.com/Bukobot%203D%20Printer)
* [Bukobot and Blender Config](http://bukobot.com/blender-notes) and [Exporting](http://bukobot.com/blender-manifold-and-exporting)
* [Cura Documentation](https://ultimaker.com/en/products/cura-software)


## Overview

In order to print objects (referred to as `parts`) on the `Bukobot` one needs an `STL` file and a `slicing` application. Deezmaker and the MDP/Making lab recommend using [Cura](https://ultimaker.com/en/products/cura-software) to control the Bukobot and configure settings. When used in conjunction with `PronterfaceUI`, `Cura` can both issue commands to the machine (referred to as `hosting`) and divide one's file into printable layers (referred to as `slicing`).

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


## Powering the CPU and Bukobot

1. Login to the Macmini connected to the Bukobot
2. Plug the power cable for the Bukobot in. If the Bukobot's fan is spinning the machine is on.
3. Open Cura. You should see a window that looks like the photo below.

INSERT PHOTO HERE

## Configuration

1. Put your `STL` file on the computer.
2. In Cura, click the `Load` button and navigate to your file to import. The button looks like this:

INSERT PHOTO HERE

3. Now that your object is on the platform (the word Cura uses to refer to the bed) you can make alterations to it including:

 * **rotate**: rotate the orientation of the STL file on the platform via any axis (X, Y, or Z). Notice that this button also reveals "lay flat" (i.e. "force this object to rest on the platform" ), and "reset" options.
 * **scale**:

 "To max" (i.e. "scale object to maximum print size for the Bukobot"),


## misc notes

## switching views

switching views: `Expert` > `Switch to quickprint` or `Switch to full settings`

`File` > `Preferences` > `Printing Window Type` > `Pronterface UI`

Then click ` Ok`

Sometimes the nozzle gets really, really jammed!
