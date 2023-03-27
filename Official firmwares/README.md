
# Update your Sibilla

Sibilla update walkthrough.

## Setup and programming

Follow the steps below to upload a new firmware to your Sibilla: </br>
- Turn off the power of your eurorack case;
- Remove the power connector on the back of Sibilla;
- Download the desired firmware;
- Open the [Daisy Web Programmer](https://electro-smith.github.io/Programmer/);
- Connect Sibilla to your computer via USB;
- Hold the BOOT button down on the back of the module, and then press and release the RESET button. Sibilla's center white LED should now be on;
- On the Daisy Web Programmer page, click the Connect button on the top of the page and then click "DFU in FS mode";
- Select "patch_sm" as desired platform;
- Click "Choose File" and select the downloades .bin file;
- Click "Program" and wait for the progress bar to finish;

You'll get the message "Programming done!" once the uploading process is finished. Sibilla will now start to operate accordingly to the uploaded firmware. Please note that not all its functions will be active with the USB power line.
To fully test your new uploaded code, disconnect the USB from the module and plug it back into your eurorack case.
