# MSM part #

| Bus | Part | SDA Pin | SCL Pin | Master / Slave | Function |
|:----|:-----|:--------|:--------|:---------------|:---------|
| FUEL\_GAUGE\_SDA/SCL\_2.6V | UCP300 | H17 (GPIO26|I2C\_SDA) | K22 (GPIO27|I2C\_SCL) | Master         | Fuel Gauge |
| FUEL\_GAUGE\_SDA/SCL\_2.6V | U305 | 8 (SDA) |  9 (SCL) | Slave          | Fuel Gauge |


# S3C part #

| Bus | Part | SDA Pin | SCL Pin | Master / Slave | Function |
|:----|:-----|:--------|:--------|:---------------|:---------|
| AP\_SDA/SCL\_1.8V | UCP701 | H4 (XM0ADDR9) | D10 (XM0ADDR8) | Master         | S3C6410  |
| AP\_SDA/SCL\_1.8V | U400 | B2 (SDA) | B3 (SCL) | Slave          | MAX Audio Codec |
| AP\_SDA/SCL\_1.8V | HEA502 | 27      | 28      | Connector      | VGA Cam / ALS |
|     |
| AP\_SDA/SCL\_3.0V | UCP701 | A19 (XI2CSDA) | A18 (XI2CSCL) | Master         | S3C6410  |
| AP\_SDA/SCL\_3.0V | HEA502 | 21      | 19      | Connector      | VGA Cam / ALS |
| AP\_SDA/SCL\_3.0V | HEA500 | 5       | 6       | Connector      | 5M Cam   |
| AP\_SDA/SCL\_3.0V | HEA600 | 31      | 32      | Connector      | Sensors  |
|     |
| FM\_SDA/SCL\_3.0V | UCP701 | J25 (XHICSN\_MAIN) | L25 (XHICSN) | Master         | S3C6410  |
| FM\_SDA/SCL\_3.0V | U501 | C4 (SDA) | C3 (SCL) | Slave          | Camera LDO |
| FM\_SDA/SCL\_3.0V | U202 | 7 (SDIO) | 6 (SCLK) | Slave          | FM Radio |
|     |
| USBSW\_SDA/SCL\_3.0V | UCP701 | [R20](https://code.google.com/p/jetdroid/source/detail?r=20) (XHIDATA7) | E26 (XHIDATA6) | Master         | S3C6410  |
| USBSW\_SDA/SCL\_3.0V | U600 | B2 (I2C\_SDA) | C2 (I2C\_SCL) | Slave          | USB switch |
|     |
| PWR\_SDA/SCL\_3.0V | UCP701 | T15 (XEINT10) | AA17 (XEINT9) | Master         | S3C6410  |
| PWR\_SDA/SCL\_3.0V | PMIC200 | F5 (SDA) | E6 (SCL) | Slave          | PMU      |