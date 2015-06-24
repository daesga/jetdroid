# Introduction #
Several options exist to get Android running on the Jet. Below some information on the bootloader options are listed.

# Jetdroid bootloader #
  * Functionality of the original bootloader should be used to keep USB download mode
  * To keep the rest simple a small bootloader like [Qi](http://wiki.openmoko.org/wiki/Qi) should be started if the right keys are pressed at power-up. Subseqently the second step bootloader should read the kernel from SD-card.

# Samsung bootloader #

Memory map for original Samsung flash memory

| Start adress | File / Section | Comment |
|:-------------|:---------------|:--------|
| 0x00000000   | boot\_loader.mbn | S3C6410 bootloader |
| 0x00100000   | dbl.mbn        | baseband bootloader |
| 0x00200000   | Amss           |         |
| 0x01100000   | Apps           |         |
| 0x03600000   | Rsrc1          |         |
| 0x08500000   | Rsrc2          |         |
| 0x08700000   | Factory FS     |  - 0x0B000000 |

Files of original Samsung firmware (S8000XWIF6)
  * Boot
    * bootloader.mbn (291.400 / 0x47248 Bytes)
    * dbl.mbn (155.205 / 0x25E45 Bytes)
  * Amss
    * amss.bin (13.744.956 / 0xD1BB3C Bytes)
  * Apps
    * apps\_compressed.bin (35.128.320 / 0x2180400 Bytes)
  * Rsrc1
    * Rsrc\_S8000\_Open\_Europe\_Common.rc1 (79.179.101 / 0x4B82D5D Bytes)
  * Rsrc2
    * Rsrc2\_S8000(Low).rc2 (1.693.292 / 0x19D66C Bytes)
  * Factory FS
    * FactoryFs\_S8000\_Open\_Europe\_Common\_OXA.ffs (42.991.616 0x2900000 Bytes)

Dram initialization sequence of the original bootloader is described in OriginalDramInit.

Samsung firmware service codes
  * `*#1234#` --> Display Firmware revision
  * `*#0*#` --> Test Mode
  * `*#06#` --> Display IMEI
  * `*#1111#` --> Software version
  * `*#2222#` --> Hardware version
  * `*2767*3855#` --> FullReset (DELETES ALL DATA)
  * `*#4777*8665#` --> GPRS-Tool
  * `*#6984125*#` --> Admin settings
  * `*#9072641*#` --> Master key (until IG1)
  * `*#7092463*#` --> Master key (from IG1)
  * `*#6984125*#` --> Internals (until IG1)
  * `*#6984125*#` --> Internals (from IG1)
  * `*#73561*#` --> PreConfig menu (until IG1)
  * `*#73561*#` --> PreConfig menu (from IG1)
  * `*#73561*#` --> Lock status
  * `*#197328640#` --> Service menu (from IG1)
  * `*#232337#` --> Bluetooth
  * `*#0228#` --> Battery info
  * `*#0206*8376263#` --> SW|Revision|HW-Version, RF calibration & D/L date

Samsung boot modes

This section was tested with s8000xeig2 firmware version and may be inapplicable to other versions.

All sets of keys to press have been bruteforced. And it have been found two special types
of boot: download mode and loading with blue screen. First is for flashing a firmware. Second is some strange: device starts with blue screen and on it loading bar or loading line runs like with normal boot but then phone's screen turns into green and nothing more happens. "What is it?" is an open question now.

Key's abbreviations:
  * p - power
  * c - camera
  * g - motion gate
  * b - block or lock key
  * +/- - volume up/down
  * l - call
  * u - cube or menu key
  * , - delimiter of sets

Blue loading:
+-p, g+-p, b+-p, +-lp, +-up, gb+-p, gb-lp, g+-lp, g+-up, b+-lp, b+-up, gb+-lp

Download mode:
c+p, c-p, cg+p, cg-p, cb+p, cb-p, c+-p, c+lp, c+up, c-lp, c-up, clup, -lup, cgb+p, cgb-p, cgblp, cg+-p, cg+lp, cg+up, cg-lp, cg-up, cglup, cb+-p, cb+lp, cb+up, cb-lp, cb-up, cblup, c+-lp, c+-up, c+lup, c-lup, g-lup, b-lup, +-lup, cgb+-p, cgb+lp, cgb+up, cgb-lp, cgb-up, cgblup, cg+-lp, cg+-up, cg+lup, cg-lup, cb+-lp, cb+-up, cb+lup, cb-lup, c+-lup, gb+-up, gb-lup, g+-lup, b+-lup, cgb+-lp, cgb+-up, cgb+lup, cgb-lup, cg+-lup, cb+-lup, gb+-lup, cgb+-lup

Other sets seems to work like a normal boot.

Upload mode:

There is other special bootloader mode. It is upload mode.
It looks like download mode except phrase and color of text message.
The text is "UPLOAD data to pc" and the color is yellow.
According to [DFG](http://darkforestgroup.com/forum/index.php?topic=1013.0) it is needed to obtain debug information when hard problems occur.
So it will start automaticly instead normal boot when you turn on your phone if serious defect is detected.