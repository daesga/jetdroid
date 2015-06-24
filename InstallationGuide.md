
---

# Contents #



# Introduction #
This a preliminary attempt to provide a detailed and start-to-finish guide to installing JetDroid in it’s current state. If anything is missing or changes, please let me know in the comments or on the DFG!

NOTE: A more up to date version is available here: [here](http://www.jetdroid.org/forum/viewtopic.php?f=11&t=18)

# Before you start #

Make sure you have the following:

  1. Unlocked (Sim and Network) Samsung Jet S8000. Refer to [Flash Guide](http://darkforestgroup.com/archives/51) For additional requirements and instructions.
  1. A 4GB and up SD **HC** micro SD card. Must be HC at the time of writing.
  1. Samsung New PC Studio or Kies (Clarification about Kies is welcomed!) for Jet’s drivers
  1. Bootloader JetQi. You can build this using the JetDroidBuildEnvironment page. Or find it here: http://jetdroid.org/forum/viewtopic.php?f=11&t=18&p=24#p24
  1. A good understanding of the flashing procedure, file operations in windows and Ubuntu (the latter is easy to learn) and partitioning.
  1. Make sure your Jet’s firmware matches one here: [Bootloader Versions](http://code.google.com/p/jetdroid/wiki/BootloaderVersions) If not, then consider flashing to a compatible version.
  1. Download Ubuntu, Virtualbox and Paragon Drive Backup (Or use GParted):
  * Here: http://www.ubuntu.com/desktop/get-ubuntu/download
  * Here: http://www.virtualbox.org/wiki/Downloads
  * And here: http://www.paragon-software.com/home/db-professional/download.html
In a single easy to reach folder in windows

Here is an example:

![http://a.imageshack.us/img838/5116/foldertw.jpg](http://a.imageshack.us/img838/5116/foldertw.jpg)


---


# Prepare the Jet #

In order for your phone to be able to start Android, we need to modify the way it starts up, to give us the option of choosing Android instead of TouchWiz.

  * **BACKUP ALL CONTENT ON PHONE AND SDCARD TO WINDOWS**. Calendar, Memo etc can be backed up using New PC Studio.
  * Locate the bootloader build and open it in Multiloader (which you learned about here:  [in the flash guide](http://darkforestgroup.com/archives/51) )

Make sure it matches this picture:

![http://a.imageshack.us/img682/9091/boota.jpg](http://a.imageshack.us/img682/9091/boota.jpg)

## Flashing JetQi ##

More detailed steps: (BUT NO SUBSTITUTE FOR READING THE [Flash Guide](http://darkforestgroup.com/forum/index.php?topic=752.0) )
  1. Use this radio button
  1. click only boot change
  1. Click ‘Boot’ button and navigate to folder containing the JetQi mbn
  1. Connect Jet in Download Mode (Turn off, then Vol down, camera and power) and then connect via usb. Click Port Search.
  1. Should say ‘Ready’ here
  1. Click Download, and cross fingers (arbitrary)
  1. Should say ‘all files ok’ or similar here.
  1. Disconnect the phone after it restarts.

You now have JetQi in place.


---


# Prepare Ubuntu Linux #

  * Install VirtualBox

  * Set up a new Virtual Machine, like so:

Start by clicking ‘New’. Then follow the prompts like so:

<img><img src='http://a.imageshack.us/img840/5695/machine.png' /></img>

After setting up the virtual machine:

  1. Click ‘Start’ green arrow.
  1. Follow the instructions to complete Ubuntu Setup. Make sure you specify the **ubuntu .iso** you downloaded at the start as the boot device.
  1. When this has finished, shut down ubuntu and return to virtualbox.
  1. Connect Jet to computer in USB Mass Storage mode and go to ‘settings’ then ‘USB’ in virtualbox.
  1. Click the ‘+’ icon and choose SAMSUNG GT-S8000 or similar to add Jet as a USB device.
  1. Boot up Ubuntu with the Jet still attached and verify the card appears.
  1. Shutdown Ubuntu


---


# Prepare the MicroSDHC card #

In order to use JetDroid, you will need to split your memory card into two 'areas' or partitions. This is because Android needs an ext3 filesystem in order to operate. This is just a different type to FAT32 or NTFS.

The first partition will be usable in the Samsung TouchWiz OS for storing media as normal, but the second one will only be visible in Ubuntu, which is why we use it and not Windows in certain places.

## Using GParted ##

  * Start GParted. This can be found in the Ubuntu Software Centre. You may need to enter your Ubuntu password.
  * On the top right of GParted, click /dev/sda and change to the one that is roughly the size of your SDHC card, and **NOT the 1GB - 2GB of your Jet!**
  * Here you will see the list of partitions on your card. If you just bought yours or have never partitioned it before it should look something like this!
![http://a.imageshack.us/img836/6526/fat32.png](http://a.imageshack.us/img836/6526/fat32.png)
  * Right click the main FAT32 partition (if new) and any extra ones you have (if previiously partitioned) (except unallocated ones) and click 'delete'.
  * You should now have the rough size of your card represented as grey and 'unallocated'
![http://a.imageshack.us/img841/6219/unall.jpg](http://a.imageshack.us/img841/6219/unall.jpg)
  * Right click this unallocated entry and click 'new'.
  * This will be the FIRST partition so change the 'New size' box to the total size minus about 1.5GB.
    * Change the 'file system' entry to 'FAT32'
    * Choose a label for your FAT32 partition. As this will be usable for media etc in the TouchWiz OS, name it MEMORY CARD or MEDIA etc
![http://a.imageshack.us/img843/1439/fat32first.jpg](http://a.imageshack.us/img843/1439/fat32first.jpg)
  * Click 'Add'
  * Now for the JetDroid ext3 partition. Right click the unallocated section and click 'new'
  * This time just change 'file system' to 'ext3' and choose a label. I chose 'NEW VOLUME'. Its not important.
  * Click 'Add'
  * Make sure FAT32 is #1 and the ext3 is #2
  * Click the tick at the top. YOU WILL LOSE ALL DATA ON THE SDCARD AT THIS POINT.
![http://a.imageshack.us/img841/1104/exampletable.jpg](http://a.imageshack.us/img841/1104/exampletable.jpg)
  * Wait for completion.
![http://a.imageshack.us/img251/63/completion.jpg](http://a.imageshack.us/img251/63/completion.jpg)
  * Close Gparted

## Or use Paragon Drive Backup ##

  1. In windows, install Paragon Drive Backup that you downloaded earlier.
  1. Connect Jet in Mass Storage Mode with the SD card inserted if not already. Make sure Ubuntu is NOT running.
  1. Under the Disk Map area, right click the FAT32 section of the Memory Card, and click delete partition.  **YOU WILL LOSE ALL DATA ON THE CARD AT THIS POINT.**
  1. Right click the empty space that appears in its place and click create partition. Make this one the majority of the space of the card, and set it to FAT32. Leave up to 1.7GB unaccounted for after this partition as this will be used for ext3.
  1. After this is done, right click the space you left over after the FAT32 partition, then click create partition again. Make this one ‘ext3’ and finish.
  1. Make sure you close all other programs apart from Paragon Drive Backup and then click ‘Apply’. **Your computer may restart to finish this procedure.**
  1. Your card should now be formatted correctly for JetDroid.


---


# Install Android files #

## Download files ##

  * Start Virtualbox, then Ubuntu
  * Connect Jet in Mass Storage Mode when Ubuntu has booted up.
  * Get latest **platform files (binary release)** , **zImage**, and **qwerty.kl** [here](http://code.google.com/p/jetdroid/downloads/list)
  * Put those three items in one easy to find folder IN UBUNTU. Here is an example: ![http://a.imageshack.us/img816/6394/platform.jpg](http://a.imageshack.us/img816/6394/platform.jpg)
  * Extract the contents of these, placing the platform files in ‘Platform’ and the zImage and qwerty.kl in the folder you already have them in. JetDroid 0.2, for me for example.
  * Open a terminal, and type `sudo nautilus`. An explorer type window will open. Example: (Yes, my name is Chris... too many places to cover up) <img><img src='http://a.imageshack.us/img682/5332/nautilus.jpg' /></img>

## Placing the files ##

  * Navigate using this window to your downloaded jetdroid files and then copy the contents of the ‘Platform’ folder onto the root folder of the ext3 partition.
Example: (KFAT1 is Jet internal, MEMORY CARD is FAT32 card partition, so you can see my ext3 partition is called NEW VOLUME) ![http://a.imageshack.us/img715/5516/platformext3.jpg](http://a.imageshack.us/img715/5516/platformext3.jpg)
  * Copy the zImage into this same root folder
  * Copy the qwerty.kl into ‘system’ -> ‘usr’ -> ‘keylayout’ and replace the existing one.
  * Close that window and the terminal behind it when this is done.

## Setting permissions ##

In order for Android to be able to use the files it needs, it needs permissions to use them. Here's how it is done:

  * Open a new terminal.
  * Type `sudo chmod -R 777` but **don't hit enter yet**
  * Go to your root ext3 partition folder (mine is NEW VOLUME) and click copy in the ‘address area’ Example:
![http://a.imageshack.us/img714/8813/copyname.jpg](http://a.imageshack.us/img714/8813/copyname.jpg)
  * Go back to the terminal you didn’t press enter on and go to ‘edit’ -> ‘paste filenames’
> > Now press enter. Enter Ubuntu password if prompted. May be a brief pause.
  * When the prompt returns, you can close the terminal and safetly remove the Jet from the ubuntu desktop. Example:
![http://a.imageshack.us/img801/6513/safea.jpg](http://a.imageshack.us/img801/6513/safea.jpg)


---


# Testing JetDroid #


  1. Switch off the handset.
  1. Hold call and end buttons simultaneously.
  1. Wait for JetDroid Desktop!


Good luck!


---


If anything is wrong or missing here, please let me know!

Also, any common problems may have been already discussed in this forum, so please read around. I will add some troubleshooting here if need be!