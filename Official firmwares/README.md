Walkthrough to:
- update your Sibilla with the newest firmware;
- upload one of the two official firmwares to expand your module with EXP-FX;

## Table of contents

- [Setup and general info](#Setup-and-general-info)
- [Update your Sibilla](#Update-your-Sibilla)
- [EXP-FX, expanding your Sibilla](#EXP-FX,-expanding-your-Sibilla)
- [Changes in power consumption](#Changes-in-power-consumption)

<br/><br/><br/>

## Setup and general info

> [!IMPORTANT]
> a micro USB type B cable is required; be sure it's a data transfer cable!

Before performing any action on your module, remember to turn off the power of your eurorack case and remove the power connector on the back of Sibilla. <br/><br/>
The fastest way to update your Sibilla is to use the [Sibilla Web programmer](https://clattersmachines.com/sibilla-programmer/): an online dedicated environment in which no firmware download nor board configuration are needed. <br/> As an alternative, you can also use the original [Daisy Web Programmer](https://electro-smith.github.io/Programmer/). <br/> <br/> 
When using the Sibilla Web Programmer, all the uploading procedures described below are also available by clicking the small questionmark button in the top right corner of the page. <br/> <br/> 

> [!NOTE]
> Do not leave the programming page/tab while waiting for the firmware to be flashed on your Daisy, the upload process will stop!

<br/> Once the firmware has been flashed, Sibilla will start to operate according to the uploaded firmware. <br/>
Please note that not all its functions will be active with the USB power line. To fully test your new uploaded code, disconnect the USB from the module and plug Sibilla back into your eurorack case.

<br/><br/><br/>

## Update your Sibilla

### Sibilla Web Programmer

Open the [Sibilla Web programmer](https://clattersmachines.com/sibilla-programmer/), connect Sibilla to your laptop and follow the steps below:

1. Hold the *`BOOT`* button down on the back of the module,  press and release the *`RESET`* and then release `BOOT`;
2. Click *`Connect`* and select *`DFU in FS mode`* on the pop-up window;
3. Select the newest firmware available from the drop down menu;
4. Click *`Program`* and wait for the progress bar to finish;

### Daisy Web Programmer

The procedure when using the Daisy Web Programmer is almost the same as described above, but with a few extra steps:
1. Download the desired [firmware](https://github.com/Clatters/Sibilla/releases);
2. Open the [Daisy Web Programmer](https://electro-smith.github.io/Programmer/);
3. Connect Sibilla to your computer via USB;
4. Hold the *`BOOT`* button down on the back of the module, and then press and release the *`RESET`* button. Release the *`BOOT`* button;
5. On the Daisy Web Programmer page, click the *`Connect`* button on the top of the page and then click and select *`DFU in FS mode`* on the pop-up window;
6. Select *`patch_sm`* in the *`"--Platform--"`* drop down menu and leave the *`"--Example--"`* section blank;
7. Click *`Choose File`* and select the downloaded .bin file;
8. Click *`Program`* and wait for the progress bar to finish;

On windows, you may have to update the driver to WinUSB. To do this, you can download the free software, Zadig. Instructions for this can be found on the [DaisyWiki](https://github.com/electro-smith/DaisyWiki/wiki) in the Windows toolchain instructions page.

You'll get the message "Programming done!" once the uploading process is finished.

<br/><br/><br/>

## EXP-FX, expanding your Sibilla

Sibilla needs to be reprogrammed in order to accept EXP-FX as an expander module: also in this case, you can either use our dedicated [Sibilla Web programmer](https://clattersmachines.com/sibilla-programmer/) or the [Daisy Web Programmer](https://electro-smith.github.io/Programmer/).

> [!IMPORTANT]
> The programming procedure is very similar to the ones described above to update Sibilla, but with the addition of a couple of steps: <strong>please carefully follow the instruction below.</strong>

Watch our video tutorial here: https://youtu.be/G4hA7FitUPQ

### Sibilla Web Programmer

Connect Sibilla to your laptop and follow the steps below:

 Hold the *`BOOT`* button down on the back of the module,  press and release the *`RESET`* and then release *`BOOT`*;
1. Click *`Connect`* and select *`DFU in FS mode`* on the pop-up window;
2. Scroll down to the bottom of the page, click *`Flash Bootloader image`* and wait for the progress bar to finish;
3. Now you need to enter the bootloader mode. To do that, press and release *`RESET`* and then press and release *`BOOT`*. A red LED on the back of your Diasy will start fading on and off;
4. Click again the *`Connect`* button and now select *`Daisy Bootloader`* on the pop-up window;
5. Select either the EXP or FX firmware from the drop down menu;
6. Click *`Program`* and wait for the progress bar to finish;

### Daisy Web Programmer

With the Daisy Web Programmer:
1. Download the desired [EXP-FX firmware](https://github.com/Clatters/EXP-FX/releases);
2. Open the [Daisy Web Programmer](https://electro-smith.github.io/Programmer/);
3. Connect Sibilla to your computer via USB;
4. Hold the *`BOOT`* button down on the back of the module, and then press and release the *`RESET`* button. Release the *`BOOT`* button;
5. On the Daisy Web Programmer page, click the *`Connect`* button on the top of the page and then click and select *`DFU in FS mode`* on the pop-up window;
6. Scroll down to the bottom of the page, click *`Advanced`* and then *`Flash Bootloader image`* and wait for the progress bar to finish;
7. Now you need to enter the bootloader mode. To do that, press and release *`RESET`* and then press and release *`BOOT`*. A red LED on the back of your Diasy will start fading on and off;
8. Click again the *`Connect`* button and now select *`Daisy Bootloader`* on the pop-up window;
9. Select *`patch_sm`* on the "--Platform--" drop down menu and leave the "--Example--" section blank;
10. Click *`Choose File`* and select the downloaded EXP-FX .bin file;
11. Click *`Program`* and wait for the progress bar to finish;

On windows, you may have to update the driver to WinUSB. To do this, you can download the free software, Zadig. Instructions for this can be found on the [DaisyWiki](https://github.com/electro-smith/DaisyWiki/wiki) in the Windows toolchain instructions page.

<br/><br/><br/>

## Changes in power consumption

Current draw specifications of Sibilla are highly dependant on the running firmwares. 
Do note that [Sibilla's power consumption data](https://github.com/Clatters/Sibilla/blob/main/README.md#current-draw) stated on the Technical specs section of its manual won't be true if a firmware different from the Sibilla_v.1.0 will be uploaded.
More info on that in the releases descriptions of both the Sibilla and EXP-FX firmwares:
- [Sibilla releases](https://github.com/Clatters/Sibilla/releases)
- [EXP-FX releases](https://github.com/Clatters/EXP-FX/releases)
