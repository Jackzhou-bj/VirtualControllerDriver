#Virtual Controller Driver#

Virtual Controller Driver simulates a single OpenVR controller.

## Why?

This allows you to create mixed reality videos with only two controllers.
The code also serves as a very simple example of how to create an OpenVR controller driver.

## Installation

The output file should be named driver_virtualcontroller.dll and should be in the SteamVR/drivers/virtualcontroller\bin\Win32 folder.

Example full path to dll:

    C:\Program Files (x86)\Steam\steamapps\common\SteamVR\drivers\virtualcontroller\bin\Win32\driver_virtualcontroller.dll
    
## Usage

* Start/Restart SteamVR.

After a few seconds you should see a third controller appear like so:

![capture](https://cloud.githubusercontent.com/assets/892178/15272260/c3f7dce0-1a25-11e6-835c-c46dcef514b8.PNG)

The third controller will look like a Generic HMD inside SteamVR. Because its position is hardcoded to (0, 0, 0) and cannot be changed it will appear exactly where a lighthouse is (if used with a Vive).

## How to create mixed reality videos?

Because this controller cannot currently be moved, it means that the position of your camera must be entered into the position and rotation of externalcamera.cfg.

I'm currently working on a tool that will allow you to find the position and rotation of a physical camera.
