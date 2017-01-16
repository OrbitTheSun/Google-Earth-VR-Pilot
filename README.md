# Google-Earth-VR-Pilot
FreePIE Script for Google Earth VR with Oculus Rift.
Lets you pilot the virtual HTC Vive controllers within Google Earth VR with your Xbox controller.

Currently, Google Earth VR can only be used with the HTC Vive headset in full functionality. Operation is by using the HTC Vive Controllers to move around in virtual reality. In order to use Google Earth VR with the Oculus Rift, a software solution can be used that emulates the controllers of the HTC Vive. The software setup uses FreePIE to control the SteamVR Driver for Razer Hydra. This driver in turn emulates the HTC Vive controllers for use in Google Earth VR.

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

- **Delete or rename** the original ***sixense.dll*** in the ***Win32*** directory. Then rename the file ***sixense_fake.dll*** to ***sixense.dll***.

- **Delete or rename** the original ***sixense_x64.dll*** in the ***Win64*** directory. Then rename the file ***sixense_fake_x64.dll*** to ***sixense_x64.dll***.

# Operation

To use *Google Earth VR* with the emulated *Hydra* controllers, you must start *FreePIE* first. Load the attached script ***' 	gevr_xbox_vive_emulation.py'** in *FreePIE* and start it with **F5**.

Then *Google Earth VR* can be started (via *Steam*). After a short time, you will be prompted to press any key on the controllers. Then **press both triggers** of the *Xbox* controller.
