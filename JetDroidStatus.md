# Preface #
The project is not done. No one can predict when or if this will ever happen. Please don't ask for a release date.

Even though we have a fuctional Bootloader and a good Kernel, the project will take still quite a while until Android is fully usable! We would be extremely lucky, if functions like calling and messaging would work without further modding.

# Hardware analysis #
Some usefull information on the Jét hardware has been gathered on the JetHardware page.

# Bootloader #
A new bootloader is the first step in getting Android to work on the Jét.

Currently the bootloader development aims at patching the original bootloader to keep the ability to download new versions via USB and only boot into the JetDroid mode if the right keys are pressed at power up.(DONE)

This concept has been successfully tested. A first alternate bootloader with the ability to load a linux kernel has successfully been flashed.

The Bootloader currently only boots from SDHC-cards(usually 4Gb and up) not from SD-cards! We are working to resolve that issue.

See JetBootloader for more details on the bootloader.

# Kernel port #
The linux kernel has been successfully ported to the Samsung S3C6410 processor several times. Android phones using this architecture include Samsung SPH-M900 and GT-I5700. Compiling and modifying the the kernel is the next step after getting the bootloader up and running.

A modified kernel source for the Jét, based on the SPH-M900 kernel source is availabe. Please see JetKernel for more details.

# Andoid System #
Attempts to compile the Samsung GT-I5700 Android 2.1 (Eclair) source files have led to a first Android system that shows the Android logo.
The Desktop has been reached and the Touchscreen is working now.
We are currently working to get the Sound to work.

Premature System files and a pre-built Kernel are available under "Downloads".
Use at own risk!

Possibly some more detailed information is available on the [Contributing](Contributing.md) page.