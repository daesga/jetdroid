Please refer to JetKernelReleases for kernel/zImage releases and JetQiReleases for JetQi bootloader releases.

# Jet Platform release history #

| **Date** | **[JetPlatform](JetAndroid.md) version** | **Android version** | **Changes** | **Download links** |
|:---------|:-----------------------------------------|:--------------------|:------------|:-------------------|
| 2010-07-22 | 0.1                                      | 2.1 (Eclair)        | Initial release | [binary](http://jetdroid.googlecode.com/files/JetPlatform-testing-2.1-100722.tgz) [build script](http://jetdroid.googlecode.com/files/JetPlatform-build%2Bpatch-100725.tgz)|

[How to install a binary?](http://code.google.com/p/jetdroid/wiki/JetDroidBinInstall)

# Currently supported functions #
  * Booting Android 2.1
  * Basic interaction with the system

# Currently not supported functions #
Many things that are not working right now are due to missing driver support from the linux kernel. Thus these features are not related to the Android system and shall not be listed here. Please see JetKernelReleases for details.

  * ADB / USB connection (mostly kernel related)
  * Making calls / network access (GSM/3G/Wifi,...)
  * Everything else that is hardware related and not yet supported by the JetKernel

# Features planned for the next release #
  * Better keymap support (work in progress)
  * Proper screen resolution (work in progress)
  * Touchscreen calibration (work in progress)

# Features planned for future releases #
  * ADB / USB connection (mostly kernel related)
  * Use Samdroid of Cyanogen sources
  * 2D/3D acceleration (This could come with Samdroid)
  * Fancy stuff like live wallpapers