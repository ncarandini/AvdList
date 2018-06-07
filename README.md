# AvdList
This repository contains a list of Android Virtual Device Specification for Google emulator.

## Motivation
I'd like to have a set of Android virtual devices that represent the combination of screen sizes and resolutions that are most used by owners of real devices out there, and I thought that this could be built and shared with many other Xamarin/Android developers.

## Usage
When using the Android Device Manager of Visual Studio 2017, each device specification is stored in `C:\Users\<username>\.android\avd` folder and is made of one `<emulator_name>.ini` file and a `<emulator_name>` folder.

This repository will have a folder for each proposed _canonical device_ (a device that represent all the products with almost same screen sizes and resolution) with three things in it:
- A readme file with all the settings (and related notes) needed to replicate the virtual device from scratch with Android Device Manager
- The `<emulator_name>.ini` file 
- The `<emulator_name>` folder with only the needed files to show up in the device list of Android Device Manager

I've decided to omit `sdcard.img`, `sdcard.img.qcow2`, `system.img.qcow2` and `userdata.img` files to save more than 650MB because I've found that they're not needed to import the device specifications as they're automatically recreated by the Android Device Manager.

After cloning the repo in your PC, follow these steps to add a virtual device specification into your Android Device Manager:
1. Open the folder of the repo cantaining the `<emulator_name>.ini` file and the `<emulator_name>` folder
2. Copy the `<emulator_name>.ini` file and the `<emulator_name>` folder and paste them in `C:\Users\<your_username>\.android\avd` folder
3. Open the Android Device Manager from Visual Studio 2017 and you should see the new entry in the device list

If the definded system image is not already present in your machine, you'll se an error message in the start button. You can easily solve it with a right click on the device row, selecting the `Download System Image` command from the pulldown menu:

![image](https://user-images.githubusercontent.com/139274/41085825-5763b54e-6a38-11e8-8147-4edbaf7fe232.png)

When finished, you should be able to start the virtual device.

# Device List
Actually consist of only one device, to test portability from one PC to another:

- Samsung Galaxy Trend Lite S7390

## Contribution
New and improved virtual device can be proposed but using issues.
Issues can also be used to discuss about (as an example):
- How to find the best set of AVDs (see issue [#1](https://github.com/ncarandini/AvdList/issues/1))
- The value and functionalities of configuration parameters

# Useful links
To find the tech specs of a model I use the [GSM ARENA - Phone Finder](https://www.gsmarena.com/search.php3?)
