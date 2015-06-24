# Function to power net mapping #

| **Function** | **Power net** | **Power source** | **Controlled by** |
|:-------------|:--------------|:-----------------|:------------------|
| T-Flash      | V-MICREL\_3.0V | MIC5365-3.0YMT   | T-FLASH\_EN ( GPG(6) ) |
| Int. Flash   | VTF\_3.0V     | PMU - PMIC200 (OUTCARD1) | PWR\_I2C          |
| FM Radio     | FM\_RADIO\_3.0V | U202 (VOUT1)     | PS\_VOUT\_30 ???  |
| ???          | VALS\_3.0V     | U202 (VOUT2)     | PS\_VOUT\_30 ???  |
| BT WIFI      | V\_BAT         | Battery          | BT/WIFI has integrated volatge regulators |
| BT\_WIFI     | VCC\_3.0V\_PDA  | PMU - PMIC200 (OUTCARD2) | PWR\_I2C          |