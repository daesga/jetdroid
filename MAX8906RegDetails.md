| **Index (hex)**) | **Register** | **slave addr**  | **reg addr**  | **mask** | **clear** | **shift** | **Name** |
|:-----------------|:-------------|:----------------|:--------------|:---------|:----------|:----------|:---------|
|                  |              |                 |               |          |           |           | B A T T E R Y   C H A R G E R S |
| 0 (0)            | CHG\_CNTL1   | 0x78            | 0x7C          | 0x80     | 0x7F      | 0x07      | nCHGEN   |
| 1 (1)            |              | 0x78            | 0x7C          | 0x60     | 0x9F      | 0x05      | CHG\_TOPOFF\_TH |
| 2 (2)            |              | 0x78            | 0x7C          | 0x18     | 0xE7      | 0x03      | CHG\_RST\_HYS |
| 3 (3)            |              | 0x78            | 0x7C          | 0x07     | 0xF8      | 0x00      | AC\_FCHG |
| 4 (4)            | CHG\_CNTL2   | 0x78            | 0x7D          | 0xC0     | 0x3F      | 0x06      | VBUS\_FCHG |
| 5 (5)            |              | 0x78            | 0x7D          | 0x30     | 0xCF      | 0x04      | FCHG\_TMR |
| 6 (6)            |              | 0x78            | 0x7D          | 0x08     | 0xF7      | 0x03      | MBAT\_REG\_TH |
| 7 (7)            |              | 0x78            | 0x7D          | 0x07     | 0xF8      | 0x00      | MBATT\_THERM\_REG) |
| 8 (8)            | CHG\_IRQ1    | 0x78            | 0x7E          | 0x80     | 0x7F      | 0x07      | VAC\_R   |
| 9 (9)            |              | 0x78            | 0x7E          | 0x40     | 0xBF      | 0x06      | VAC\_F   |
| 10 (A)           |              | 0x78            | 0x7E          | 0x20     | 0xDF      | 0x05      | VAC\_OVP |
| 11 (B)           |              | 0x78            | 0x7E          | 0x10     | 0xEF      | 0x04      | VBUS\_R  |
| 12 (C)           |              | 0x78            | 0x7E          | 0x08     | 0xF7      | 0x03      | VBUS\_F  |
| 13 (D)           |              | 0x78            | 0x7E          | 0x04     | 0xFB      | 0x02      | VBUS\_OVP |
| 14 (E)           | CHG\_IRQ2    | 0x78            | 0x7F          | 0x80     | 0x7F      | 0x07      | CHG\_TMR\_FAULT |
| 15 (F)           |              | 0x78            | 0x7F          | 0x40     | 0xBF      | 0x06      | CHG\_TOPOFF |
| 16 (10)          |              | 0x78            | 0x7F          | 0x20     | 0xDF      | 0x05      | CHG\_DONE |
| 17 (11)          |              | 0x78            | 0x7F          | 0x10     | 0xEF      | 0x04      | CHG\_RST |
| 18 (12)          |              | 0x78            | 0x7F          | 0x08     | 0xF7      | 0x03      | MBATTLOWR |
| 19 (13)          |              | 0x78            | 0x7F          | 0x04     | 0xFB      | 0x02      | MBATTLOWF |
| 20 (14)          | CHG\_IRQ1\_MASK | 0x78            | 0x80          | 0x80     | 0x7F      | 0x07      | VAC\_R\_MASK |
| 21 (15)          |              | 0x78            | 0x80          | 0x40     | 0xBF      | 0x06      | VAC\_F\_MASK |
| 22 (16)          |              | 0x78            | 0x80          | 0x20     | 0xDF      | 0x05      | VAC\_OVP\_MASK |
| 23 (17)          |              | 0x78            | 0x80          | 0x10     | 0xEF      | 0x04      | VBUS\_R\_MASK |
| 24 (18)          |              | 0x78            | 0x80          | 0x08     | 0xF7      | 0x03      | VBUS\_F\_MASK |
| 25 (19)          |              | 0x78            | 0x80          | 0x04     | 0xFB      | 0x02      | VBUS\_OVP\_MASK |
| 26 (1A)          | CHG\_IRQ2\_MASK  | 0x78            | 0x81          | 0x80     | 0x7F      | 0x07      | CHG\_TMR\_FAULT\_MASK |
| 27 (1B)          |              | 0x78            | 0x81          | 0x40     | 0xBF      | 0x06      | CHG\_TOPOFF\_MASK |
| 28 (1C)          |              | 0x78            | 0x81          | 0x20     | 0xDF      | 0x05      | CHG\_DONE\_MASK |
| 29 (1D)          |              | 0x78            | 0x81          | 0x10     | 0xEF      | 0x04      | CHG\_RST\_MASK |
| 30 (1E)          |              | 0x78            | 0x81          | 0x08     | 0xF7      | 0x03      | MBATTLOWR\_MASK |
| 31 (1F)          |              | 0x78            | 0x81          | 0x04     | 0xFB      | 0x02      | MBATTLOWF\_MASK |
| 32 (20)          | CHG\_STAT    | 0x78            | 0x82          | 0x80     | 0x7F      | 0x07      | VAC\_OK  |
| 33 (21)          |              | 0x78            | 0x82          | 0x40     | 0xBF      | 0x06      | VBUS\_OK |
| 34 (22)          |              | 0x78            | 0x82          | 0x20     | 0xDF      | 0x05      | CHG\_TMR |
| 35 (23)          |              | 0x78            | 0x82          | 0x10     | 0xEF      | 0x04      | CHG\_EN\_STAT |
| 36 (24)          |              | 0x78            | 0x82          | 0x0C     | 0xF3      | 0x02      | CHG\_MODE |
| 37 (25)          |              | 0x78            | 0x82          | 0x02     | 0xFD      | 0x01      | MBATT\_DET |
| 38 (26)          |              | 0x78            | 0x82          | 0x01     | 0xFE      | 0x00      | MBATTLOW |
| 39 (27)          | BBATTCNFG    | 0x78            | 0x78          | 0x80     | 0x7F      | 0x07      | APPALLOFF |
| 40 (28)          |              | 0x78            | 0x78          | 0x03     | 0xFC      | 0x00      | VBBATTCV |
|                  |              |                 |               |          |           |           | S T E P - D O W N    R E G U L A T O R S |
| 41 (29)          | WBBCOREEN    | 0x78            | 0x5C          | 0x80     | 0x7F      | 0x07      | nWCRADE  |
| 42 (2A)          |              | 0x78            | 0x5C          | 0x0E     | 0xF1      | 0x01      | WCRENSRC |
| 43 (2B)          |              | 0x78            | 0x5C          | 0x01     | 0xFE      | 0x00      | WCREN    |
| 44 (2C)          | WBBCOREFSEQ  | 0x78            | 0x5D          | 0xF0     | 0x0F      | 0x04      | WCRFSEQPU |
| 45 (2D)          |              | 0x78            | 0x5D          | 0x0F     | 0xF0      | 0x00      | WCRFSEQPD |
| 46 (2E)          | WBBCORETV    | 0x78            | 0x5E          | 0x3F     | 0xC0      | 0x00      | WCRTV    |
| 47 (2F)          | WBBRFEN      | 0x78            | 0x9C          | 0x80     | 0x7F      | 0x07      | nWRFADE  |
| 48 (30)          |              | 0x78            | 0x9C          | 0x0E     | 0xF1      | 0x01      | WRFENSRC |
| 49 (31)          |              | 0x78            | 0x9C          | 0x01     | 0xFE      | 0x00      | WRFEN    |
| 50 (32)          | WBBRFFSEQ    | 0x78            | 0x9D          | 0xF0     | 0x0F      | 0x04      | WRFFSEQPU |
| 51 (33)          |              | 0x78            | 0x9D          | 0x0F     | 0xF0      | 0x00      | WRFFSEQPD |
| 52 (34)          | WBBRFTV      | 0x78            | 0x9E          | 0x3F     | 0xC0      | 0x00      | WRFTV    |
| 53 (35)          | APPSEN       | 0x78            | 0x04          | 0x80     | 0x7F      | 0x07      | nAPPSADE |
| 54 (36)          |              | 0x78            | 0x04          | 0x10     | 0xEF      | 0x04      | nOVER1ENAPPS |
| 55 (37)          |              | 0x78            | 0x04          | 0x0E     | 0xF1      | 0x01      | APPSENSRC |
| 56 (38)          |              | 0x78            | 0x04          | 0x01     | 0xFE      | 0x00      | APPSEN   |
| 57 (39)          | OVER1        | 0x68            | 0x10          | 0x04     | 0xFB      | 0x02      | ENSRAM   |
| 58 (3A)          |              | 0x68            | 0x10          | 0x01     | 0xFE      | 0x00      | ENAPPS   |
| 59 (3B)          | APPSFSEQ     | 0x78            | 0x05          | 0xF0     | 0x0F      | 0x04      | APPSFSEQPU |
| 60 (3C)          |              | 0x78            | 0x05          | 0x0F     | 0xF0      | 0x00      | APPSFSEQPD |
| 61 (3D)          | ADTV1        | 0x68            | 0x23          | 0x80     | 0x7F      | 0x07      | T1AOST   |
| 62 (3E)          |              | 0x68            | 0x23          | 0x3F     | 0xC0      | 0x00      | T1APPS   |
| 63 (3F)          | ADTV2        | 0x68            | 0x24          | 0x80     | 0x7F      | 0x07      | T2AOST   |
| 64 (40)          |              | 0x68            | 0x24          | 0x3F     | 0xC0      | 0x00      | T2APPS   |
| 65 (41)          | APPSCLG      | 0x78            | 0x06          | 0x3F     | 0xC0      | 0x00      | CLGAPPS  |
| 66 (42)          | VCC1         | 0x68            | 0x20          | 0x80     | 0x7F      | 0x07      | MVS      |
| 67 (43)          |              | 0x68            | 0x20          | 0x40     | 0xBF      | 0x06      | MGO      |
| 68 (44)          |              | 0x68            | 0x20          | 0x20     | 0xDF      | 0x05      | SVS      |
| 69 (45)          |              | 0x68            | 0x20          | 0x10     | 0xEF      | 0x04      | SGO      |
| 70 (46)          |              | 0x68            | 0x20          | 0x02     | 0xFD      | 0x01      | AVS      |
| 71 (47)          |              | 0x68            | 0x20          | 0x01     | 0xFE      | 0x00      | AGO      |
| 72 (48)          | IOEN         | 0x78            | 0x08          | 0x80     | 0x7F      | 0x07      | nIOADE   |
| 73 (49)          |              | 0x78            | 0x08          | 0x0E     | 0xF1      | 0x01      | IOENSRC  |
| 74 (4A)          |              | 0x78            | 0x08          | 0x01     | 0xFE      | 0x00      | IOEN     |
| 75 (4B)          | IOFSEQ       | 0x78            | 0x09          | 0xF0     | 0x0F      | 0x04      | IOFSEQPU |
| 76 (4C)          |              | 0x78            | 0x09          | 0x0F     | 0xF0      | 0x00      | IOFSEQPD |
| 77 (4D)          | MEMEN        | 0x78            | 0x0C          | 0x80     | 0x7F      | 0x07      | nMEMADE  |
| 78 (4E)          |              | 0x78            | 0x0C          |    0x30  | 0xCF      | 0x04      | MEMDVM   |
| 79 (4F)          |              | 0x78            | 0x0C          | 0x0E     | 0xF1      | 0x01      | MEMENSRC |
| 80 (50)          |              | 0x78            | 0x0C          | 0x01     | 0xFE      | 0x00      | MEMEN    |
| 81 (51)          | MEMFSEQ      | 0x78            | 0x0D          | 0xF0     | 0x0F      | 0x04      | MEMFSEQPU |
| 82 (52)          |              | 0x78            | 0x0D          | 0x0F     | 0xF0      | 0x00      | MEMFSEQPD |
|                  |              |                 |               |          |           |           | L I N E A R   R E G U L A T O R S |
| 83 (53)          | WBBMEMEN     | 0x78            | 0x10          | 0x80     | 0x7F      | 0x07      | nWMEMADE |
| 84 (54)          |              | 0x78            | 0x10          | 0x0E     | 0xF1      | 0x01      | WMEMENSRC |
| 85 (55)          |              | 0x78            | 0x10          | 0x01     | 0xFE      | 0x00      | WMEMEN   |
| 86 (56)          | WBBMEMFSEQ   | 0x78            | 0x11          | 0xF0     | 0x0F      | 0x04      | WMEMFSEQPU |
| 87 (57)          |              | 0x78            | 0x11          | 0x0F     | 0xF0      | 0x00      | WMEMFSEQPD |
| 88 (58)          | WBBMEMTV     | 0x78            | 0x12          | 0x3F     | 0xC0      | 0x00      | WMEMTV   |
| 89 (59)          | WBBIOEN      | 0x78            | 0x14          | 0x80     | 0x7F      | 0x07      | nWIOADE  |
| 90 (5A)          |              | 0x78            | 0x14          | 0x10     | 0xEF      | 0x04      | SFTRSTWBB |
| 91 (5B)          |              | 0x78            | 0x14          | 0x0E     | 0xF1      | 0x01      | WIOENSRC |
| 92 (5C)          |              | 0x78            | 0x14          | 0x01     | 0xFE      | 0x00      | WIOEN    |
| 93 (5D)          | WBBIOFSEQ    | 0x78            | 0x15          | 0xF0     | 0x0F      | 0x04      | WIOFSEQPU |
| 94 (5E)          |              | 0x78            | 0x15          | 0x0F     | 0xF0      | 0x00      | WIOFSEQPD |
| 95 (5F)          | WBBIOTV      | 0x78            | 0x16          | 0x3F     | 0xC0      | 0x00      | WIOTV    |
| 96 (60)          | WBBANAEN     | 0x78            | 0x18          | 0x80     | 0x7F      | 0x07      | nWANAADE |
| 97 (61)          |              | 0x78            | 0x18          | 0x0E     | 0xF1      | 0x01      | WANAENSRC |
| 98 (62)          |              | 0x78            | 0x18          | 0x01     | 0xFE      | 0x00      | WANAEN   |
| 99 (63)          | WBBANAFSEQ   | 0x78            | 0x19          | 0xF0     | 0x0F      | 0x04      | WANAFSEQPU |
| 100 (64)         |              | 0x78            | 0x19          | 0x0F     | 0xF0      | 0x00      | WANAFSEQPD |
| 101 (65)         | WBBANATV     | 0x78            | 0x1A          | 0x3F     | 0xC0      | 0x00      | WANATV   |
| 102 (66)         | RFRXLEN      | 0x78            | 0x1C          | 0x80     | 0x7F      | 0x07      | nRFRXLADE |
| 103 (67)         |              | 0x78            | 0x1C          | 0x0E     | 0xF1      | 0x01      | RFRXLENSRC |
| 104 (68)         |              | 0x78            | 0x1C          | 0x01     | 0xFE      | 0x00      | RFRXLEN  |
| 105 (69)         | RFRXLFSEQ    | 0x78            | 0x1D          | 0xF0     | 0x0F      | 0x04      | RFRXLFSEQPU |
| 106 (6A)         |              | 0x78            | 0x1D          | 0x0F     | 0xF0      | 0x00      | RFRXLFSEQPD |
| 107 (6B)         | RFRXLTV      | 0x78            | 0x1E          | 0x3F     | 0xC0      | 0x00      | RFRXLTV  |
| 108 (6C)         | RFTXLEN      | 0x78            | 0x20          | 0x80     | 0x7F      | 0x07      | nRFTXLADE |
| 109 (6D)         |              | 0x78            | 0x20          | 0x0E     | 0xF1      | 0x01      | RFTXLENSRC |
| 110 (6E)         |              | 0x78            | 0x20          | 0x01     | 0xFE      | 0x00      | RFTXLEN  |
| 111 (6F)         | RFTXLFSEQ    | 0x78            | 0x21          | 0xF0     | 0x0F      | 0x04      | RFTXLFSEQPU |
| 112 (70)         |              | 0x78            | 0x21          | 0x0F     | 0xF0      | 0x00      | RFTXLFSEQPD |
| 113 (71)         | RFTXLTV      | 0x78            | 0x22          | 0x3F     | 0xC0      | 0x00      | RFTXLTV  |
| 114 (72)         | RFRXHEN      | 0x78            | 0x24          | 0x80     | 0x7F      | 0x07      | nRFRXHADE |
| 115 (73)         |              | 0x78            | 0x24          | 0x0E     | 0xF1      | 0x01      | RFRXHENSRC |
| 116 (74)         |              | 0x78            | 0x24          | 0x01     | 0xFE      | 0x00      | RFRXHEN  |
| 117 (75)         | RFRXHFSEQ    | 0x78            | 0x25          | 0xF0     | 0x0F      | 0x04      | RFRXHFSEQPU |
| 118 (76)         |              | 0x78            | 0x25          | 0x0F     | 0xF0      | 0x00      | RFRXHFSEQPD |
| 119 (77)         | RFRXHTV      | 0x78            | 0x26          | 0x3F     | 0xC0      | 0x00      | RFRXHTV  |
| 120 (78)         | RFTCXOEN     | 0x78            | 0x28          | 0x80     | 0x7F      | 0x07      | nRFTCXOADE |
| 121 (79)         |              | 0x78            | 0x28          | 0x0E     | 0xF1      | 0x01      | RFTCXOENSRC |
| 122 (7A)         |              | 0x78            | 0x28          | 0x01     | 0xFE      | 0x00      | RFTCXOEN |
| 123 (7B)         | RFTCXOFSEQ   | 0x78            | 0x29          | 0xF0     | 0x0F      | 0x04      | RFTCXOFSEQPU |
| 124 (7C)         |              | 0x78            | 0x29          | 0x0F     | 0xF0      | 0x00      | RFTCXOFSEQPD |
| 125 (7D)         | RFTCXOTV     | 0x78            | 0x2A          | 0x3F     | 0xC0      | 0x00      | RFTCXOLTV |
| 126 (7E)         | LDOAEN       | 0x78            | 0x2C          | 0x80     | 0x7F      | 0x07      | nLDOAADE |
| 127 (7F)         |              | 0x78            | 0x2C          | 0x0E     | 0xF1      | 0x01      | LDOAENSRC |
| 128 (80)         |              | 0x78            | 0x2C          | 0x01     | 0xFE      | 0x00      | LDOAEN   |
| 129 (81)         | LDOAFSEQ     | 0x78            | 0x2D          | 0xF0     | 0x0F      | 0x04      | LDOAFSEQPU |
| 130 (82)         |              | 0x78            | 0x2D          | 0x0F     | 0xF0      | 0x00      | LDOAFSEQPD |
| 131 (83)         | LDOATV       | 0x78            | 0x2E          | 0x3F     | 0xC0      | 0x00      | LDOATV   |
| 132 (84)         | LDOBEN       | 0x78            | 0x30          | 0x80     | 0x7F      | 0x07      | nLDOBADE |
| 133 (85)         |              | 0x78            | 0x30          | 0x0E     | 0xF1      | 0x01      | LDOBENSRC |
| 134 (86)         |              | 0x78            | 0x30          | 0x01     | 0xFE      | 0x00      | LDOBEN   |
| 135 (87)         | LDOBFSEQ     | 0x78            | 0x31          | 0xF0     | 0x0F      | 0x04      | LDOBFSEQPU |
| 136 (88)         |              | 0x78            | 0x31          | 0x0F     | 0xF0      | 0x00      | LDOBFSEQPD |
| 137 (89)         | LDOBTV       | 0x78            | 0x32          | 0x3F     | 0xC0      | 0x00      | LDOBTV   |
| 138 (8A)         | LDOCEN       | 0x78            | 0x34          | 0x80     | 0x7F      | 0x07      | nLDOCADE |
| 139 (8B)         |              | 0x78            | 0x34          | 0x0E     | 0xF1      | 0x01      | LDOCENSRC |
| 140 (8C)         |              | 0x78            | 0x34          | 0x01     | 0xFE      | 0x00      | LDOCEN   |
| 141 (8D)         | LDOCFSEQ     | 0x78            | 0x35          | 0xF0     | 0x0F      | 0x04      | LDOCFSEQPU |
| 142 (8E)         |              | 0x78            | 0x35          | 0x0F     | 0xF0      | 0x00      | LDOCFSEQPD |
| 143 (8F)         | LDOCTV       | 0x78            | 0x36          | 0x3F     | 0xC0      | 0x00      | LDOCTV   |
| 144 (90)         | LDODEN       | 0x78            | 0x38          | 0x80     | 0x7F      | 0x07      | nLDODADE |
| 145 (91)         |              | 0x78            | 0x38          | 0x0E     | 0xF1      | 0x01      | LDODENSRC |
| 146 (92)         |              | 0x78            | 0x38          | 0x01     | 0xFE      | 0x00      | LDODEN   |
| 147 (93)         | LDODFSEQ     | 0x78            | 0x39          | 0xF0     | 0x0F      | 0x04      | LDODFSEQPU |
| 148 (94)         |              | 0x78            | 0x39          | 0x0F     | 0xF0      | 0x00      | LDODFSEQPD |
| 149 (95)         | LDODTV       | 0x78            | 0x3A          | 0x3F     | 0xC0      | 0x00      | LDODTV   |
| 150 (96)         | SIMLTEN      | 0x78            | 0x3C          | 0x80     | 0x7F      | 0x07      | nSIMLTADE |
| 151 (97)         |              | 0x78            | 0x3C          | 0x0E     | 0xF1      | 0x01      | SIMLTENSRC |
| 152 (98)         |              | 0x78            | 0x3C          | 0x01     | 0xFE      | 0x00      | SIMLTEN  |
| 153 (99)         | SIMLTFSEQ    | 0x78            | 0x3D          | 0xF0     | 0x0F      | 0x04      | SIMLTFSEQPU |
| 154 (9A)         |              | 0x78            | 0x3D          | 0x0F     | 0xF0      | 0x00      | SIMLTFSEQPD |
| 155 (9B)         | SIMLTTV      | 0x78            | 0x3E          | 0x3F     | 0xC0      | 0x00      | SIMLTTV  |
| 156 (9C)         | SRAMEN       | 0x78            | 0x40          | 0x80     | 0x7F      | 0x07      | nSRAMADE |
| 157 (9D)         |              | 0x78            | 0x40          | 0x10     | 0xEF      | 0x04      | nOVER1ENSRAM |
| 158 (9E)         |              | 0x78            | 0x40          | 0x0E     | 0xF1      | 0x01      | SRAMENSRC |
| 159 (9F)         |              | 0x78            | 0x40          | 0x01     | 0xFE      | 0x00      | SRAMEN   |
| 160 (A0)         | SRAMFSEQ     | 0x78            | 0x41          | 0xF0     | 0x0F      | 0x04      | SRAMFSEQPU |
| 161 (A1)         |              | 0x78            | 0x41          | 0x0F     | 0xF0      | 0x00      | SRAMFSEQPD |
| 162 (A2)         | SDTV1        | 0x68            | 0x29          | 0x80     | 0x7F      | 0x07      | T1SOST   |
| 163 (A3)         |              | 0x68            | 0x29          | 0x3F     | 0xC0      | 0x00      | T1SRAM   |
| 164 (A4)         | SDTV2        | 0x68            | 0x2A          | 0x80     | 0x7F      | 0x07      | T2SOST   |
| 165 (A5)         |              | 0x68            | 0x2A          | 0x3F     | 0xC0      | 0x00      | T2SRAM   |
| 166 (A6)         | SRAMCLG      | 0x78            | 0x42          | 0x3F     | 0xC0      | 0x00      | CLGSRAM  |
| 167 (A7)         | CARD1EN      | 0x78            | 0x44          | 0x80     | 0x7F      | 0x07      | nCARD1ADE |
| 168 (A8)         |              | 0x78            | 0x44          | 0x0E     | 0xF1      | 0x01      | CARD1ENSRC |
| 169 (A9)         |              | 0x78            | 0x44          | 0x01     | 0xFE      | 0x00      | CARD1EN  |
| 170 (AA)         | CARD1FSEQ    | 0x78            | 0x45          | 0xF0     | 0x0F      | 0x04      | CARD1FSEQPU |
| 171 (AB)         |              | 0x78            | 0x45          | 0x0F     | 0xF0      | 0x00      | CARD1FSEQPD |
| 172 (AC)         | CARD1TV      | 0x78            | 0x46          | 0x3F     | 0xC0      | 0x00      | CARD1TV  |
| 173 (AD)         | CARD2EN      | 0x78            | 0x48          | 0x80     | 0x7F      | 0x07      | nCARD2ADE |
| 174 (AE)         |              | 0x78            | 0x48          | 0x0E     | 0xF1      | 0x01      | CARD2ENSRC |
| 175 (AF)         |              | 0x78            | 0x48          | 0x01     | 0xFE      | 0x00      | CARD2EN  |
| 176 (B0)         | CARD2FSEQ    | 0x78            | 0x49          | 0xF0     | 0x0F      | 0x04      | CARD2FSEQPU |
| 177 (B1)         |              | 0x78            | 0x49          | 0x0F     | 0xF0      | 0x00      | CARD2FSEQPD |
| 178 (B2)         | CARD2TV      | 0x78            | 0x4A          | 0x3F     | 0xC0      | 0x00      | CARD2TV  |
| 179 (B3)         | MVTENEN      | 0x78            | 0x4C          | 0x80     | 0x7F      | 0x07      | nMVTADE  |
| 180 (B4)         |              | 0x78            | 0x4C          | 0x0E     | 0xF1      | 0x01      | MVTENSRC |
| 181 (B5)         |              | 0x78            | 0x4C          | 0x01     | 0xFE      | 0x00      | MVTEN    |
| 182 (B6)         | MVTFSEQ      | 0x78            | 0x4D          | 0xF0     | 0x0F      | 0x04      | MVTFSEQPU |
| 183 (B7)         |              | 0x78            | 0x4D          | 0x0F     | 0xF0      | 0x00      | MVTFSEQPD |
| 184 (B8)         | MDTV1        | 0x78            | 0x32          | 0x0F     | 0xF0      | 0x00      | T1MVT    |
| 185 (B9)         | MDTV2        | 0x78            | 0x33          | 0x0F     | 0xF0      | 0x00      | T2MVT    |
| 186 (BA)         | BIASEN       | 0x78            | 0x50          | 0x80     | 0x7F      | 0x07      | nBIASADE |
| 187 (BB)         |              | 0x78            | 0x50          | 0x0E     | 0xF1      | 0x01      | BIASENSRC |
| 188 (BC)         |              | 0x78            | 0x50          | 0x01     | 0xFE      | 0x00      | BIASEN   |
| 189 (BD)         | BIASFSEQ     | 0x78            | 0x51          | 0xF0     | 0x0F      | 0x04      | BIASFSEQPU |
| 190 (BE)         |              | 0x78            | 0x51          | 0x0F     | 0xF0      | 0x00      | BIASFSEQPD |
| 191 (BF)         | BIASTV       | 0x78            | 0x52          | 0x3F     | 0xC0      | 0x00      | BIASTV   |
| 192 (C0)         | VBUSEN       | 0x78            | 0x54          | 0x80     | 0x7F      | 0x07      | nVBUSADE |
| 193 (C1)         |              | 0x78            | 0x54          | 0x10     | 0xEF      | 0x04      | VBUSVINEN |
| 194 (C2)         |              | 0x78            | 0x54          | 0x0E     | 0xF1      | 0x01      | VBUSENSRC |
| 195 (C3)         |              | 0x78            | 0x54          | 0x01     | 0xFE      | 0x00      | VBUSEN   |
| 196 (C4)         | VBUSFSEQ     | 0x78            | 0x55          | 0xF0     | 0x0F      | 0x04      | VBUSFSEQPU |
| 197 (C5)         |              | 0x78            | 0x55          | 0x0F     | 0xF0      | 0x00      | VBUSFSEQPD |
| 198 (C6)         | USBTXRXEN    | 0x78            | 0x58          | 0x80     | 0x7F      | 0x07      | nUSBTXRXADE |
| 199 (C7)         |              | 0x78            | 0x58          | 0x10     | 0xEF      | 0x04      | USBTXRXVINEN |
| 200 (C8)         |              | 0x78            | 0x58          | 0x0E     | 0xF1      | 0x01      | USBTXRXENSRC |
| 201 (C9)         |              | 0x78            | 0x58          | 0x01     | 0xFE      | 0x00      | USBTXRXEN |
| 202 (CA)         | USBTXRXFSEQ  | 0x78            | 0x59          | 0xF0     | 0x0F      | 0x04      | USBTXRXFSEQPU |
| 203 (CB)         |              | 0x78            | 0x59          | 0x0F     | 0xF0      | 0x00      | USBTXRXFSEQPD |
|                  |              |                 |               |          |           |           | M A I N - B A T T E R Y   F A U L T   D E T E C T O R |
| 204 (CC)         | LBCNFG       | 0x78            | 0x60          | 0x30     | 0xCF      | 0x04      | LHYST    |
| 205 (CD)         |              | 0x78            | 0x60          | 0x0E     | 0xF1      | 0x01      | LBDAC    |
| 206 (CE)         |              | 0x78            | 0x60          | 0x01     | 0xFE      | 0x00      | LBEN     |
|                  |              |                 |               |          |           |           | O N / O F F   C O N T R O L L E R |
| 207 (CF)         | EXTWKSEL     | 0x78            | 0x00          | 0x80     | 0x7F      | 0x07      | HRDRSTEN |
| 208 (D0)         |              | 0x78            | 0x00          | 0x40     | 0xBF      | 0x06      | ????     |
| 209 (D1)         |              | 0x78            | 0x00          | 0x10     | 0xEF      | 0x04      | WKVBUS   |
| 210 (D2)         |              | 0x78            | 0x00          | 0x08     | 0xF7      | 0x03      | WKVAC    |
| 211 (D3)         |              | 0x78            | 0x00          | 0x04     | 0xFB      | 0x02      | WKALRM1R |
| 212 (D4)         |              | 0x78            | 0x00          | 0x02     | 0xFD      | 0x01      | WKALRM0R |
| 213 (D5)         |              | 0x78            | 0x00          | 0x01     | 0xFE      | 0x00      | WKSW     |
| 214 (D6)         | ON\_OFF\_IRQ | 0x78            | 0x01          | 0x80     | 0x7F      | 0x07      | SW\_R    |
| 215 (D7)         |              | 0x78            | 0x01          | 0x40     | 0xBF      | 0x06      | SW\_F    |
| 216 (D8)         |              | 0x78            | 0x01          | 0x20     | 0xDF      | 0x05      | SW\_1SEC |
| 217 (D9)         |              | 0x78            | 0x01          | 0x10     | 0xEF      | 0x04      | JIG\_R   |
| 218 (DA)         |              | 0x78            | 0x01          | 0x08     | 0xF7      | 0x03      | JIG\_F   |
| 219 (DB)         |              | 0x78            | 0x01          | 0x04     | 0xFB      | 0x02      | SW\_3SEC |
| 220 (DC)         |              | 0x78            | 0x01          | 0x02     | 0xFD      | 0x01      | MPL\_EVENT |
| 221 (DD)         | ON\_OFF\_IRQ\_MASK | 0x78            | 0x02          | 0x80     | 0x7F      | 0x07      | SW\_R\_MASK |
| 222 (DE)         |              | 0x78            | 0x02          | 0x40     | 0xBF      | 0x06      | SW\_F\_MASK |
| 223 (DF)         |              | 0x78            | 0x02          | 0x20     | 0xDF      | 0x05      | SW\_1SEC\_MASK |
| 224 (E0)         |              | 0x78            | 0x02          | 0x10     | 0xEF      | 0x04      | JIG\_R\_MASK |
| 225 (E1)         |              | 0x78            | 0x02          | 0x08     | 0xF7      | 0x03      | JIG\_F\_MASK |
| 226 (E2)         |              | 0x78            | 0x02          | 0x04     | 0xFB      | 0x02      | SW\_3SEC\_MASK |
| 227 (E3)         |              | 0x78            | 0x02          | 0x02     | 0xFD      | 0x01      | MPL\_EVENT\_MASK |
| 228 (E4)         | ON\_OFF\_STAT | 0x78            | 0x03          | 0x80     | 0x7F      | 0x07      | SW       |
| 229 (E5)         |              | 0x78            | 0x03          | 0x40     | 0xBF      | 0x06      | SW\_1SEC |
| 230 (E6)         |              | 0x78            | 0x03          | 0x20     | 0xDF      | 0x05      | JIG      |
| 231 (E7)         |              | 0x78            | 0x03          | 0x10     | 0xEF      | 0x04      | SW\_3SEC |
|                  |              |                 |               |          |           |           | F L E X I B L E   P O W E R   S E Q U E N C E R |
| 232 (E8)         | SEQ1CNFG     | 0x78            | 0x64          | 0x38     | 0xC7      | 0x03      | SEQ1T    |
| 233 (E9)         |              | 0x78            | 0x64          | 0x06     | 0xF9      | 0x01      | SEQ1SRC  |
| 234 (EA)         |              | 0x78            | 0x64          | 0x01     | 0xFE      | 0x00      | SEQ1EN   |
| 235 (EB)         | SEQ2CNFG     | 0x78            | 0x65          | 0x38     | 0xC7      | 0x03      | SEQ2T    |
| 236 (EC)         |              | 0x78            | 0x65          | 0x06     | 0xF9      | 0x01      | SEQ2SRC  |
| 237 (ED)         |              | 0x78            | 0x65          | 0x01     | 0xFE      | 0x00      | SEQ2EN   |
| 238 (EE)         | SEQ3CNFG     | 0x78            | 0x66          | 0x38     | 0xC7      | 0x03      | SEQ3T    |
| 239 (EF)         |              | 0x78            | 0x66          | 0x06     | 0xF9      | 0x01      | SEQ3SRC  |
| 240 (F0)         |              | 0x78            | 0x66          | 0x01     | 0xFE      | 0x00      | SEQ3EN   |
| 241 (F1)         | SEQ4CNFG     | 0x78            | 0x67          | 0x38     | 0xC7      | 0x03      | SEQ4T    |
| 242 (F2)         |              | 0x78            | 0x67          | 0x06     | 0xF9      | 0x01      | SEQ4SRC  |
| 243 (F3)         |              | 0x78            | 0x67          | 0x01     | 0xFE      | 0x00      | SEQ4EN   |
| 244 (F4)         | SEQ5CNFG     | 0x78            | 0x68          | 0x38     | 0xC7      | 0x03      | SEQ5T    |
| 245 (F5)         |              | 0x78            | 0x68          | 0x06     | 0xF9      | 0x01      | SEQ5SRC  |
| 246 (F6)         |              | 0x78            | 0x68          | 0x01     | 0xFE      | 0x00      | SEQ5EN   |
| 247 (F7)         | SEQ6CNFG     | 0x78            | 0x69          | 0x38     | 0xC7      | 0x03      | SEQ6T    |
| 248 (F8)         |              | 0x78            | 0x69          | 0x06     | 0xF9      | 0x01      | SEQ6SRC  |
| 249 (F9)         |              | 0x78            | 0x69          | 0x01     | 0xFE      | 0x00      | SEQ6EN   |
| 250 (FA)         | SEQ7CNFG     | 0x78            | 0x6A          | 0x38     | 0xC7      | 0x03      | SEQ7T    |
| 251 (FB)         |              | 0x78            | 0x6A          | 0x06     | 0xF9      | 0x01      | SEQ7SRC  |
| 252 (FC)         |              | 0x78            | 0x6A          | 0x01     | 0xFE      | 0x00      | SEQ7EN   |
|                  |              |                 |               |          |           |           | U S B   T R A N S C E I V E R |
| 253 (FD)         | USBCNFG      | 0x78            | 0x6C          | 0x30     | 0xCF      | 0x04      | USB\_PU\_EN |
| 254 (FE)         |              | 0x78            | 0x6C          | 0x08     | 0xF7      | 0x03      | USB\_SUSP |
| 255 (FF)         |              | 0x78            | 0x6C          | 0x06     | 0xF9      | 0x01      | USB\_EN  |
|                  |              |                 |               |          |           |           | T C X O   B U F F E R |
| 256 (100)        | TCXOCNFG     | 0x78            | 0x74          | 0x01     | 0xFE      | 0x00      | TCXOEN   |
|                  |              |                 |               |          |           |           | R E F E R E N C E   O U T P U T (R E F O U T)  |
| 257 (101)        | REFOUTCNFG   | 0x78            | 0x70          | 0x01     | 0xFE      | 0x00      | REFOUTEN |
|                  |              |                 |               |          |           |           | R E A L   T I M E   C L O C K (R T C) |
| 258 (102)        | R T C        | 0xD0            | 0x00          | 0x0F     | 0xF0      | 0x00      | RTC\_SEC |
| 259 (103)        |              | 0xD0            | 0x00          | 0x70     | 0x8F      | 0x04      | RTC\_10SEC |
| 260 (104)        |              | 0xD0            | 0x01          | 0x0F     | 0xF0      | 0x00      | RTC\_MIN |
| 261 (105)        |              | 0xD0            | 0x01          | 0x70     | 0x8F      | 0x04      | RTC\_10MIN |
| 262 (106)        |              | 0xD0            | 0x02          | 0x0F     | 0xF0      | 0x00      | RTC\_HOURS |
| 263 (107)        |              | 0xD0            | 0x02          | 0x30     | 0xCF      | 0x04      | RTC\_10HOURS |
| 264 (108)        |              | 0xD0            | 0x02          | 0x80     | 0x7F      | 0x07      | RTC\_12\_n24 |
| 265 (109)        |              | 0xD0            | 0x03          | 0x07     | 0xF8      | 0x00      | RTC\_WEEKDAY |
| 266 (10A)        |              | 0xD0            | 0x04          | 0x0F     | 0xF0      | 0x00      | RTC\_DATE |
| 267 (10B)        |              | 0xD0            | 0x04          | 0x30     | 0xCF      | 0x04      | RTC\_10DATE |
| 268 (10C)        |              | 0xD0            | 0x05          | 0x0F     | 0xF0      | 0x00      | RTC\_MONTH |
| 269 (10D)        |              | 0xD0            | 0x05          | 0x10     | 0xEF      | 0x04      | RTC\_10MONTH |
| 270 (10E)        |              | 0xD0            | 0x06          | 0x0F     | 0xF0      | 0x00      | RTC\_YEAR |
| 271 (10F)        |              | 0xD0            | 0x06          | 0xF0     | 0x0F      | 0x04      | RTC\_10YEAR |
| 272 (110)        |              | 0xD0            | 0x07          | 0x0F     | 0xF0      | 0x00      | RTC\_100YEAR |
| 273 (111)        |              | 0xD0            | 0x07          | 0xF0     | 0x0F      | 0x04      | RTC\_1000YEAR |
| 274 (112)        | ALARM0       | 0xD0            | 0x08          | 0x0F     | 0xF0      | 0x00      | ALARM0\_SEC |
| 275 (113)        |              | 0xD0            | 0x08          | 0x70     | 0x8F      | 0x04      | ALARM0\_10SEC |
| 276 (114)        |              | 0xD0            | 0x09          | 0x0F     | 0xF0      | 0x00      | ALARM0\_MIN |
| 277 (115)        |              | 0xD0            | 0x09          | 0x70     | 0x8F      | 0x04      | ALARM0\_10MIN |
| 278 (116)        |              | 0xD0            | 0x0A          | 0x0F     | 0xF0      | 0x00      | ALARM0\_HOURS |
| 279 (117)        |              | 0xD0            | 0x0A          | 0x30     | 0xCF      | 0x04      | ALARM0\_10HOURS |
| 280 (118)        |              | 0xD0            | 0x0A          | 0x80     | 0x7F      | 0x07      | ALARM0\_12\_n24 |
| 281 (119)        |              | 0xD0            | 0x0B          | 0x07     | 0xF8      | 0x00      | ALARM0\_WEEKDAY |
| 282 (11A)        |              | 0xD0            | 0x0C          | 0x0F     | 0xF0      | 0x00      | ALARM0\_DATE |
| 283 (11B)        |              | 0xD0            | 0x0C          | 0x30     | 0xCF      | 0x04      | ALARM0\_10DATE |
| 284 (11C)        |              | 0xD0            | 0x0D          | 0x0F     | 0xF0      | 0x00      | ALARM0\_MONTH |
| 285 (11D)        |              | 0xD0            | 0x0D          | 0x10     | 0xEF      | 0x04      | ALARM0\_10MONTH |
| 286 (11E)        |              | 0xD0            | 0x0E          | 0x0F     | 0xF0      | 0x00      | ALARM0\_YEAR |
| 287 (11F)        |              | 0xD0            | 0x0E          | 0xF0     | 0x0F      | 0x04      | ALARM0\_10YEAR |
| 288 (120)        |              | 0xD0            | 0x0F          | 0x0F     | 0xF0      | 0x00      | ALARM0\_100YEAR |
| 289 (121)        |              | 0xD0            | 0x0F          | 0xF0     | 0x0F      | 0x04      | ALARM0\_1000YEAR |
| 290 (122)        | ALARM1       | 0xD0            | 0x10          | 0x0F     | 0xF0      | 0x00      | ALARM1\_SEC |
| 291 (123)        |              | 0xD0            | 0x10          | 0x70     | 0x8F      | 0x04      | ALARM1\_10SEC |
| 292 (124)        |              | 0xD0            | 0x11          | 0x0F     | 0xF0      | 0x00      | ALARM1\_MIN |
| 293 (125)        |              | 0xD0            | 0x11          | 0x70     | 0x8F      | 0x04      | ALARM1\_10MIN |
| 294 (126)        |              | 0xD0            | 0x12          | 0x0F     | 0xF0      | 0x00      | ALARM1\_HOURS |
| 295 (127)        |              | 0xD0            | 0x12          | 0x30     | 0xCF      | 0x04      | ALARM1\_10HOURS |
| 296 (128)        |              | 0xD0            | 0x12          | 0x80     | 0x7F      | 0x07      | ALARM1\_12\_n24 |
| 297 (129)        |              | 0xD0            | 0x13          | 0x07     | 0xF8      | 0x00      | ALARM1\_WEEKDAY |
| 298 (12A)        |              | 0xD0            | 0x14          | 0x0F     | 0xF0      | 0x00      | ALARM1\_DATE |
| 299 (12B)        |              | 0xD0            | 0x14          | 0x30     | 0xCF      | 0x04      | ALARM1\_10DATE |
| 300 (12C)        |              | 0xD0            | 0x15          | 0x0F     | 0xF0      | 0x00      | ALARM1\_MONTH |
| 301 (12D)        |              | 0xD0            | 0x15          | 0x10     | 0xEF      | 0x04      | ALARM1\_10MONTH |
| 302 (12E)        |              | 0xD0            | 0x16          | 0x0F     | 0xF0      | 0x00      | ALARM1\_YEAR |
| 303 (12F)        |              | 0xD0            | 0x16          | 0xF0     | 0x0F      | 0x04      | ALARM1\_10YEAR |
| 304 (130)        |              | 0xD0            | 0x17          | 0x0F     | 0xF0      | 0x00      | ALARM1\_100YEAR |
| 305 (131)        |              | 0xD0            | 0x17          | 0xF0     | 0x0F      | 0x04      | ALARM1\_1000YEAR |
| 306 (132)        | ALARM0\_CNTL | 0xD0            | 0x18          | 0xFF     | 0x00      | 0x00      | ALARM0\_CNTL |
| 307 (133)        | ALARM1\_CNTL | 0xD0            | 0x19          | 0xFF     | 0x00      | 0x00      | ALARM1\_CNTL |
| 308 (134)        | RTC\_STATUS  | 0xD0            | 0x1A          | 0x80     | 0x7F      | 0x07      | RTC\_STATUS\_DIV\_OK  |
| 309 (135)        |              | 0xD0            | 0x1A          | 0x40     | 0xBF      | 0x06      | RTC\_STATUS\_LEAP\_OK       |
| 310 (136)        |              | 0xD0            | 0x1A          | 0x20     | 0xDF      | 0x05      | RTC\_STATUS\_MON\_OK |
| 311 (137)        |              | 0xD0            | 0x1A          | 0x10     | 0xEF      | 0x04      | RTC\_STATUS\_CARY\_OK     |
| 312 (138)        |              | 0xD0            | 0x1A          | 0x08     | 0xF7      | 0x03      | RTC\_STATUS\_REG\_OK |
| 313 (139)        |              | 0xD0            | 0x1A          | 0x04     | 0xFB      | 0x02      | RTC\_STATUS\_ALARM0 |
| 314 (13A)        |              | 0xD0            | 0x1A          | 0x02     | 0xFD      | 0x01      | RTC\_STATUS\_ALARM1 |
| 315 (13B)        |              | 0xD0            | 0x1A          | 0x01     | 0xFE      | 0x00      | RTC\_STATUS\_XTAL\_FLT     |
| 316 (13C)        | RTC\_CNTL    | 0xD0            | 0x1B          | 0x20     | 0xDF      | 0x05      | RTC\_CNTL\_ALARM\_WP  |
| 317 (13D)        |              | 0xD0            | 0x1B          | 0x10     | 0xEF      | 0x04      | RTC\_CNTL\_RTC\_WP |
| 318 (13E)        |              | 0xD0            | 0x1B          | 0x08     | 0xF7      | 0x03      | RTC\_CNTL\_nTCLKWBB\_EN |
| 319 (13F)        |              | 0xD0            | 0x1B          | 0x02     | 0xFD      | 0x01      | RTC\_CNTL\_nTCLKAP\_EN |
| 320 (140)        |              | 0xD0            | 0x1B          | 0x01     | 0xFE      | 0x00      | RTC\_CNTL\_nRTC\_EN      |
| 321 (141)        | RTC\_IRQ     | 0xD0            | 0x1C          | 0x08     | 0xF7      | 0x03      | ALARM0\_R  |
| 322 (142)        |              | 0xD0            | 0x1C          | 0x04     | 0xFB      | 0x02      | ALARM1\_R |
| 323 (143)        | RTC\_IRQ\_MASK | 0xD0            | 0x1D          | 0x08     | 0xF7      | 0x03      | ALARM0\_R\_MASK  |
| 324 (144)        |              | 0xD0            | 0x1D          | 0x04     | 0xFB      | 0x02      | ALARM1\_R\_MASK  |
| 325 (145)        | MPL\_CNTL    | 0xD0            | 0x1E          | 0x10     | 0xEF      | 0x04      | EN\_MPL  |
| 326 (146)        |              | 0xD0            | 0x1E          | 0x0C     | 0xF3      | 0x02      | TIME\_MPL  |
| 327 (147)        |              | 0xD0            | 0x1E          | 0x40     | 0xBF      | 0x06      | WTSR\_SMPL\_CNTL\_EN\_WTSR |
| 328 (148)        |              | 0xD0            | 0x1E          | 0x10     | 0xEF      | 0x04      | WTSR\_SMPL\_CNTL\_EN\_SMPL  |
| 329 (149)        |              | 0xD0            | 0x1E          | 0x0C     | 0xF3      | 0x02      | WTSR\_SMPL\_CNTL\_TIME\_SMPL  |
| 330 (14A)        |              | 0xD0            | 0x1E          | 0x03     | 0xFC      | 0x00      | WTSR\_SMPL\_CNTL\_TIME\_WTSR  |
|                  |              |                 |               |          |           |           | T O U C H - S C R E E N / A D C   C O N T R O L L E R |
| 331 (14B)        | TSC\_STA\_INT | 0x8E            | 0x00          | 0x10     | 0xEF      | 0x04      | nREF\_OK |
| 332 (14C)        |              | 0x8E            | 0x00          | 0x08     | 0xF7      | 0x03      | nCONV\_NS |
| 333 (14D)        |              | 0x8E            | 0x00          | 0x04     | 0xFB      | 0x02      | CONV\_S  |
| 334 (14E)        |              | 0x8E            | 0x00          | 0x02     | 0xFD      | 0x01      | nTS\_NS  |
| 335 (14F)        |              | 0x8E            | 0x00          | 0x01     | 0xFE      | 0x00      | nTS\_S   |
| 336 (150)        | TSC\_INT\_MASK | 0x8E            | 0x01          | 0x08     | 0xF7      | 0x03      | nCONV\_NS\_M |
| 337 (151)        |              | 0x8E            | 0x01          | 0x04     | 0xFB      | 0x02      | CONV\_S\_M |
| 338 (152)        |              | 0x8E            | 0x01          | 0x02     | 0xFD      | 0x01      | nTS\_NS\_M |
| 339 (153)        |              | 0x8E            | 0x01          | 0x01     | 0xFE      | 0x00      | nTS\_S\_M |
| 340 (154)        | TSC\_CNFG1   | 0x8E            | 0x02          | 0x80     | 0x7F      | 0x07      | PU\_100\_50 |
| 341 (155)        |              | 0x8E            | 0x02          | 0x10     | 0xEF      | 0x04      | Four\_Wire\_CNFG |
| 342 (156)        |              | 0x8E            | 0x02          | 0x03     | 0xFC      | 0x00      | REF\_CNFG |
| 343 (157)        | TSC\_CNFG2   | 0x8E            | 0x03          | 0x80     | 0x7F      | 0x07      | RES\_X   |
| 344 (158)        |              | 0x8E            | 0x03          | 0x40     | 0xBF      | 0x06      | RES\_Y   |
| 345 (159)        |              | 0x8E            | 0x03          | 0x20     | 0xDF      | 0x05      | RES\_Z1  |
| 346 (15A)        |              | 0x8E            | 0x03          | 0x10     | 0xEF      | 0x04      | RES\_Z2  |
| 347 (15B)        |              | 0x8E            | 0x03          | 0x08     | 0xF7      | 0x03      | AVG-X    |
| 348 (15C)        |              | 0x8E            | 0x03          | 0x04     | 0xFB      | 0x02      | AVG\_Y   |
| 349 (15D)        |              | 0x8E            | 0x03          | 0x02     | 0xFD      | 0x01      | AVG\_Z1  |
| 350 (15E)        |              | 0x8E            | 0x03          | 0x01     | 0xFE      | 0x00      | AVG\_Z2  |
| 351 (15F)        | TSC\_CNFG3   | 0x8E            | 0x04          | 0xC0     | 0x3F      | 0x06      | T\_ACQ\_X |
| 352 (160)        |              | 0x8E            | 0x04          | 0x30     | 0xCF      | 0x04      | T\_ACQ\_Y |
| 353 (161)        |              | 0x8E            | 0x04          | 0x0C     | 0xF3      | 0x02      | T\_ACQ\_Z1 |
| 354 (162)        |              | 0x8E            | 0x04          | 0x03     | 0xFC      | 0x00      | T\_ACQ\_Z2 |
| 355 (163)        | TSC\_CNFG4   | 0x8E            | 0x05          | 0x08     | 0xF7      | 0x03      | D\_CV\_X |
| 356 (164)        |              | 0x8E            | 0x05          | 0x04     | 0xFB      | 0x02      | D\_CV\_Y |
| 357 (165)        |              | 0x8E            | 0x05          | 0x02     | 0xFD      | 0x01      | D\_CV\_Z1 |
| 358 (166)        |              | 0x8E            | 0x05          | 0x01     | 0xFE      | 0x00      | D\_CV-Z2 |
| 359 (167)        | TSC\_RES\_CNFG1 | 0x8E            | 0x06          | 0x80     | 0x7F      | 0x07      | RES\_AUX1 |
| 360 (168)        |              | 0x8E            | 0x06          | 0x40     | 0xBF      | 0x06      | RES\_VBUS |
| 361 (169)        |              | 0x8E            | 0x06          | 0x20     | 0xDF      | 0x05      | RES\_VAC |
| 362 (16A)        |              | 0x8E            | 0x06          | 0x10     | 0xEF      | 0x04      | RES\_MBATT |
| 363 (16B)        |              | 0x8E            | 0x06          | 0x08     | 0xF7      | 0x03      | RES\_BBATT |
| 364 (16C)        |              | 0x8E            | 0x06          | 0x04     | 0xFB      | 0x02      | RES\_ICHG |
| 365 (16D)        |              | 0x8E            | 0x06          | 0x02     | 0xFD      | 0x01      | RES\_TDIE |
| 366 (16E)        |              | 0x8E            | 0x06          | 0x01     | 0xFE      | 0x00      | RES\_AUX2 |
| 367 (16F)        | TSC\_AVG\_CNFG1 | 0x8E            | 0x07          | 0x80     | 0x7F      | 0x07      | AVG\_AUX1 |
| 368 (170)        |              | 0x8E            | 0x07          | 0x40     | 0xBF      | 0x06      | AVG\_VBUS |
| 369 (171)        |              | 0x8E            | 0x07          | 0x20     | 0xDF      | 0x05      | AVG\_VAC |
| 370 (172)        |              | 0x8E            | 0x07          | 0x10     | 0xEF      | 0x04      | AVG\_MBATT |
| 371 (173)        |              | 0x8E            | 0x07          | 0x08     | 0xF7      | 0x03      | AVG\_BBATT |
| 372 (174)        |              | 0x8E            | 0x07          | 0x04     | 0xFB      | 0x02      | AVG\_ICHG |
| 373 (175)        |              | 0x8E            | 0x07          | 0x02     | 0xFD      | 0x01      | AVG\_TDIE |
| 374 (176)        |              | 0x8E            | 0x07          | 0x01     | 0xFE      | 0x00      | AVG\_AUX2 |
| 375 (177)        | TSC\_ACQ\_CNFG1 | 0x8E            | 0x08          | 0xC0     | 0x3F      | 0x06      | T\_ACQ\_AUX1 |
| 376 (178)        |              | 0x8E            | 0x08          | 0x30     | 0xCF      | 0x04      | T\_ACQ\_VBUS |
| 377 (179)        |              | 0x8E            | 0x08          | 0x0C     | 0xF3      | 0x02      | T\_ACQ\_VAC |
| 378 (17A)        |              | 0x8E            | 0x08          | 0x03     | 0xFC      | 0x00      | T\_ACQ\_MBATT |
| 379 (17B)        | TSC\_ACQ\_CNFG2 | 0x8E            | 0x09          | 0xC0     | 0x3F      | 0x06      | T\_ACQ\_BBATT |
| 380 (17C)        |              | 0x8E            | 0x09          | 0x30     | 0xCF      | 0x04      | T\_ACQ\_ICHG |
| 381 (17D)        |              | 0x8E            | 0x09          | 0x0C     | 0xF3      | 0x02      | T\_ACQ\_TDIE |
| 382 (17E)        |              | 0x8E            | 0x09          | 0x03     | 0xFC      | 0x00      | T\_ACQ\_AUX2 |
| 383 (17F)        | TSC\_ACQ\_CNFG3 | 0x8E            | 0x0A          | 0x80     | 0x7F      | 0x07      | D\_CV\_AUX1 |
| 384 (180)        |              | 0x8E            | 0x0A          | 0x40     | 0xBF      | 0x06      | D\_CV\_VBUS |
| 385 (181)        |              | 0x8E            | 0x0A          | 0x20     | 0xDF      | 0x05      | D\_CV\_VAC |
| 386 (182)        |              | 0x8E            | 0x0A          | 0x10     | 0xEF      | 0x04      | D\_CV\_MBATT |
| 387 (183)        |              | 0x8E            | 0x0A          | 0x08     | 0xF7      | 0x03      | D\_CV\_BBATT |
| 388 (184)        |              | 0x8E            | 0x0A          | 0x04     | 0xFB      | 0x02      | D\_CV\_ICHG |
| 389 (185)        |              | 0x8E            | 0x0A          | 0x02     | 0xFD      | 0x01      | D\_CV\_TDIE |
| 390 (186)        |              | 0x8E            | 0x0A          | 0x01     | 0xFE      | 0x00      | D\_CV\_AUX2 |
| 391 (187)        | ADC\_RESULTS | 0x8E            | 0x50          | 0xFF     | 0x00      | 0x00      | X\_MSB   |
| 392 (188)        |              | 0x8E            | 0x51          | 0xF0     | 0x0F      | 0x04      | X\_LSB   |
| 393 (189)        |              | 0x8E            | 0x52          | 0xFF     | 0x00      | 0x00      | Y\_MSB   |
| 394 (18A)        |              | 0x8E            | 0x53          | 0xF0     | 0x0F      | 0x04      | Y\_LSB   |
| 395 (18B)        |              | 0x8E            | 0x54          | 0xFF     | 0x00      | 0x00      | Z1\_MSB  |
| 396 (18C)        |              | 0x8E            | 0x55          | 0xF0     | 0x0F      | 0x04      | Z1\_LSB  |
| 397 (18D)        |              | 0x8E            | 0x56          | 0xFF     | 0x00      | 0x00      | Z2\_MSB  |
| 398 (18E)        |              | 0x8E            | 0x57          | 0xF0     | 0x0F      | 0x04      | Z2\_LSB  |
| 399 (18F)        |              | 0x8E            | 0x60          | 0xFF     | 0x00      | 0x00      | AUX1\_MSB |
| 400 (190)        |              | 0x8E            | 0x61          | 0xF0     | 0x0F      | 0x04      | AUX1\_LSB |
| 401 (191)        |              | 0x8E            | 0x62          | 0xFF     | 0x00      | 0x00      | VBUS\_MSB |
| 402 (192)        |              | 0x8E            | 0x63          | 0xF0     | 0x0F      | 0x04      | VBUS\_LSB |
| 403 (193)        |              | 0x8E            | 0x64          | 0xFF     | 0x00      | 0x00      | VAC\_MSB |
| 404 (194)        |              | 0x8E            | 0x65          | 0xF0     | 0x0F      | 0x04      | VAC\_LSB |
| 405 (195)        |              | 0x8E            | 0x66          | 0xFF     | 0x00      | 0x00      | MBATT\_MSB |
| 406 (196)        |              | 0x8E            | 0x67          | 0xF0     | 0x0F      | 0x04      | MBATT\_LSB |
| 407 (197)        |              | 0x8E            | 0x68          | 0xFF     | 0x00      | 0x00      | BBATT\_MSB |
| 408 (198)        |              | 0x8E            | 0x69          | 0xF0     | 0x0F      | 0x04      | BBATT\_LSB |
| 409 (199)        |              | 0x8E            | 0x6A          | 0xFF     | 0x00      | 0x00      | ICHG\_MSB |
| 410 (19A)        |              | 0x8E            | 0x6B          | 0xF0     | 0x0F      | 0x04      | ICHG\_LSB |
| 411 (19B)        |              | 0x8E            | 0x6C          | 0xFF     | 0x00      | 0x00      | TDIE\_MSB |
| 412 (19C)        |              | 0x8E            | 0x6D          | 0xF0     | 0x0F      | 0x04      | TDIE\_LSB |
| 413 (19D)        |              | 0x8E            | 0x6E          | 0xFF     | 0x00      | 0x00      | AUX2\_MSB |
| 414 (19E)        |              | 0x8E            | 0x6F          | 0xF0     | 0x0F      | 0x04      | AUX2\_LSB |
| 415 (19F)        | TOUCH-SCREEN CONVERSION COMMAND | 0x8E            | 0x80          | 0x07     | 0xF8      | 0x00      | X\_Drive |
| 416 (1A0)        |              | 0x8E            | 0x88          | 0x07     | 0xF8      | 0x00      | X\_Measurement |
| 417 (1A1)        |              | 0x8E            | 0x90          | 0x07     | 0xF8      | 0x00      | Y\_Drive       |
| 418 (1A2)        |              | 0x8E            | 0x98          | 0x07     | 0xF8      | 0x00      | Y\_Measurement |
| 419 (1A3)        |              | 0x8E            | 0xA0          | 0x07     | 0xF8      | 0x00      | Z1\_Drive       |
| 420 (1A4)        |              | 0x8E            | 0xA8          | 0x07     | 0xF8      | 0x00      | Z1\_Measurement |
| 421 (1A5)        |              | 0x8E            | 0xB0          | 0x07     | 0xF8      | 0x00      | Z2\_Drive       |
| 422 (1A6)        |              | 0x8E            | 0xB8          | 0x07     | 0xF8      | 0x00      | Z2\_Measurement |
| 423 (1A7)        |              | 0x8E            | 0xC0          | 0x07     | 0xF8      | 0x00      | AUX1\_Measurement       |
| 424 (1A8)        |              | 0x8E            | 0xC8          | 0x07     | 0xF8      | 0x00      | VBUS\_Measurement |
| 425 (1A9)        |              | 0x8E            | 0xD0          | 0x07     | 0xF8      | 0x00      | VAC\_Measurement       |
| 426 (1AA)        |              | 0x8E            | 0xD8          | 0x07     | 0xF8      | 0x00      | MBATT\_Measurement |
| 427 (1AB)        |              | 0x8E            | 0xE0          | 0x07     | 0xF8      | 0x00      | BBATT\_Measurement       |
| 428 (1AC)        |              | 0x8E            | 0xE8          | 0x07     | 0xF8      | 0x00      | ICHG\_Measurement |
| 429 (1AD)        |              | 0x8E            | 0xF0          | 0x07     | 0xF8      | 0x00      | TDIE\_Measurement       |
| 430 (1AE)        |              | 0x8E            | 0xF8          | 0x07     | 0xF8      | 0x00      | AUX2\_Measurement |
|                  |              |                 |               |          |           |           | A U D I O   S U B S Y S T E M |
| 431 (1AF)        | PGA\_CNTL1   | 0x78            | 0x84          | 0xC0     | 0x3F      | 0x06      | VOICE\_PGA\_CNTL\_P |
| 432 (1B0)        |              | 0x78            | 0x84          | 0x30     | 0xCF      | 0x04      | VOICE\_PGA\_CNTL\_N |
| 433 (1B1)        |              | 0x78            | 0x84          | 0x08     | 0xF7      | 0x03      | VOICE\_IN\_CONFIG |
| 434 (1B2)        |              | 0x78            | 0x84          | 0x03     | 0xFC      | 0x00      | IN1\_PGA\_CNTL |
| 435 (1B3)        | PGA\_CNTL2   | 0x78            | 0x85          | 0xC0     | 0x3F      | 0x06      | IN2\_PGA\_CNTL |
| 436 (1B4)        |              | 0x78            | 0x85          | 0x30     | 0xCF      | 0x04      | IN3\_PGA\_CNTL |
| 437 (1B5)        |              | 0x78            | 0x85          | 0x0A     | 0xF5      | 0x01      | IN4\_PGA\_CNTL |
| 438 (1B6)        |              | 0x78            | 0x85          | 0x01     | 0xFE      | 0x00      | ZDC      |
| 439 (1B7)        | LMIX\_CNTL   | 0x78            | 0x86          | 0x20     | 0xDF      | 0x05      | VOICE\_IN\_P\_LMIX |
| 440 (1B8)        |              | 0x78            | 0x86          | 0x10     | 0xEF      | 0x04      | VOICE\_IN\_N\_LMIX |
| 441 (1B9)        |              | 0x78            | 0x86          | 0x08     | 0xF7      | 0x03      | IN1\_LMIX |
| 442 (1BA)        |              | 0x78            | 0x86          | 0x04     | 0xFB      | 0x02      | IN2\_LMIX |
| 443 (1BB)        |              | 0x78            | 0x86          | 0x02     | 0xFD      | 0x01      | IN3\_LMIX |
| 444 (1BC)        |              | 0x78            | 0x86          | 0x01     | 0xFE      | 0x00      | IN4\_LMIX |
| 445 (1BD)        | RMIX\_CNTL   | 0x78            | 0x87          | 0x20     | 0xDF      | 0x05      | VOICE\_IN\_P\_RMIX |
| 446 (1BE)        |              | 0x78            | 0x87          | 0x10     | 0xEF      | 0x04      | VOICE\_IN\_N\_RMIX |
| 447 (1BF)        |              | 0x78            | 0x87          | 0x08     | 0xF7      | 0x03      | IN1\_RMIX |
| 448 (1C0)        |              | 0x78            | 0x87          | 0x04     | 0xFB      | 0x02      | IN2\_RMIX |
| 449 (1C1)        |              | 0x78            | 0x87          | 0x02     | 0xFD      | 0x01      | IN3\_RMIX |
| 450 (1C2)        |              | 0x78            | 0x87          | 0x01     | 0xFE      | 0x00      | IN4\_RMIX |
| 451 (1C3)        | MMIX\_CNTL   | 0x78            | 0x88          | 0x03     | 0xFC      | 0x00      | MONO\_MIX\_CNTL |
| 452 (1C4)        | HS\_RIGHT\_GAIN\_CNTL | 0x78            | 0x89          | 0x1F     | 0xE0      | 0x00      | RIGHT\_HS\_GAIN |
| 453 (1C5)        | HS\_LEFT\_GAIN\_CNTL | 0x78            | 0x8A          | 0x1F     | 0xE0      | 0x00      | LEFT\_HS\_GAIN |
| 454 (1C6)        | LINE\_OUT\_GAIN\_CNTL | 0x78            | 0x8B          | 0x1F     | 0xE0      | 0x00      | LINE\_OUT\_GAIN |
| 455 (1C7)        | LS\_GAIN\_CNTL | 0x78            | 0x8C          | 0x1F     | 0xE0      | 0x00      | LS\_GAIN |
| 456 (1C8)        | AUDIO\_CNTL  | 0x78            | 0x8D          | 0x80     | 0x7F      | 0x07      | MUTE     |
| 457 (1C9)        |              | 0x78            | 0x8D          | 0x40     | 0xBF      | 0x06      | AUDIO\_SHDN |
|                  | //           | 0x78            | 0x8D          | 0x20     | 0xDF      | 0x05      | LS\_BP\_EN |
| 458 (1CA)        |              | 0x78            | 0x8D          | 0x10     | 0xEF      | 0x04      | AMP\_EN\_CNTL |
| 459 (1CB)        |              | 0x78            | 0x8D          | 0x0C     | 0xF3      | 0x02      | CLASS\_D\_OSC\_CNTL |
| 460 (1CC)        |              | 0x78            | 0x8D          | 0x02     | 0xFD      | 0x01      | HS\_MONO\_SW |
| 461 (1CD)        | AUDIO\_ENABLE1 | 0x78            | 0x8E          | 0x20     | 0xDF      | 0x05      | LS\_BP\_EN |
| 462 (1CE)        |              | 0x78            | 0x8E          | 0x08     | 0xF7      | 0x03      | LS\_AMP\_EN |
| 463 (1CF)        |              | 0x78            | 0x8E          | 0x04     | 0xFB      | 0x02      | LS\_LINEOUT\_EN |
| 464 (1D0)        |              | 0x78            | 0x8E          | 0x03     | 0xFC      | 0x00      | HS\_EN   |
|                  |              |                 |               |          |           |           | C H I P   I D E N T I F I C A T I O N |
| 465 (1D1)        | II1RR        | 0x68            | 0x8E          | 0xFF     | 0x00      | 0x00      | IIR1     |
| 466 (1D2)        | II2RR        | 0x68            | 0x8F          | 0xFF     | 0x00      | 0x00      | IIR2     |
|                  |              |                 |               |          |           |           | I N T E R R U P T   &   S T A T U S |
| 467 (1D3)        | IRQ\_STAT    | 0x78            | 0x98          | 0x02     | 0xFD      | 0x01      | SFT\_nTIRQ |
| 468 (1D4)        |              | 0x78            | 0x98          | 0x01     | 0xFE      | 0x00      |  SFT\_nIRQ |