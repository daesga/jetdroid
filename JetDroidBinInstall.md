**Note: do NOT only go by the pictures, you will miss important steps!**

# Contents #




> # What you need: #
    * Computer set up as described in [JetDroidBuildEnvironment](JetDroidBuildEnvironment.md)(for this tutorial you need to run Ubuntu(Linux) only)
    * S8000 Jét with a succesfully flashed JetQi-Bootloader
    * binary release from JetPlatformReleases
    * SDHC-card, which you don't currently need
    * zImage of a working Kernel
> > Optional:
      * JetDroid-Keyboard-layout-patch(under Downloads)
# How to do it: #
    1. **format your SDHC-card to the ext3-file format**
  * **This erases all Data on your SDHC-card!!**
  * **RUN UBUNTU**(Linux)
  * Make sure your SDHC-card is inserted into your Jét and connect the Jét to your Computer in **Mass Storage** mode.
  * Close the 2 upcoming windows.
  * Start **System>Administration>Disk Utility**

![http://www.pictureupload.de/originals/pictures/020810143032_Binaryinstall1.png](http://www.pictureupload.de/originals/pictures/020810143032_Binaryinstall1.png)

  * Choose **Samsung TFLASH**(**NOT** MFLASH, MFLASH is the internal memory of your Phone)
  * Click **Unmount Volume** (For all possible partitions)
  * Click **"Format Drive"**, Choose **"Master Boot Record"**; Click format.

> ![http://www.pictureupload.de/originals/pictures/010810163831_Binaryinstall2.png](http://www.pictureupload.de/originals/pictures/010810163831_Binaryinstall2.png)

  * Click **create Partition** > Choose **ext3** ,give your Partition a name(in my case "JetDroid")and Check "Take ownership of the Device". (I set size to **1GB**, has to be < 2GB)


  * ![http://www.pictureupload.de/originals/pictures/010810163913_Binaryinstall3.png](http://www.pictureupload.de/originals/pictures/010810163913_Binaryinstall3.png)

  * Click **create** and confirm.
  * Click on the remaining 3GB(or more), **create Partition** and make them FAT in the same fashion(I called the partition "Data")
  * When it is done, click **Mount Volume** to remount the SDHC-card.(Do it for **both** Partitions)

> Your SDHC-card is now formatted in the right file-format and all Data on it has been  deleted.

> 2. **Copy the necessary files on your SDHC-card**
  * Open up the folder of the **JetDroid-Partition**
  * **Copy all files** from JetPlatform archive to the partition.


  * ![http://www.pictureupload.de/originals/pictures/310710140539_Binaryinstall4.png](http://www.pictureupload.de/originals/pictures/310710140539_Binaryinstall4.png)



  * Now Copy the contents of "JetKernel-0.2.binary.tgz" onto your JetDroid-partition(don't forget to copy the folder called "boot" and its content) (http://code.google.com/p/jetdroid/downloads/detail?name=JetKernel-0.2.binary.tgz)
  * Now replace the "qwerty.kl" in "JetDroid/system/usr/keylayout/" with the one from "JetDroid\_Keyboard\_layout.zip"
The Filesystem should now look like this:


(Picture was misleading, updated picture coming soon)


  * Last: right click on the JetDroid-Partition, click properties and set the access rights **all** to "create and delete files".Check "run file as program", and click to copy the access rights to all contained files.



**You should now be able to boot JetDroid,
Have Fun**

-JetDroid Development Team

# Not Working? - Bugfixing #
# Bootloader messages like: "Unable to mount ext2 file system"
  * possible reason: you did not choose "Master Boot Record", but "GUID partition table"
  * possible solution: delete all partitions and reformat the device using "Master Boot Record"(MBR)

**OR**

  * possible reason: The ext3-partition cannot be accessed by the bootloader.
  * solution: Set the access rights for the partition as described above!

# Kernel message with: "...Permission denied." at the end.
  * reason: improper access rights.
  * solution: set access rights as described above.

# Bootloop (Desktop doesn't show up, instead you keep seeing the animated "android" logo)
  * reason: broken binary
  * solution: download and try a different version.