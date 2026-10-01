| Flag   | Status      | Why 
| CF     | 0 (cleared) | There is no carry beyond bit 7. The result 130 fits in 8 unsigned bits. 
| ZF     | 0 (cleared) | The result `10000010` is not zero. 
| SF     | 1 (set)     | The most significant bit is `1`. 
| OF     | 1 (set)     | Two positive signed numbers were added, but the result `130` is greater than the signed maximum `127`. 
| AF     | 1 (set)     | The lower nibbles are `1000 + 1010`, which produces a carry from bit 3 to bit 4. 
| PF     | 1 (set)     | `10000010` contains **two 1s**, which is even parity. 