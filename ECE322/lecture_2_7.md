# Amplifiers

See lecture 12 onenote for background

---

$v_{ce}$ = wiggle

Voltage gain: $\frac{v_{ce}}{v_{be}}=-\left(\frac{I_C}{V_{th}})\cdot R_C$

Transconductance (siemens): $\frac{A}{V}$

Gain $\prop IC \ & \ \prop RC$

| DC BJT | AC BJT|
| :---- | :---- |
| IC/VBE curve approximated as vertical line at 0.7 | estimated as tangent line to exponential curve centered at Quiesecent point |
| constant voltage drop model | find slope $gm=\frac{\delta I_C}{\delta V_{BE}}=\frac{i_c}{v_{be}}$ |

$gm\prop \ slope$

$gm=\frac{\delta I_C}{\delta V_{BE}}=\frac{i_c}{v_{be}}$ 

You choose Q point as designer


Derivation

$I_C=I_s \cdot e^{\frac{V_{BE}}{V_{th}}}$

$\frac{i_{c}{b_{be}}}= \frac{\Delta I_C}{\Delta V_{BE}}=\frac{\delta I_C}{\delta V_{BE}}= I_S \cdot e^{\frac{V_{BE}}{V_{th}}}\cdot\frac{1}{V_{th}}$

$gm=\frac{I_C}{V_{th}}$

- small signal approximation:

Approximating at non-linear (exponential) curve with a straight line

gm = transconductance = converting voltage to current

more base current = more collector current = more drop in collector voltage through RC

$I_B = \frac{I_s}{\beta}\cdot e^{\frac{V_{BE}}{V_{th}}}$

$r\pi$= base resistance (small signal resistance)

$r\pi=\frac{\beta}{gm}=\frac{v_{be}}{i_b}$

$I_E=\frac{I_S}{\alpha}\cdot e^{\frac{V_{BE}}{V_{th}}}$

$\frac{i_e}{v_{be}}$

bjt: amplification is possible because collector current is independent of collector voltage, and instead the voltage on the other terminals


