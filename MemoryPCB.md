# Main connector #

| **Pin (odd)** | **Signal**       | **Pin (even)** | **Signal**     |
|:--------------|:-----------------|:---------------|:---------------|
| 1             | GND              | 2              | GND            |
| 3             | KeyRow\_0        | 2              | KeyCol\_2      |
| 5             | T-FLASH\_D2      | 6              | T-FLASH\_D3    |
| 7             | T-FLASH\_CMD     | 8              | V\_T-FLASH (3V)     |
| 9             | T-FLASH\_CLK     | 10             | T-FLASH\_D0    |
| 11            | T-FLASH\_D1      | 12             | T-FLASH\_Detect |
| 13            | ACC\_INT         | 14             | V-BAT          |
| 15            | GND              | 16             | V-BAT          |
| 17            | CAM-FL\_SET      | 18             | V-BAT          |
| 19            | CAM-FL\_EN       | 20             | NAND\_D0       |
| 21            | NAND\_D1         | 22             | NAND\_D2       |
| 23            | NAND\_D3         | 24             | NAND\_CLK      |
| 25            | NAND\_CMD        | 26             | T-FLASH\_EN    |
| 27            | SIM\_CLK         | 28             | SIM\_RESET     |
| 29            | V\_SIM (3V)      | 30             | SIM\_DAT       |
| 31            | AP-SDA (3V)      | 32             | SP-SCL (3V)    |
| 33            | MSense\_IRQ      | 34             | MSense\_RESET  |
| 35            | V\_PDA (3V)      | 36             | KeyRow\_2      |
| 37            | KeyCol\_1        | 38             | KeyRow\_1      |
| 39            | GND              | 40             | GND            |

# MIC5365-3.0YMT #
Micrel 3.0V 150mA Low DropOut voltager regulator (LDO) [Datasheet](http://www.micrel.com/_PDF/mic5365.pdf).

| **Pin** | **Function** | **Signal on PCB** |
|:--------|:-------------|:------------------|
| 1       | VOUT         | V-MICREL (3V)     |
| 2       | GND          | GND               |
| 3       | EN           | T-FLASH\_EN       |
| 4       | VIN          | V-BAT             |

# SD-Card connector #

| **Pin** | **Function** | **Signal on PCB** |
|:--------|:-------------|:------------------|
| Card detect SW A |              | GND               |
| Card detect SW B |              | T-FLASH\_Detect   |
| 1       | D2           | T-FLASH\_D2       |
| 2       | D3           | T-FLASH\_D3       |
| 3       | CMD          | T-FLASH\_CMD      |
| 4       | VCC          | V-MICREL (3V)     |
| 5       | CLK          | T-FLASH\_CLK      |
| 6       | GND          | GND               |
| 7       | D0           | T-FLASH\_D0       |
| 8       | D1           | T-FLASH\_D1       |

# Lock button #

| **Pin** | **Function** | **Signal on PCB** |
|:--------|:-------------|:------------------|
| 1       | Push-button (default open) | KeyRow\_0         |
| 2       | Push-button         | KeyCol\_2         |
| 3       | GND          | GND               |

# Up/down buttons #

| **Pin** | **Function** | **Signal on PCB** |
|:--------|:-------------|:------------------|
| 1       | Push-button DOWN (default open) | KeyRow\_1         |
| 2       | Push-button DOWN + UP          | KeyCol\_1         |
| 3       | Push-button UP (default open)   | KeyRow\_2         |
| 4       | GND          | GND               |