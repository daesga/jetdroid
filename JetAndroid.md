# Introduction #

With the latest kernel adjustments it was possible to boot an Android system on the Jet. Many (essential) things (e.g. touchscreen) are still not working but good progress has been made so far.

On this page you can find some useful stuff about running and the Android system on the Jet.

# Keypad #

We can now use a modified keymap to control the Android system. Here are the instructions how to implement this. Modify the file /system/usr/keylayout/qwerty.kl to look like below.

```

key 9	  CALL		WAKE_DROPPED  
key 249   ENDCALL	WAKE_DROPPED
key 2     CAMERA 	WAKE_DROPPED #not working
key 3     CAMERA	WAKE_DROPPED #not working
key 1     MENU		WAKE_DROPPED
key 17    BACK		WAKE_DROPPED
key 11    VOLUME_UP	WAKE	
key 10	  VOLUME_DOWN	WAKE
key 19    HOME          WAKE #not working

```
Now you can use the phone keys to control the Android system. The picture below shows the key mapping.

[
![http://www.pictureupload.de/originals/pictures/050810142018_JetDroid_Keymap.jpg](http://www.pictureupload.de/originals/pictures/050810142018_JetDroid_Keymap.jpg)
]

The keymap and the instructions are also available on the [download page](http://code.google.com/p/jetdroid/downloads/list).