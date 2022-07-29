usb_device_notification
=======================

Simple C++ library for USB device change (Insertion/removal) notification handling.
Runs in Windows and Unix environments, can be compiled using GCC or MSVC.


Prior to build on Debian, install build-dependencies:

```
 sudo apt-get install libudev-dev libusb-dev

```

Please note
=======================

This is a fork with minor improvements and fixes.
These include (not complete):
- Fix the build on current MSVC compiler.
- Add CMakeLists.txt to make this project linkable from other CMake projects.
