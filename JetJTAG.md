# Introduction #

The phone contains an unmounted 10-pin connector that features the [JTAG](JTAG.md) port to the S3C6410 JTAG interface

# Connector #

[![](http://farm3.static.flickr.com/2715/4266222404_ba0734a6a2.jpg)](http://www.flickr.com/photos/44723902@N02/4266222404/)

A connector that fits perfectly to this footprint is [AXT610124](http://www.panasonic-electric-works.com/catalogues/downloads/connectors/ds_65316_0000_en_axe5_6.pdf) (part of the AXE5/6 or FS4 Series) by Panasonic Electric Works. The header is shown on the bottom right in below picture. It can be ordered e.g. at DigiKey (part# [255-2406-1-ND](http://search.digikey.com/scripts/DkSearch/dksus.dll?Detail&name=255-2406-1-ND)).
You can see such connector on other side of the board. It connects jack 3.5 to the board.

![http://farm3.static.flickr.com/2803/4268709243_f55f21f832.jpg](http://farm3.static.flickr.com/2803/4268709243_f55f21f832.jpg)

# Pinout #
The pins of the connector are numbered like below
| 9 | 7 | 5 | 3 | 1 |
|:--|:--|:--|:--|:--|
| 10 | 8 | 6 | 4 | 2 |

Below is the signal assignment.

| **PIN** | **Signal** | **Description** |
|:--------|:-----------|:----------------|
| 1       | Vcc        | Power Supply    |
| 2       | TCK        | Test Clock      |
| 3       | nTRST      |                 |
| 4       | RTCK       |                 |
| 5       | TDI        | Test Data In    |
| 6       | TDO        | Test Data Out   |
| 7       | TMS        | Test Mode Select |
| 8       | SYSRST     |                 |
| 9       | NC         |  not connected (A) |
| 10      | GND        | Ground          |

4 big pins around these are mounting points. They are intended to carry a connector. It seems they are ground as 10 pin.

(A) note: it seems to be not connected as someone can see on the photo. It is also heard to be GND. Some pinouts can be found [here @hardwarebook.info](http://www.hardwarebook.info/JTAG).

# Links #
  * [S8000 repair guide](http://www.omnia-repair.com/forum/topic/s8000-repair-guide)