# TGPKernel S7 (for Android Oreo 8)

![TGPKernel Logo](https://github.com/TheGalaxyProject/tgpkernel-s7-o/blob/master/build/logo.png?raw=true)

A Custom Kernel for Samsung Galaxy S7 / S7 Edge.

* XDA S7 Forum: http://forum.xda-developers.com/showthread.php?t=3462897
* XDA S7 Edge Forum: http://forum.xda-developers.com/showthread.php?t=3501571


Compiled using Google GCC 4.9 Toolchain

* URL: https://android.googlesource.com/platform/prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.9

## How to use
Adjust the toolchain path in build.sh and Makefile to match the path on your system. 

Run build.sh with the following options, doesn't matter what order keep and silent are in.

For example: build.sh 930 -s

- **./build.sh** will build TGPKernel
- **./build.sh -k** will build TGPKernel and also copy the .img files to the .output folder
- **./build.sh -s** will build TGPKernel but only display warning and errors in the log
- **./build.sh -ks** will do both **-k** and **-s** at the same time
- **./build.sh 930** will only build the S7 Kernel
- **./build.sh 935** will only build the S7 Edge Kernel

When finished, the new files and logs will be created in the .output directory.

If Java is installed, the .zip file will be signed.


These commands can only be executed by themselves

- **./build.sh 0** will clear the workspace
- **./build.sh 00** will clear CCACHE
- **./build.sh configs** will regenerate the stock hero(2)lte configs and overwrite the old ones


## Credit and Thanks to the following:
- [Samsung Open Source Release Center](http://opensource.samsung.com) for the Source code (my personal repo [here](https://github.com/djb77/samsung-kernel))
- [Google](https://android.googlesource.com/kernel/common) for AOSP Common Kernel Source
- @osm0sis for [Android Image Kitchen](https://github.com/osm0sis/Android-Image-Kitchen/tree/AIK-Linux) and [anykernel2](https://github.com/osm0sis/AnyKernel2)
- @Tkkg1994, @morogoku, @Noxxxious, @farovitus, and @mwilky for help and commits

