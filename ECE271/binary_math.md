### **Binary Math Glossary:**

---

### **General Concepts:**
- **Bit (Binary Digit):**  
  The smallest unit of data in computing, represented as either `0` or `1`.

- **Nibble:**  
  A group of 4 bits. Example: `1101`

- **Byte:**  
  A group of 8 bits. Example: `10101100`

- **Word:**  
  A fixed-length group of bits (commonly 16, 32, or 64 bits).

---

### **Number Representations:**
- **Unsigned Binary:**  
  A binary number representing only non-negative values.  
  Example: `00011010` = 26 (decimal)

- **Signed Binary:**  
  A binary number that represents both positive and negative values. Methods include **sign-magnitude, one’s complement,** and **two’s complement**.

- **Sign Bit:**  
  The leftmost bit in signed binary numbers that indicates the sign:  
  - `0` for positive  
  - `1` for negative  

---

### **Representations of Negative Numbers:**
- **Sign-Magnitude:**  
  The MSB (most significant bit) represents the sign, and the remaining bits represent the magnitude.  
  Example: `10011001` = -25

- **One’s Complement:**  
  Negative numbers are represented by inverting all the bits of the positive number.  
  Example: `25` (decimal) → `00011001` → `11100110` (one’s complement for -25)

- **Two’s Complement:**  
  Formed by inverting all bits of a number and adding 1. The most commonly used method in computers.  
  Example: `11100111` = -25  

---

### **Binary Operations:**
- **Addition:**  
  Similar to decimal addition but with only `0` and `1`.  
  - `1 + 1 = 10` (carry the `1`)  

- **Subtraction:**  
  Typically performed by adding the **two’s complement** of the subtrahend.  
  Example: `5 - 3` → `5 + (-3)`

- **Multiplication:**  
  Repeated addition of binary numbers, often with bit-shifting.

- **Division:**  
  Repeated subtraction, similar to long division in decimal.

---

### **Logical Operations:**
- **AND:**  
  `1 AND 1 = 1`, otherwise `0`  
  Example: `1010 AND 1100` → `1000`

- **OR:**  
  `1 OR 0 = 1`, only `0 OR 0 = 0`  
  Example: `1010 OR 1100` → `1110`

- **XOR (Exclusive OR):**  
  `1 XOR 1 = 0`, `1 XOR 0 = 1`  
  Example: `1010 XOR 1100` → `0110`

- **NOT:**  
  Inverts each bit.  
  Example: `NOT 1010` → `0101`

---

### **Bitwise Operations:**
- **Bit Shift (Left or Right):**  
  Moves bits left or right, filling with zeros.  
  Example: `1010 << 1` → `10100` (Left shift by 1)

- **Arithmetic Shift:**  
  Similar to bit shifts but preserves the sign bit during right shifts.

---

### **Overflow and Carry:**
- **Overflow:**  
  Occurs when the result of an operation exceeds the fixed bit length.  
  Example: Adding `01111111` (127) and `00000001` causes overflow.

- **Carry:**  
  When a `1` is carried to the next column during addition.  

---

### **Miscellaneous:**
- **LSB (Least Significant Bit):**  
  The rightmost bit in a binary number.

- **MSB (Most Significant Bit):**  
  The leftmost bit in a binary number.

- **Parity Bit:**  
  A bit added to maintain even or odd parity (used in error detection).

- **Masking:**  
  Using a bitwise AND to extract specific bits from a binary number.

- **Twos Complement Wraparound:**  
  When subtracting large numbers, the result “wraps around” to the opposite end of the binary range.
