# Integer Overflow in Assembly Memory Access

This repository demonstrates a common but subtle error in assembly programming: integer overflow during memory address calculation.  The code attempts to access memory at an address calculated using EBX, ECX, and a constant offset.  If the calculation exceeds the maximum representable value in the registers, an integer overflow occurs, leading to unpredictable results.

The `bug.asm` file contains the buggy code.  The `bugSolution.asm` file presents a corrected version that mitigates the risk of overflow.

This example highlights the importance of careful consideration of potential integer overflow in low-level programming, especially when working with memory addresses.