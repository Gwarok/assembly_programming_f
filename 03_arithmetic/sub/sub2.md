| Flag | Status | Why 
| CF   | 1      | 1000 is less than 2000, so unsigned subtraction requires a borrow
| ZF   | 0      | The result is not zero
| SF   | 1      | Bit 15 is '1', indicating a negative signed result
| OF   | 0      | '1000 - 2000 = -1000', and -1000 is within the signed 16-bit range
| AF   | 0      | The lower nibbles are '0 - 0', there is no borrow between bits 3 and 4
| PF   | 1      | The low byte '18 = 00011000' contains two 1s, giving even parity