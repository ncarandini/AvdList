# AvdList
This repository contains a list of Android Virtual Device Specification for Google emulator.

## Motivation
I'd like to have a set of Android virtual devices that represent the combination of screen sizes and resolutions that are most used by owners of real devices out there, and I thought that this could be built and shared with many other Xamarin/Android developers.

## Usage
When using the Android Device Manager of Visual Studio 2017, each device specification is stored in `C:\Users\<user_name>\.android\avd` folder and is made of one `<emulator_name>.ini` file and a `<emulator_name>` folder.

This repository will have a folder for each proposed _canonical device_ (a device that represent all the products with almost same screen sizes and resolution) with three things in it:
- A readme file with all the settings needed to replicate the virtual device from scratch with Android Device Manager
- The `<emulator_name>.ini` file 
- The `<emulator_name>` folder

Let's see if we can do something useful of it.
