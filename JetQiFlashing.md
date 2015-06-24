## Flashing the JetQi bootloader to a phone ##

### BE CAUTIOUS! THIS PROCEDURE COULD TURN YOUR PHONE INTO A BRICK ###
Any fault at this point will turn your phone into a _brick_.

It is spoke that a phone with simlock breaks itself without fail.
So only normal phones can be flashed.

It is important to say that flashing with a **bad** bootloader _**cannot be rollbacked**_. Any mistake with it will turn your phone into a _**brick**_! As flashing via USB is a feature of the bootloader a broken bootloader will not have this feature. Also the phone after it may _**lose**_ an ability to load current OS. So the phone will _**not work**_!

The JetDroid project is not functional right now. Thus it advised to flash the bootloader only if you are a developer and you **know what you are doing**. Regular users _**should not use it**_ now! As the project is not fuctional right now you have more chances to break your phone than to have anything useful.

### CONTINUE AT YOUR OWN RISK! WE DON'T TAKE ANY RESPONSIBILITY FOR DAMAGES ###

### Dependencies ###
This section has non-free dependencies: current firmware with original os from the phone, multiloader tool, samsung's new pc studio, and ms windows. All tools used here will only work on windows, not on linux. You can also find instructions on flashing e.g. in the DarkForst Group (DFG) forum ([link](http://darkforestgroup.com/forum/index.php?topic=752.0), [link2](http://darkforestgroup.com/samsung-flash-guide)).

It is not very convenient to restart your computer, running linux for building, to windows for flashing. Thus it is possible to use a virtual machine for one of the tasks. For example you can build the bootloader on your linux and flash it to the phone from windows running in virtualbox with a connected usb device (for this you should run virtualbox as root or set correct rights on usb devices). The other way around is also an option (building the bootloader inside a virtual linux machine and flashing in the windowas host system).

### Preparation ###
  1. Start windows
  1. Install the Samsung New PC Studio (NPS) and all drivers that come with it
  1. Download multiloader tool of version above 5.54
  1. Find and download your firmware files
  1. Restart the computer
  1. Disable the NPS tray icon and make sure NPS is not started automatically when connecting the phone

### Flashing ###
**THIS IS THE DANGEROUS PART! CONTINUE AT YOUR OWN RISK! WE DON'T TAKE ANY RESPONSIBILITY FOR DAMAGES**
  1. Start multiloader
http://lh4.ggpht.com/_loD3PaNk5OI/S-KXgcNUjEI/AAAAAAAAACE/lpzGO9tNUk0/s512/MultiLoader.annotated.PNG
  1. Select "LSI6410" radiobutton (1)
  1. Select "Boot Change" checkbox (2)
  1. Click on "Boot" button and select the directory containing the bootloader files you prepared before (3)
  1. Connect your phone in "download mode" to computer. You may see NPS icon with arrows (if you did not disable it before) in system tray but NPS should not start. Make sure you will see port detected by multiloader as shown in the picture (4)
  1. If you know what you are doing and you are sure you want to take the risk, click on the "Download" button (5). You will see running line where port selected, all should be ok in the seconds.
  1. If you see "security fail" then try to detach and attach the phone again
  1. If it fails again then try to workaround on this or try another tutorial

### Activating JetDroid Mode ###
If flashing to your phone was successful the phone should restart and begin booting the Samsung system. The JetDroid mode will only be activated if you hold down either the call button (left to the cube/menu button) or the lock button (top right of you phone) while powering up the phone.
After activating the JetDroid mode as described above, you should see messages on your display that look like in the picture below.

http://lh4.ggpht.com/_loD3PaNk5OI/S-RCTIWHsGI/AAAAAAAAACg/3WvCSYcnkkM/s512/IMG_7353s.JPG
