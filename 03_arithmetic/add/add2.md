| Flag | Status | Why 
| CF   | 0      | There is no carry beyond bit 15. 32500 fits in unsigned 16-bit range `0-65535`. 
| ZF   | 0      | `7EF4` is not zero. |
| SF   | 0      | Bit 15 is `0`, so the result is positive when interpreted as signed. 
| OF   | 0      | `32000 + 500 = 32500`, which is still within signed 16-bit range `-32768 to +32767`. 
| AF   | 0      | The low nibbles are `0 + 4`, producing no carry from bit 3 to bit 4. 
| PF   | 0      | The low byte is `F4 = 11110100`, which has **five 1s**, an odd number. 