When a **MOSFET is diode-connected**, it means its **gate and drain are shorted** together. This forms a 2-terminal device that behaves similarly to a diode, with **unidirectional current flow** and a **threshold voltage drop**.

---

### **Which terminal is the anode and which is the cathode?**

- **Anode** → **Source**
- **Cathode** → **Gate/Drain** (since they are connected)

---

### **Why?**

For an **nMOS** transistor:

- Current flows when \( V_{GS} > V_{th} \).
- In the diode-connected configuration, \( V_{GD} = 0 \), so \( V_{GS} = V_{DS} \).
- Current flows from **drain to source**, i.e., **from cathode to anode** (just like a normal diode).
- So the **source** must be at a lower potential → **acts as the anode**.
- The **gate/drain** must be at a higher potential → **acts as the cathode**.

---

### **Summary**

| Device Type | Gate = Drain (Cathode) | Source (Anode) |
|-------------|------------------------|----------------|
| **nMOS**    | High potential         | Low potential  |
| **pMOS**    | Low potential          | High potential |

So, **anode = source**, **cathode = gate/drain**, for both nMOS and pMOS, considering conventional current direction.
