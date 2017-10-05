# Printing on the MAKEiT Pro-L

Relevant Links:
* [User Manual](http://makeit-3d.com/manuals/safe-operation/)
* [Cura Documentation](https://ultimaker.com/en/products/cura-software)


## Overview

In order to print objects (referred to as `parts`) on the `MAKEiT Pro-L` one needs an `STL` file and a `slicing` application. The MDP/Making lab recommends using [Cura](https://ultimaker.com/en/products/cura-software) to control the MAKEiT Pro-L and configure settings. When used in conjunction with `PronterfaceUI`, `Cura` can both issue commands to the machine (referred to as `hosting`) and divide one's file into printable layers (referred to as `slicing`).

After configuring `Cura` for the appropriate material type and print resolution the part must be `sliced`. The MAKEiT Pro-L uses an additive technology called `Fused Deposition Modeling` (`FDM`) in which layers of material are laid down to create the part. Slicing cuts the part into a series of layers that are extruded onto the printer platform (frequently called the `bed`), one at a time, building the part from bottom to top.


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


## Powering the CPU and MAKEiT Pro-L

1. Login to the Macmini connected to the MAKEiT Pro-L
2. Turn the MAKEiT Pro-L on. If the MAKEiT Pro-L's fan is spinning the machine is on.
3. Open Cura. You should see a window that looks like the photo below.

![](/screenshots/cura_ui.png)


## Object Configuration

1. Put your `STL` file on the computer.
2. In Cura, click the `Load` button and navigate to your file to import. The button looks like this: ![](/screenshots/load_file.png)
3. Now that your object is on the `platform` (the word Cura uses to refer to the `bed`) you can make alterations to it including:
 * `rotate`: rotates the orientation of the `STL` file on the platform (X, Y, or Z via axes). Notice that this button also reveals `lay flat` (i.e. "force this object to rest on the platform" ) and `reset` options. By default rotation changes are in increments of 15 degrees. `Shift-clicking` on the model will enable one to rotate in increments of 1 degree.
 * `scale`: adjusts the size of the object. To increase its size change the scale to a number greater than 1, to decrease change scale to a number less than 1. By default `Uniform scale` is locked, however one can override it by clicking on the lock. Additionally, the `To max` button increases the object's size to the maximum print size available on the MAKEiT Pro-L.
 * `mirror`: flips the model on the X, Y, or Z axes.


## Machine Calibration

The MDP/Making lab recommends performing a few standard calibration procedures prior to starting each job. These procedures include checking to make sure the bed is level on the X and Y axes as well as resetting the nozzle distance (i.e. checking the Z-axis).

### Calibration Procedure

1. Press the knob down (i.e. click) to enter the `Setup` Menu.
2. Scroll down (turn the knob to the left) until the arrow is pointing to `Calibration`. Click to enter this section of the Menu.
3. Scroll down until the arrow is pointing at `X-axis leveling`. Click to initiate the X-axis leveling check. The check is complete when the menu reads "Left and right are leveled" and the nozzle returns to the home position.
4. Click once more to return to the `Calibration` menu.
5. Scroll until the arrow is pointing at `Y-axis leveling`. Click to initiate the `Y-axis level check`. The check is complete when the menu reads "Left edge leveled, Right edge leveled, Click to proceed."
6. Click to return to the `Calibration` menu.
7. Scroll until the arrow is pointing at `Nozzle distance`. Click to initiate nozzle distance calibration. It will take some time for the Pro-L to clean and heat the extruder nozzle (both of which are required for an accurate distance reading). When the nozzle moves to the center of the bed you are ready to move to the next step.
8. Find a post-it note and slide it between the bottom of the `nozzle` and the top of the `bed`.
9. While moving the post-it note between the `nozzle` and `bed` pay attention to the amount of resistance opposing its movement. Some resistance is important but we should be able to easily move the post-it note. Use the knob on the right to change the `Offset distance`, increasing the number if the post-it note doesn't move and decreasing it if it moves without resistance. An offset of 1.35 seems to be a good distance.
10. Press the knob down to exit `Nozzle distance` calibration. When the nozzle returns `home` you are ready to move to the next step.


## Loading Filament

1. Place filament on the two rollers on the right side of the printer. The material should unroll from the bottom for optimal results.
2. Click the knob to enter the menu and navigate to `Filament`.
3. Scroll until the arrow is pointing at `Filament 1` and then click.
4. Gently unroll enough filament to go into the hole directly in front of where the filament is currently sitting. Hold it here while you move on to the next step.
5. Scroll until the arrow is pointing at `Insert filament1` and click. You will feel the machine grab the filament, which is your cue to let go of it. If the extruder nozzle is not hot enough to melt the filament yet the machine will hold it in place until it reaches the proper temperature.
6. Click the knob to exit this part of the menu and return to the home screen.


## Print Configuration

The bulk of the work around 3D Printing goes into fine-tuning print configuration settings for the job at hand. This is not a fast process and generally involves a lot of trial and error. For example, we recommend planning to use the machine for at least an hour as well as assuming that you will have to print the object multiple times to get optimal results.

In general, our recommended profile settings can be found on the Desktop of the Macmini attached to the MAKEiT Pro-L. Simply navigate to the profile that is write for your job and load it into Cura by navigating to `File > Open Profile` and then selecting the desired profile. Start with these settings for job attempt number 1 and augment to suit your needs as necessary for successive jobs.


## Cleanup Procedure

1. Click the knob and scroll down to `Filament`.
2. Scroll to `Filament 1`, click to proceed.
3. Scroll to `Remove filament1`, click to proceed.
4. After the Nozzle reaches 210 degrees the filament will automatically retract. If you are using the Making Lab's filament note that it **must be returned to its plastic bucket**.
5. Power down the MAKEiT Pro-L.
6. Log out from the Macmini.


## Best Practices

* Do not expect your object to turn out perfectly the first time your print it
* Do not walk away from the MAKEiT Pro-L while a job is running
* Keep a close eye on how the material is sitting in the spool. It is easy for the material to get tangled, which can cause gaps to appear, which will ruin your object
