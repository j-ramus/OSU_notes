$V_B = 10v \quad R_B=1k$

with vbe 0.7

$I_B = \frac{10-0.7}{1k}$

wiggle in vbe = wiggle in ic

$\frac{ic}{vbe}=gm$

$\frac{vbe}{ib}=r\pi=\frac{\beta}{gm}$

$\frac{vbe}{ie}=re=\frac{\alpha}{gm}$

Avoid using T-models for cases where $\beta=\infty$

---

### AC analysis of BJT amplifier

1. dc analysis

  - Kill all ac excitation:
  - short all AC voltage sources
  - open all AC current sources
  - eaiser AC value $0\cdot\sin{(\omega t)}$
  - open all capacitors -> they pass no dc current
  - calculate all DC voltages and currents
  - $I_C \longrightarrow gm=\frac{I_C}{V_{th}}$
  2. AC analysis
  - calculate small signal parameters
  - draw small signal model of bjt
  - short all capacitors -> they let AC flow
  - $C_{BFC} = \frac{1}{j\omega c}$ where $\omega$ is large and $c$ is large
  - Replace all DC voltage sources with AC ground
  - Replace all DC current sources with open
  - if a node is tightly held by DC and there is no ac signal, replace with AC ground (not moving with relation to AC)
  - dc current tightly controls curretn and wins against AC
  - DC wins and AC cant change it
  3. solve for AC gain
  - AC ground -> 0v AC
  - DC ground -> 0v AC and 0v DC
  - Vo is across AC and DC ground
  - gain $= \frac{vo}{vi}$
  

