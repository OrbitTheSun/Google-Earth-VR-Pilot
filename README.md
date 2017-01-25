# Google-Earth-VR-Pilot
**_FreePIE_ Script for _Google Earth VR_ with _Oculus Rift_**  
Lets you pilot the virtual *HTC Vive* controllers within *Google Earth VR* with your *Xbox* controller.

Currently, *Google Earth VR* can only be used with the *HTC Vive* headset in full functionality.
Operation is by using the *HTC Vive* controllers to move around in virtual reality. In order to use
*Google Earth VR* with the *Oculus Rift*, a software solution can be used that emulates the controllers
of the *HTC Vive*. The software setup uses *FreePIE* to control the *SteamVR Driver for Razer Hydra*.
This driver in turn emulates the *HTC Vive* controllers for use in *Google Earth VR*.

# Downloads

Download ***FreePIE*** from: http://andersmalmgren.github.io/FreePIE/

Download ***"SteamVR Driver for Razer™ Hydra"*** on *Steam* from: http://store.steampowered.com/app/491380/

# Installation

*FreePIE* and the *SteamVR* driver must be installed first.

Then two files have to be replaced:

- In the FreePIE program directory, find the files ***sixense_fake.dll*** and ***sixense_fake_x64.dll***.

- Find the directories ***Win32*** and ***Win64*** under the following path:

    ***"C:\Program Files (x86)\Steam\steamapps\common\SteamVR Driver for Razer Hydra\hydra\bin\"***

- Copy ***sixense_fake.dll*** to the ***Win32*** subdirectory.

- Copy ***sixense_fake_x64.dll*** to the ***Win64*** subdirectory.

- **Delete or rename** the original ***sixense.dll*** in the ***Win32*** directory.
Then rename the file ***sixense_fake.dll*** to ***sixense.dll***.

- **Delete or rename** the original ***sixense_x64.dll*** in the ***Win64*** directory.
Then rename the file ***sixense_fake_x64.dll*** to ***sixense_x64.dll***.

# Operation

To use *Google Earth VR* with the emulated *Hydra* controllers, you must start *FreePIE* first.
Load the attached script ***gevr_xbox_vive_emulation.py*** in *FreePIE* and start it with **F5**.

After that start *Google Earth VR* (via *Steam*). After a short time, you will be prompted to press any
key on the controllers. Then **press both triggers** of the *Xbox* controller.

Then hold **LB** and **RB** and press **START** button. Initialization of the control is now complete.

### How the _HTC Vive_ controls work

The left *Vive* controller can be used like a flashlight pointer to grab and move the virtual world by pulling
the trigger. Other buttons allow you to open and scroll the menu, fly and rotate the world.

The right *Vive* controller holds a mini-globe to display the current world position, which is also displayed with text.  
The buttons on this controller can be used to scroll through the menu or to save the current view as a snapshot.

Watch the tutorial (see menu) to get an introduction to the operation of the buttons.

### Operation using the _Xbox_ controller

Interacting with the virtual world is mainly done with the left *Vive* controller.
Therefore, the *Xbox* controls primarily affect this controller.

To affect the **right** *Vive* controller, the **RB** key must be pressed and **held**.

- You can change the **orientation** of a *Vive* controller by using the **Left Stick** of the *Xbox* controller.
**Pitch** and **yaw** of the controller are changed.
- The **position** of a *Vive* controller can be changed with the **Right Stick**, the **D-Pad** or the
**Left Stick** while the **LB** button is pressed:  
  - The **D-Pad** moves a *Vive* controller **horizontally** along its axes.  
  - A **stick** moves a controller **vertically** or makes it **circle** around the origin.  
  - A **thumb press** returns a controller to its **starting point**.  
    Press the **left** or the **right thumb** for the respective controller.
    
#### Button assignment and function

*Xbox* controller button | *HTC Vive* controller button | Function
--- | --- | ---
**Left Trigger** | Left Trigger | *Grab* earth or sky <br> *Click menu* <br> *Slow down* flight
**Right Trigger** | Right Trigger | *No function*
Face button **B** | bbb | *Fly forward* <br> *Scroll forward* in menu
Face button **A** | aaa | *Fly backwards* <br> *Scroll backwards* in menu
Face button **Y** | yyy | *Open* or *close* menu
Face button **X** | xxx | **Hold** to *rotate landscape* with the **Left Stick**


