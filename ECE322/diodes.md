- N-material has free electrons
- P-material has room for them to move to 
- Where they meet is the depletion zone

---

Biasing $\Longrightarrow$ applying voltage

- No voltage = no bias $\Longrightarrow$ no current flow
- positive voltage = forward bias $\Longrightarrow$ large current flow because depletion zone shrinks
- negative voltage = reverse bias $\Longrightarrow$ small reverse saturation current

$V_T$ = thermal voltage: approx 26mv at room temp

---

### IV graph:
- x-axis = voltage
- y-axis = current

---

$V_k$ = knee voltage: minimum voltage for conduction. where current spikes on IV graph

$V_b$ = voltage breakdown; when negative voltage overcomes depletion region and ruins diode

$V_b$ has a much greater magnitude than $V_k$

---
conduction
- **Forward Conduction**: When the forward voltage (typically around 0.7V for silicon diodes and 0.3V for germanium diodes) is applied, the diode enters conduction mode and current flows.  
- **Reverse Bias (Non-Conduction)**: When the diode is reverse-biased (anode connected to the negative terminal and cathode to the positive terminal), the diode ideally blocks current and does not conduct, except for a very small leakage current.  
- **Knee/Threshold Voltage**: The point at which the diode begins to conduct significantly in the forward direction is known as the **cut-in** or **threshold voltage** or **knee voltage**.  

---

| **Material** | $V_k$    | $V_b$     | 
| :----------- | :------: | :-------: |
| Silicon      | 0.7v     | -75v      | 
| Germanium    | 0.3v     | -50v      |
| GaAs         | 1.5v     | -100      |

---

### DC static resistance  
$R_D = \dfrac{V_D}{I_D}$
- Taken at a singular point on the IV graph.

---

### AC dynamic resistance:
$R_d = \dfrac{\Delta V_d}{\Delta I_d}$
- From the peak to the trough of a sine wave
$R_{d} = \dfrac{V_{peak} - V_{trough}}{I_{peak} - I_{trough}}$

---

### Average AC resistance

$R_{av}=\dfrac{\Delta V_d}{\Delta I_d} {\Large\vert}_{Point \ to \ Point}$

---

### Piecewise Linear Equivalent Circuit
In the real world we treat a diode as if it does not conduct at all until the knee voltage, where we assume a linear increase.

---

#### $I_0$

Changing the dark saturation current changes the turn on voltage of the diode. The ideality factor changes the shape of the diode.

Any physical effect that increases the ideality factor would substantially increase the dark saturation current, $I_0$, so that a device with a high ideality factor would typically have a lower turn on voltage.

---

### Transition Capacitance/Junction Capacitance

The depletion zone is a gap similar to the gap between capacitor plates.

When forward biased, there is no capacitance.

When reverse-biased there is capacitance

Wide depletion region = small capacitance
Narrow depletion region = large capacitance

$C_T = \dfrac{\Delta Q}{\Delta V}$

---

###Reverse Recovery time

There is a lag from when bias is switched from forward to reverse where the diode still conducts current.

Denoted as $t_{rr}$  

The "storage time", or the delay, is $t_s$: Amount of time the diode conducts reverse current

The transition time is $t_t$: Time it takes to ramp up/down in voltage after switching

and $t_{rr}=t_s+t_t$

 





