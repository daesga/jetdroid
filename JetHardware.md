# Specifications #

  * Samsung S3C6410 CPU running at 800 MHz
  * Qualcomm MSM6246 baseband
  * 3.1" inch AMOLED display (480 x 800 pixels) 16M colors
  * 256 MB RAM ( 208 MB for CPU + 32 MB for baseband + 16 MB shared between both )
  * 256 MB + 2 GB Flash ROM (256 MB inside S3C6410 package, 2 GB connected to SD-card port, other amounts are also known depending on exact jet's model number)
  * Dimensions: 109x54x11.9mm; weight 110g
  * 2 GB microSD card included (not always) / expandable up to 32? GB (micro SDHC Sandisk Ultra 16GB was tested)
  * Standard Lithium (LiIon) battery 1080 mAh
  * No Keypad
  * 5 megapixel camera with flash and camcorder with auto-focus
  * WiFi 802.11 b/g, Bluetooth, GPS
  * Accelerometer and proximity sensor
  * Ships with Samsung own System Software
Note: jet is known with different model numbers (S8000, S8000L, S8003 or other). So some characteristics may vary.

Samsung provide jet's short specification [here](http://innovator.samsungmobile.com/prd/sym/productDetl.view.do?modelCode=Jet_cubic31&platformId=12).
Omnia II (GT-I8000) seems to be jet's sister with windows mobile ([samsung's specs](http://innovator.samsungmobile.com/prd/sym/productDetl.view.do?modelCode=GT-i8000&platformId=12)).

# Disassembly #
Pictures of disassembled phones can be found here:
  * FCC report [link](https://fjallfoss.fcc.gov/oetcf/eas/reports/ViewExhibitReport.cfm?mode=Exhibits&RequestTimeout=500&calledFromFrame=N&application_id=186034&fcc_id=%27A3LGTS8000L%27).
  * Handy-faq.de [link](http://www.handy-faq.de/forum/samsung_s8000_jet_forum/98143-s8000_aufgeschraubt.html),
  * Service manual [Google search link](http://www.google.com/search?q=s8000+service+manual)
Instructions on how to disassembly Jet can be found here:
  * formymobile.co.uk guide [link](http://www.formymobile.co.uk/jetdisassembly.php)

# Components #

| **Category** | **Manufacturer** | **PartNumber** | **Information** | **Image** | **Comment** |
|:-------------|:-----------------|:---------------|:----------------|:----------|:------------|
| CPU          | Samsung Semiconductor | [S3C6410](S3C6410.md) | See S3C6410 wiki page |           | 800 MHz     |
| Memory Module | Samsung Semiconductor | KAC00F008M-AE77 | [Brochure](http://www.samsung.com/global/business/semiconductor/support/brochures/downloads/memory/psg_memory_storage_200901.pdf) |           | 256MB OneNAND flash + 2x128MB mobile DDR SDRAM |
| Display      | Samsung Mobile Display (SMD) | AMS310FN07     |                 |           | 480x800 AmOLED, display driver TL2796 |
| Baseband + RF |
| Modem / Baseband | Qualcomm         | MSM6246        | [Press Release](http://www.qualcomm.com/news/releases/2007/071112_Qualcomm_Drives_Migration.html) |           |             |
| RF Frontend  | Qualcomm         | RTR6285        |                 |           | Found in Nexus One with Android |
| RF Power Amplifier (PAM) | Skyworks Inc.    | SKY77336-13    | [Manufacturer's page](http://www.skyworksinc.com/Product.aspx?ProductID=437) |           | Found in Nexus One (teardown [here](http://www.ifixit.com/Teardown/Nexus-One-Teardown/1654/2)) with Android |
| Power + Audio |
| Power Management (PMU) | Maxim            | [MAX8906EWA](MAX8906EWA.md) |                 |           | Includes audio amp, linux kernel support available |
| Audio Codec  | Maxim            | MAX9880        | [Info](http://www.maxim-ic.com/quick_view2.cfm/qv_pk/6363/t/do) |           | High-Performance, Low-Power, Dual I2S, Stereo Audio Codec |
| Battery gauge | Maxim            | MAX17040       | [Datasheet](http://datasheets.maxim-ic.com%2Fen%2Fds%2FMAX17040-MAX17041.pdf) |           | Kernel support available |
| Camera PMIC  | National         | LP8720         | [datasheet](http://www.national.com/ds/LP/LP8720.pdf) |           |             |
| Sensors + Camera |
| Accelerometer | Kionix           | KXSD9          | [Manufacturer's page](http://www.kionix.com/accelerometers/accelerometer-KXSD9.html) |           | Driver for minimal support exists |
| 5M Camera Processor | NEC              | CE131          | [Info1](http://www.nec.co.jp/techrep/en/journal/g09/n01/090106.pdf) [Info2](http://www.necel.com/mobile/en/camera/ce143.html) [Info3](http://www.uberphones.com/2009/02/nec_ce143_chip/) |           | driver available in GT-I9000 source |
| VGA Camera   | Samsung          | S5KA3D         |                 |           | driver available in GT-I9000 source |
| Proximity and ambient light sensor | Sharp            | GP2AP002A00F   | [Info](http://translate.google.com/translate?hl=en&sl=ja&tl=en&u=http%3A%2F%2Fwww.sharp.co.jp%2Fproducts%2Fdevice%2Flineup%2Fselection%2Fopto%2FAdjacentSensor%2Findex.html) |           |             |
| Others       |
| Bluetooth + FM radio + WiFi ??? | Broadcom ???     | Cm FA641301A PQ | [Manufacturer's page](http://www.broadcom.com/products/Bluetooth/Bluetooth-RF-Silicon-and-Software-Solutions/BCM4325) |           | BCM4325 ??? (A) |

(A) note: it is guessed according to broadcom's "Cm" mark (found in Acer N50 on [handhelds.org](http://www.handhelds.org/moin/moin.cgi/AcerN50Hardware)) and functionality not covered by other chips. Manufacturer's driver for Android is known existing.

It is possible to find all parts listed in a shop that provides spare parts. For instance, [this shop](http://www.gsmparts-shop.ru/parts_samsung_1.html) looks interesting to obtain such information.