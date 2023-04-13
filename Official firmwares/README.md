
# Update your Sibilla

Sibilla update walkthrough.

## Setup and programming

Follow the steps below to upload a new firmware to your Sibilla: </br>
- Turn off the power of your eurorack case;
- Remove the power connector on the back of Sibilla;
- Download the desired firmware;
- Open the [Daisy Web Programmer](https://electro-smith.github.io/Programmer/);
- Connect Sibilla to your computer via USB;
- Hold the BOOT button down on the back of the module, and then press and release the RESET button. Release the BOOT button and Sibilla's center white LED will be on;
- On the Daisy Web Programmer page, click the Connect button on the top of the page and then click and select "DFU in FS mode" on the pop-up window;
- Select "patch_sm" on the "--Platform--" drop down menu and leave the "--Example--" section blank;
- Click "Choose File" and select the downloaded .bin file;
- Click "Program" and wait for the progress bar to finish;

On windows, you may have to update the driver to WinUSB. To do this, you can download the free software, Zadig. Instructions for this can be found on the [DaisyWiki](https://github.com/electro-smith/DaisyWiki/wiki) in the Windows toolchain instructions page.

You'll get the message "Programming done!" once the uploading process is finished. Sibilla will now start to operate according to the uploaded firmware. Please note that not all its functions will be active with the USB power line.
To fully test your new uploaded code, disconnect the USB from the module and plug Sibilla back into your eurorack case.

### Change in power consumption

Current draw specifications of Sibilla are highly dependant on the running firmwares. 
Do note that [Sibilla's power consumption data](https://github.com/Clatters/Sibilla/blob/main/README.md#current-draw) stated on the Technical specs section of its manual won't be true if a firmware different from the Sibilla_v.1.0 will be uploaded.
