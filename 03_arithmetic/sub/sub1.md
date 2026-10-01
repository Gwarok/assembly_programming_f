| Flag | Status | Why
| CF   | 1      | 50 is smaller than 80, so unsigned subtraction requires a borrow
| ZF   | 0      | The result is 'E2', not zero
| SF   | 1      | The most significant bit of 'E2' is '1'
| OF   | 1      | Signed '50 - (-80)' would be '130', outside the signed 8-bit range
| AF   | 0      | No borrow occurs from bit 4
| PF   | 1      | 'E2 = 11100010' contains four 1's, which is even parity