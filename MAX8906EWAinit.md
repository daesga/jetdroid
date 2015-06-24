# Observations #

| Register | Content (initial) | after BBinit | After trial write | Comment / Voltage |
|:---------|:------------------|:-------------|:------------------|:------------------|
| LDOAEN (0x2c)     | 0x0f              | 0x0f         | 0x0f              |VLCD\_3.1V         |
| LDOAFSEQ  (0x2d)  | 0x20              | 0x20         | 0x20              |                   |
| LDOATV (0x2e)     | 0x2e              | 0x2e         | 0x2e              |                   |
| SIMLTEN (0x3c)    | 0x0e              | 0x0a         | 0x0b              | VREG\_USIM\_3.0V  |
| SIMLTFSEQ (0x3d)  | 0x00              | 0x00         | 0x00              |                   |
| SIMLTTV (0x3e)    | 0x15              | 0x15         | 0x15              |                   |
| CARD1EN (0x44)    | 0x0f              | 0x0f         | 0x0b              | VTF\_3.0V         |
| CARD1FSEQ (0x45)  | 0x20              | 0x20         | 0x20              |                   |
| CARD1TV (0x46)    | 0x2d              | 0x2d         | 0x2d              |                   |

| Register | Content | EN | SRC | Supply |
|:---------|:--------|:---|:----|:-------|
| SIMLTEN (0x3c) | 0x00    | 0  | 0   | ON     |
|          | 0x01    | 1  | 0   | ON     |
|          | 0x02    | 0  | 1   | ON     |
|          | 0x03    | 1  | 1   | ON     |
|          | 0x04    | 0  | 2   | ON     |
|          | 0x05    | 1  | 2   | ON     |
|          | 0x06    | 0  | 3   | ON     |
|          | 0x07    | 1  | 3   | ON     |
|          | 0x08    | 0  | 4   | OFF    |
|          | 0x09    | 1  | 4   | OFF    |
|          | 0x0a    | 0  | 5   | OFF    |
|          | 0x0b    | 1  | 5   | OFF    |
|          | 0x0c    | 0  | 6   | OFF    |
|          | 0x0d    | 1  | 6   | OFF    |
|          | 0x0e    | 0  | 7   | OFF    |
|          | 0x0f    | 1  | 7   | ON     |
| CARD1EN (0x44) | 0x00    | 0  | 0   | OFF    |
|          | 0x01    | 1  | 0   | OFF    |
|          | 0x02    | 0  | 1   | OFF    |
|          | 0x03    | 1  | 1   | OFF    |
|          | 0x04    | 0  | 2   | OFF    |
|          | 0x05    | 1  | 2   | OFF    |
|          | 0x06    | 0  | 3   | OFF    |
|          | 0x07    | 1  | 3   | OFF    |
|          | 0x08    | 0  | 4   | OFF    |
|          | 0x09    | 1  | 4   | OFF    |
|          | 0x0a    | 0  | 5   | OFF    |
|          | 0x0b    | 1  | 5   | OFF    |
|          | 0x0c    | 0  | 6   | OFF    |
|          | 0x0d    | 1  | 6   | OFF    |
|          | 0x0e    | 0  | 7   | OFF    |
|          | 0x0f    | 1  | 7   | OFF    |