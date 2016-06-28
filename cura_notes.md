# Printing on the Bukobot

Relevant Links:
* [Bukobot Instructions and Docs](http://bukobot.com/Bukobot%203D%20Printer)
* [Cura Documentation](https://ultimaker.com/en/products/cura-software)


## Overview

In order to print objects (referred to as "parts") on the `Bukobot` you need an `STL` file and a `slicing` application. Deezmaker and the MDP/Making lab both recommend [Cura](https://ultimaker.com/en/products/cura-software), which, when combined with `PronterfaceUI`, can both issue commands to the machine (referred to as "hosting") and divide one's file into small layers (referred to as "slicing").

After configuring `Cura` for the material type and printing resolution the part must be `sliced`. The Bukobot uses an additive technology called `Fused Deposition Modeling` (`FDM`) in which layers of material are laid down to create the part. Slicing cuts the part into a series of layers that are extruded onto the printer platform (frequently called the `bed`), one at a time, building the part from bottom to top.


### Parts are Usually Hollow

To save material, and print faster, the interior of a part is printed in an efficient geometric pattern (frequently honeycomb-shaped), resulting in a predominantly hollow object.

## Printing Materials

The Bukobot can print with either `PLA` or `ABS` material. If this is your first time using the Bukobot we recommend starting with `PLA`.

`PLA` vs `ABS`:
* `PLA` – Made from plants, is more environmentally friendly, and easier to work with than `ABS`. `PLA` is more rigid, but also more brittle than `ABS`, and does not require the printer platform to be heated.
* `ABS` – Petroleum based, higher melting point, and easier to work with (e.g. sanding, machining, etc.) after the part is printed. More pliable than `PLA`, but not as strong. Incidentally this is the same type of plastic found in Legos



## misc notes

## switching views

switching views: `Expert` > `Switch to quickprint` or `Switch to full settings`

`File` > `Preferences` > `Printing Window Type` > `Pronterface UI`

Then click ` Ok`

Sometimes the nozzle gets really, really jammed!
