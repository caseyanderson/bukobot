# MAKEiT Pro-L Usage Document

## Powering the CPU and MAKEiT Pro-L

1. Login to the Macmini connected to the MAKEiT Pro-L
2. Turn the MAKEiT Pro-L on. If the fan is spinning the machine is on
3. Open Cura. You should see a window that looks like the photo below

![](/screenshots/cura_ui.png)


## Object Configuration

1. Put your `STL` file on the computer
2. In Cura, click the `File > Open File(s)` in the menu and navigate to your file to import
3. Now that your object is on the `platform` (the word Cura uses to refer to the `bed`) you can make alterations to it including:
 * `rotate`: rotates the orientation of the `STL` file on the platform (X, Y, or Z via axes). Notice that this button also reveals `lay flat` (i.e. "force this object to rest on the platform" ) and `reset` options. By default rotation changes are in increments of 15 degrees. `Shift-clicking` on the model will enable one to rotate in increments of 1 degree
 * `scale`: adjusts the size of the object. To increase its size change the scale to a number greater than 1, to decrease change scale to a number less than 1. By default `Uniform scale` is locked, however one can override it by clicking on the lock. Additionally, the `To max` button increases the object's size to the maximum print size available on the MAKEiT Pro-L
 * `mirror`: flips the model on the X, Y, or Z axes


## Machine Calibration

We recommend performing a few standard calibration procedures prior to starting each job. These procedures include checking to make sure the bed is level on the X and Y axes as well as resetting the nozzle distance (i.e. checking the Z-axis).

### Calibration Procedure

1. Press the knob down (i.e. click) to enter the `Setup` Menu.

</br>

![turn_on_calibrate_1](https://user-images.githubusercontent.com/30060990/35246684-6b911452-ff7c-11e7-92ce-c0e290685d78.gif)

</br>

2. Scroll down (turn the knob to the left) until the arrow is pointing to `Calibration`. Click to proceed
3. Scroll down until the arrow is pointing at `X-axis leveling`. Click to initiate the X-axis leveling check. The check is complete when the menu reads "Left and right are leveled" and the nozzle returns to the home position
4. Click to return to the `Calibration` menu
5. Scroll until the arrow is pointing at `Y-axis leveling`. Click to initiate the `Y-axis level check`. The check is complete when the menu reads "Left edge leveled, Right edge leveled, Click to proceed."
6. Click to return to the `Calibration` menu
7. Scroll until the arrow is pointing at `Nozzle distance`. Click to initiate nozzle distance calibration. It will take some time for the Pro-L to clean and heat the extruder nozzle (both of which are required for an accurate distance reading). When the nozzle moves to the center of the bed you are ready to move to the next step
8. Find a post-it note and slide it between the bottom of the `nozzle` and the top of the `bed`

</br>


![zspace](https://user-images.githubusercontent.com/30060990/35254981-909af694-ffa1-11e7-9840-110af3b3c87b.gif)

</br>

9. While moving the post-it note between the `nozzle` and `bed` pay attention to the amount of resistance opposing its movement. Some resistance is important but we should be able to easily move the post-it note. Use the knob on the right to change the `Offset distance`, increasing the number if the post-it note doesn't move and decreasing it if it moves without resistance
10. Click to exit `Nozzle distance` calibration. When the nozzle returns `home` you are ready to move to the next step


## Loading Filament

1. Place filament on the two rollers on the right side of the printer. The material should unroll from the bottom

</br>

![how_to_load_1](https://user-images.githubusercontent.com/30060990/35246729-93f79420-ff7c-11e7-9a75-2d0202338506.gif)

</br>

2. Click to enter the menu and navigate to `Filament`
3. Scroll until the arrow is pointing at `Filament 1`, click to proceed
4. Gently unroll enough filament to go into the hole directly in front of where the filament is currently sitting. Hold it here while you move to the next step

</br>

![load_01](https://user-images.githubusercontent.com/30060990/35246761-adcc20a0-ff7c-11e7-9b3e-0d93fb5543c8.gif)

</br>

![load_02_4](https://user-images.githubusercontent.com/30060990/35247231-7cdd3b30-ff7e-11e7-9cf6-f9f1fb880ad4.gif)

</br>

5. Scroll until the arrow is pointing at `Insert filament1` and click to proceed. You will feel the machine grab the filament, which is your cue to let go. If the extruder nozzle is not hot enough to melt the filament the machine will hold it in place until it reaches the proper temperature
6. Click to exit this part of the menu and return to the home screen


## Print Configuration

The bulk of the work around 3D Printing goes into fine-tuning print configuration settings for the job at hand. This is not a fast process and generally involves a lot of trial and error. For example, we recommend planning to use the machine for at least an hour as well as assuming that you will have to print the object multiple times to get optimal results.

In general, our recommended profile settings can be found on the Desktop of the Macmini attached to the MAKEiT Pro-L


## Running the Job

1. Click `Slice`to divide your part into layers. After the file is processed one should a time estimate for the job
2. Apply a layer of gluestick to the area surrounding the location of your object on the build plate
3. Click `Print via USB` to run the job


## Cleanup Procedure

1. Click and scroll down to `Filament`
2. Scroll to `Filament 1`, click to proceed
3. Scroll to `Remove Filament1`, click to proceed
4. After the Nozzle heats up the filament will automatically retract. If you are using the Making Lab's filament note that it **must be returned to its plastic bucket**
5. Power down the MAKEiT Pro-L
6. Log out from the Macmini
7. Remove the Build Plate and clean it with water and dish soap
8. Dry it thoroughly and then finish with rubbing alcohol


## Best Practices

* Do not expect your object to turn out perfectly the first time your print it
* Do not walk away from the MAKEiT Pro-L while a job is running
* Keep a close eye on how the material is sitting in the spool. It is easy for the material to get tangled, which can cause gaps to appear, which will ruin your object
