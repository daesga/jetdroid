# Driver #
See [MAX8906driver](MAX8906driver.md).

# Registers (Look up table 1) #

See [MAX8906RegDetails](MAX8906RegDetails.md) for Look up table 2.

| **Index (Hex)** | **Function** | **Slave addr** | **Reg addr** | **Reg name** |
|:----------------|:-------------|:---------------|:-------------|:-------------|
| 0 (0)           | Battery chargers | 0x78           | 0x7C         | REG\_CHG\_CNTL1 |
| 1 (1)           |              | 0x78           | 0x7D         | REG\_CHG\_CNTL2 |
| 2 (2)           |              | 0x78           | 0x7E         | REG\_CHG\_IRQ1 |
| 3 (3)           |              | 0x78           | 0x7F         | REG\_CHG\_IRQ2 |
| 4 (4)           |              | 0x78           | 0x80         | REG\_CHG\_IRQ1\_MASK |
| 5 (5)           |              | 0x78           | 0x81         | REG\_CHG\_IRQ2\_MASK |
| 6 (6)           |              | 0x78           | 0x82         | REG\_CHG\_STAT |
| 7 (7)           |              | 0x78           | 0x78         | REG\_BBATTCNFG |
| 8 (8)           | Step-down regulators | 0x78           | 0x5C         | REG\_WBBCOREEN |
| 9 (9)           |              | 0x78           | 0x5D         | REG\_WBBCOREFSEQ |
| 10 (A)          |              | 0x78           | 0x5E         | REG\_WBBCORETV |
| 11 (B)          |              | 0x78           | 0x9C         | REG\_WBBRFEN |
| 12 (C)          |              | 0x78           | 0x9D         | REG\_WBBRFFSEQ |
| 13 (D)          |              | 0x78           | 0x9E         | REG\_WBBRFTV |
| 14 (E)          |              | 0x78           | 0x04         | REG\_APPSEN  |
| 15 (F)          |              | 0x68           | 0x10         | REG\_OVER1   |
| 16 (10)         |              | 0x78           | 0x05         | REG\_APPSFSEQ |
| 17 (11)         |              | 0x68           | 0x23         | REG\_ADTV1   |
| 18 (12)         |              | 0x68           | 0x24         | REG\_ADTV2   |
| 19 (13)         |              | 0x78           | 0x06         | REG\_APPSCLG |
| 20 (14)         |              | 0x68           | 0x20         | REG\_VCC1    |
| 21 (15)         |              | 0x78           | 0x08         | REG\_IOEN    |
| 22 (16)         |              | 0x78           | 0x09         | REG\_IOFSEQ  |
| 23 (17)         |              | 0x78           | 0x0C         | REG\_MEMEN   |
| 24 (18)         |              | 0x78           | 0x0D         | REG\_MEMFSEQ |
| 25 (19)         | Linear regulators| 0x78           | 0x10         | REG\_WBBMEMEN |
| 26 (1A)         |              | 0x78           | 0x11         | REG\_WBBMEMFSEQ |
| 27 (1B)         |              | 0x78           | 0x12         | REG\_WBBMEMTV |
| 28 (1C)         |              | 0x78           | 0x14         | REG\_WBBIOEN |
| 29 (1D)         |              | 0x78           | 0x15         | REG\_WBBIOFSEQ |
| 30 (1E)         |              | 0x78           | 0x16         | REG\_WBBIOTV |
| 31 (1F)         |              | 0x78           | 0x18         | REG\_WBBANAEN |
| 32 (20)         |              | 0x78           | 0x19         | REG\_WBBANAFSEQ |
| 33 (21)         |              | 0x78           | 0x1A         | REG\_WBBANATV |
| 34 (22)         |              | 0x78           | 0x1C         | REG\_RFRXLEN |
| 35 (23)         |              | 0x78           | 0x1D         | REG\_RFRXLFSEQ |
| 36 (24)         |              | 0x78           | 0x1E         | REG\_RFRXLTV |
| 37 (25)         |              | 0x78           | 0x20         | REG\_RFTXLEN |
| 38 (26)         |              | 0x78           | 0x21         | REG\_RFTXLFSEQ |
| 39 (27)         |              | 0x78           | 0x22         | REG\_RFTXLTV |
| 40 (28)         |              | 0x78           | 0x24         | REG\_RFRXHEN |
| 41 (29)         |              | 0x78           | 0x25         | REG\_RFRXHFSEQ |
| 42 (2A)         |              | 0x78           | 0x26         | REG\_RFRXHTV |
| 43 (2B)         |              | 0x78           | 0x28         | REG\_RFTCXOEN |
| 44 (2C)         |              | 0x78           | 0x29         | REG\_RFTCXOFSEQ |
| 45 (2D)         |              | 0x78           | 0x2A         | REG\_RFTCXOTV |
| 46 (2E)         |              | 0x78           | 0x2C         | REG\_LDOAEN  |
| 47 (2F)         |              | 0x78           | 0x2D         | REG\_LDOAFSEQ |
| 48 (30)         |              | 0x78           | 0x2E         | REG\_LDOATV  |
| 49 (31)         |              | 0x78           | 0x30         | REG\_LDOBEN  |
| 50 (32)         |              | 0x78           | 0x31         | REG\_LDOBFSEQ |
| 51 (33)         |              | 0x78           | 0x32         | REG\_LDOBTV  |
| 52 (34)         |              | 0x78           | 0x34         | REG\_LDOCEN  |
| 53 (35)         |              | 0x78           | 0x35         | REG\_LDOCFSEQ |
| 54 (36)         |              | 0x78           | 0x36         | REG\_LDOCTV  |
| 55 (37)         |              | 0x78           | 0x38         | REG\_LDODEN  |
| 56 (38)         |              | 0x78           | 0x39         | REG\_LDODFSEQ |
| 57 (39)         |              | 0x78           | 0x3A         | REG\_LDODTV  |
| 58 (3A)         |              | 0x78           | 0x3C         | REG\_SIMLTEN |
| 59 (3B)         |              | 0x78           | 0x3D         | REG\_SIMLTFSEQ |
| 60 (3C)         |              | 0x78           | 0x3E         | REG\_SIMLTTV |
| 61 (3D)         |              | 0x78           | 0x40         | REG\_SRAMEN  |
| 62 (3E)         |              | 0x78           | 0x41         | REG\_SRAMFSEQ |
| 63 (3F)         |              | 0x68           | 0x29         | REG\_SDTV1   |
| 64 (40)         |              | 0x68           | 0x2A         | REG\_SDTV2   |
| 65 (41)         |              | 0x78           | 0x42         | REG\_SRAMCLG |
| 66 (42)         |              | 0x78           | 0x44         | REG\_CARD1EN |
| 67 (43)         |              | 0x78           | 0x45         | REG\_CARD1FSEQ |
| 68 (44)         |              | 0x78           | 0x46         | REG\_CARD1TV |
| 69 (45)         |              | 0x78           | 0x48         | REG\_CARD2EN |
| 70 (46)         |              | 0x78           | 0x49         | REG\_CARD2FSEQ |
| 71 (47)         |              | 0x78           | 0x4A         | REG\_CARD2TV |
| 72 (48)         |              | 0x78           | 0x4C         | REG\_MVTENEN |
| 73 (49)         |              | 0x78           | 0x4D         | REG\_MVTFSEQ |
| 74 (4A)         |              | 0x68           | 0x32         | REG\_MDTV1   |
| 75 (4B)         |              | 0x68           | 0x33         | REG\_MDTV2   |
| 76 (4C)         |              | 0x78           | 0x50         | REG\_BIASEN  |
| 77 (4D)         |              | 0x78           | 0x51         | REG\_BIASFSEQ |
| 78 (4E)         |              | 0x78           | 0x52         | REG\_BIASTV  |
| 79 (4F)         |              | 0x78           | 0x54         | REG\_VBUSEN  |
| 80 (50)         |              | 0x78           | 0x55         | REG\_VBUSFSEQ |
| 81 (51)         |              | 0x78           | 0x58         | REG\_USBTXRXEN |
| 82 (52)         |              | 0x78           | 0x59         | REG\_USBTXRXFSEQ |
| 83 (53)         | Main-battery fault detector | 0x78           | 0x60         | REG\_LBCNFG  |
| 84 (54)         | On/off controller | 0x78           | 0x00         | REG\_EXTWKSEL |
| 85 (55)         |              | 0x78           | 0x01         | REG\_ON\_OFF\_IRQ |
| 86 (56)         |              | 0x78           | 0x02         | REG\_ON\_OFF\_IRQ\_MASK |
| 87 (57)         |              | 0x78           | 0x03         | REG\_ON\_OFF\_STAT |
| 88 (58)         | Flexible power sequencer | 0x78           | 0x64         | REG\_SEQ1CNFG |
| 89 (59)         |              | 0x78           | 0x65         | REG\_SEQ2CNFG |
| 90 (5A)         |              | 0x78           | 0x66         | REG\_SEQ3CNFG |
| 91 (5B)         |              | 0x78           | 0x67         | REG\_SEQ4CNFG |
| 92 (5C)         |              | 0x78           | 0x68         | REG\_SEQ5CNFG |
| 93 (5D)         |              | 0x78           | 0x69         | REG\_SEQ6CNFG |
| 94 (5E)         |              | 0x78           | 0x6A         | REG\_SEQ7CNFG |
| 95 (5F)         | USB transceiver | 0x78           | 0x6C         | REG\_USBCNFG |
| 96 (60)         | TCX buffer   | 0x78           | 0x74         | REG\_TCXOCNFG |
| 97 (61)         | Reference output (REFOUT) | 0x78           | 0x70         | REG\_REFOUTCNFG |
| 98 (62)         | Realtime clock (RTC) | 0xD0           | 0x00         | REG\_RTC\_SEC |
| 99 (63)         |              | 0xD0           | 0x01         | REG\_RTC\_MIN |
| 100 (64)        |              | 0xD0           | 0x02         | REG\_RTC\_HOURS |
| 101 (65)        |              | 0xD0           | 0x03         | REG\_RTC\_WEEKDAY |
| 102 (66)        |              | 0xD0           | 0x04         | REG\_RTC\_DATE |
| 103 (67)        |              | 0xD0           | 0x05         | REG\_RTC\_MONTH |
| 104 (68)        |              | 0xD0           | 0x06         | REG\_RTC\_YEAR1 |
| 105 (69)        |              | 0xD0           | 0x07         | REG\_RTC\_YEAR2 |
| 106 (6A)        |              | 0xD0           | 0x08         | REG\_ALARM0\_SEC |
| 107 (6B)        |              | 0xD0           | 0x09         | REG\_ALARM0\_MIN |
| 108 (6C)        |              | 0xD0           | 0x0A         | REG\_ALARM0\_HOURS |
| 109 (6D)        |              | 0xD0           | 0x0B         | REG\_ALARM0\_WEEKDAY |
| 110 (6E)        |              | 0xD0           | 0x0C         | REG\_ALARM0\_DATE |
| 111 (6F)        |              | 0xD0           | 0x0D         | REG\_ALARM0\_MONTH |
| 112 (70)        |              | 0xD0           | 0x0E         | REG\_ALARM0\_YEAR1 |
| 113 (71)        |              | 0xD0           | 0x0F         | REG\_ALARM0\_YEAR2 |
| 114 (72)        |              | 0xD0           | 0x10         | REG\_ALARM1\_SEC |
| 115 (73)        |              | 0xD0           | 0x11         | REG\_ALARM1\_MIN |
| 116 (74)        |              | 0xD0           | 0x12         | REG\_ALARM1\_HOURS |
| 117 (75)        |              | 0xD0           | 0x13         | REG\_ALARM1\_WEEKDAY |
| 118 (76)        |              | 0xD0           | 0x14         | REG\_ALARM1\_DATE |
| 119 (77)        |              | 0xD0           | 0x15         | REG\_ALARM1\_MONTH |
| 120 (78)        |              | 0xD0           | 0x16         | REG\_ALARM1\_YEAR1 |
| 121 (79)        |              | 0xD0           | 0x17         | REG\_ALARM1\_YEAR2 |
| 122 (7A)        |              | 0xD0           | 0x18         | REG\_ALARM0\_CNTL |
| 123 (7B)        |              | 0xD0           | 0x19         | REG\_ALARM1\_CNTL |
| 124 (7C)        |              | 0xD0           | 0x1A         | REG\_RTC\_STATUS |
| 125 (7D)        |              | 0xD0           | 0x1B         | REG\_RTC\_CNTL |
| 126 (7E)        |              | 0xD0           | 0x1C         | REG\_RTC\_IRQ |
| 127 (7F)        |              | 0xD0           | 0x1D         | REG\_RTC\_IRQ\_MASK |
| 128 (80)        |              | 0xD0           | 0x1E         | REG\_MPL\_CNTL |
| 129 (81)        | Touch-screen/ADC controller | 0x8E           | 0x00         | REG\_TSC\_STA\_INT |
| 130 (82)        |              | 0x8E           | 0x01         | REG\_TSC\_INT\_MASK |
| 131 (83)        |              | 0x8E           | 0x02         | REG\_TSC\_CNFG1 |
| 132 (84)        |              | 0x8E           | 0x03         | REG\_TSC\_CNFG2 |
| 133 (85)        |              | 0x8E           | 0x04         | REG\_TSC\_CNFG3 |
| 134 (86)        |              | 0x8E           | 0x05         | REG\_TSC\_CNFG4 |
| 135 (87)        |              | 0x8E           | 0x06         | REG\_TSC\_RES\_CNFG1 |
| 136 (88)        |              | 0x8E           | 0x07         | REG\_TSC\_AVG\_CNFG1 |
| 137 (89)        |              | 0x8E           | 0x08         | REG\_TSC\_ACQ\_CNFG1 |
| 138 (8A)        |              | 0x8E           | 0x09         | REG\_TSC\_ACQ\_CNFG2 |
| 139 (8B)        |              | 0x8E           | 0x0A         | REG\_TSC\_ACQ\_CNFG3 |
| 140 (8C)        | ADC results  | 0x8E           | 0x50         | REG\_ADC\_X\_MSB |
| 141 (8D)        |              | 0x8E           | 0x51         | REG\_ADC\_X\_LSB |
| 142 (8E)        |              | 0x8E           | 0x52         | REG\_ADC\_Y\_MSB |
| 143 (8F)        |              | 0x8E           | 0x53         | REG\_ADC\_Y\_LSB |
| 144 (90)        |              | 0x8E           | 0x54         | REG\_ADC\_Z1\_MSB |
| 145 (91)        |              | 0x8E           | 0x55         | REG\_ADC\_Z1\_LSB |
| 146 (92)        |              | 0x8E           | 0x56         | REG\_ADC\_Z2\_MSB |
| 147 (93)        |              | 0x8E           | 0x57         | REG\_ADC\_Z2\_LSB |
| 148 (94)        |              | 0x8E           | 0x60         | REG\_ADC\_AUX1\_MSB |
| 149 (95)        |              | 0x8E           | 0x61         | REG\_ADC\_AUX1\_LSB |
| 150 (96)        |              | 0x8E           | 0x62         | REG\_ADC\_VBUS\_MSB |
| 151 (97)        |              | 0x8E           | 0x63         | REG\_ADC\_VBUS\_LSB |
| 152 (98)        |              | 0x8E           | 0x64         | REG\_ADC\_VAC\_MSB |
| 153 (99)        |              | 0x8E           | 0x65         | REG\_ADC\_VAC\_LSB |
| 154 (9A)        |              | 0x8E           | 0x66         | REG\_ADC\_MBATT\_MSB |
| 155 (9B)        |              | 0x8E           | 0x67         | REG\_ADC\_MBATT\_LSB |
| 156 (9C)        |              | 0x8E           | 0x68         | REG\_ADC\_BBATT\_MSB |
| 157 (9D)        |              | 0x8E           | 0x69         | REG\_ADC\_BBATT\_LSB |
| 158 (9E)        |              | 0x8E           | 0x6A         | REG\_ADC\_ICHG\_MSB |
| 159 (9F)        |              | 0x8E           | 0x6B         | REG\_ADC\_ICHG\_LSB |
| 160 (A0)        |              | 0x8E           | 0x6C         | REG\_ADC\_TDIE\_MSB |
| 161 (A1)        |              | 0x8E           | 0x6D         | REG\_ADC\_TDIE\_LSB |
| 162 (A2)        |              | 0x8E           | 0x6E         | REG\_ADC\_AUX2\_MSB |
| 163 (A3)        |              | 0x8E           | 0x6F         | REG\_ADC\_AUX2\_LSB |
| 164 (A4)        | Touch-screen conversion command | 0x8E           | 0x80         | REG\_TSC\_X\_Drive |
| 165 (A5)        |              | 0x8E           | 0x88         | REG\_TSC\_X\_Measurement |
| 166 (A6)        |              | 0x8E           | 0x90         | REG\_TSC\_Y\_Drive |
| 167 (A7)        |              | 0x8E           | 0x98         | REG\_TSC\_Y\_Measurement |
| 168 (A8)        |              | 0x8E           | 0xA0         | REG\_TSC\_Z1\_Drive |
| 169 (A9)        |              | 0x8E           | 0xA8         | REG\_TSC\_Z1\_Measurement |
| 170 (AA)        |              | 0x8E           | 0xB0         | REG\_TSC\_Z2\_Drive |
| 171 (AB)        |              | 0x8E           | 0xB8         | REG\_TSC\_Z2\_Measurement |
| 172 (AC)        |              | 0x8E           | 0xC0         | REG\_TSC\_AUX1\_Measurement |
| 173 (AD)        |              | 0x8E           | 0xC8         | REG\_TSC\_VBUS\_Measurement |
| 174 (AE)        |              | 0x8E           | 0xD0         | REG\_TSC\_VAC\_Measurement |
| 175 (AF)        |              | 0x8E           | 0xD8         | REG\_TSC\_MBATT\_Measurement |
| 176 (B0)        |              | 0x8E           | 0xE0         | REG\_TSC\_BBATT\_Measurement |
| 177 (B1)        |              | 0x8E           | 0xE8         | REG\_TSC\_ICHG\_Measurement |
| 178 (B2)        |              | 0x8E           | 0xF0         | REG\_TSC\_TDIE\_Measurement |
| 179 (B3)        |              | 0x8E           | 0xF8         | REG\_TSC\_AUX2\_Measurement |
| 180 (B4)        | Audio subsystem | 0x78           | 0x84         | REG\_PGA\_CNTL1 |
| 181 (B5)        |              | 0x78           | 0x85         | REG\_PGA\_CNTL2 |
| 182 (B6)        |              | 0x78           | 0x86         | REG\_LMIX\_CNTL |
| 183 (B7)        |              | 0x78           | 0x87         | REG\_RMIX\_CNTL |
| 184 (B8)        |              | 0x78           | 0x88         | REG\_MMIX\_CNTL |
| 185 (B9)        |              | 0x78           | 0x89         | REG\_HS\_RIGHT\_GAIN\_CNTL |
| 186 (BA)        |              | 0x78           | 0x8A         | REG\_HS\_LEFT\_GAIN\_CNTL |
| 187 (BB)        |              | 0x78           | 0x8B         | REG\_LINE\_OUT\_GAIN\_CNTL |
| 188 (BC)        |              | 0x78           | 0x8C         | REG\_LS\_GAIN\_CNTL |
| 189 (BD)        |              | 0x78           | 0x8D         | REG\_AUDIO\_CNTL |
| 190 (BE)        |              | 0x78           | 0x8E         | REG\_AUDIO\_ENABLE1 |
| 191 (BF)        | Chip identification | 0x68           | 0x8E         | REG\_II1RR   |
| 192 (C0)        |              | 0x68           | 0x8F         | REG\_II2RR   |
| 193 (C1)        |              | 0x78           | 0x98         | REG\_IRQ\_STAT |