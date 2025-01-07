In **sign-magnitude representation** for an 8-bit binary number:
- The **leftmost bit** (most significant bit or MSB) is the **sign bit**.
- The remaining **7 bits** represent the **magnitude** (absolute value) of the number.

### Breakdown:
- **0xxxxxxx** → Positive number  
- **1xxxxxxx** → Negative number  

Where **`xxxxxxx`** is the binary representation of the magnitude.

---

### Example:
1. **+25 (decimal):**  
   - Binary for 25: `0011001` (7 bits)  
   - Add sign bit (`0` for positive): `00011001`  
   **Result:** `00011001`  

2. **-25 (decimal):**  
   - Binary for 25: `0011001` (7 bits)  
   - Add sign bit (`1` for negative): `10011001`  
   **Result:** `10011001`  

---

### Important Notes:
- **Magnitude does not change** when switching between positive and negative.  
- The sign bit is purely for **indicating direction** (positive or negative).



When comparing **sign-magnitude** to **non-sign-magnitude** representations like **two's complement**, here’s a simple way to think about it:

---

### **Colloquial Identification:**

1. **Sign-Magnitude: "The leftmost bit just tells you if it's positive or negative."**  
   - The **value** doesn’t change except for the sign.  
   - Flip the leftmost bit to switch between positive and negative.  
   - **Example:**  
     - `00011001` → +25  
     - `10011001` → -25  

---

2. **Two’s Complement: "The whole number flips and shifts for negatives."**  
   - It’s not just the leftmost bit; the **entire binary value changes** for negatives.  
   - **Example:**  
     - `00011001` → +25  
     - `11100111` → -25  
   - To recognize two’s complement negatives:  
     - If the leftmost bit is `1`, the whole number represents a negative value.  
     - You can convert it by **inverting all bits and adding 1**.

---

### **How to Spot the Difference Quickly:**
- **Sign-Magnitude:** The leftmost bit looks like a simple "switch."  
- **Two’s Complement:** The entire number looks "upside down" for negatives (with 1’s and 0’s flipped).  

---

### **Analogy:**
- **Sign-Magnitude** is like **flipping a sign on a price tag**:  
  - “$25” → “-$25” (same digits, different sign).  
- **Two’s Complement** is like **turning the price into a discount code**:  
  - $25 → A weird code that requires decoding to know it means -25.

