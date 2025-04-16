study from lec-9 to lec-20 for exam 2

---

# Biasing

$A_V = -gm\cdot R_L$

and 

$-gm = \frac{I_C}{V_{th}}$

---

1. single supply biasing

- base is biased wtih same $V_{CC}$ as collector.

- $R_C$ gives the feedback

$I_C$ increase causes increade in $V_E$, which causes decrease in $V_{BE}$ which causes decrease in $I_C$

- find thevanin equivalents

- KVL: $V_{thevanin} -R_{thevanin}I_B-V_{BE}-I_ER_E=0$

$V_{thevainin} - V_{BE} = \frac{R_{thevanin}}{\beta+1}I_E+I_ER_E$

$I_E=\frac{V_{thevain}-V_{BE}}{\frac{R_{thevanin}}{\beta+1}+R_E}$

- Design choice $V_{thevanin} > V_{BE}$
- Design choice $R_E > \frac{R_{thevanin}}{\beta+1}$

$I_E \approx \frac{V_{BB}}{R_E}$

2. Supply biasing

two supplies: $V_{CC}$ and $-V_{EE}$

- KVL: $0-V_{BE}_I_ER_E=-V_{EE}$

$I_ER_E=V_{EE}-V_{BE}$

$I_E=\frac{V_{EE}-V_{BE}}{RE}$

- Design choice $V_{EE} > V_{BE}$
- Design choice $V_{EE}-V_{BE} \approx V_{EE}$

3. Self Biasing

- one supply $V_{CC}$
- Base connected to collector with resistor
- $I_E=I_C+I_B$

- KVL: $V_{CC}-I_ER_C-I_BR_B-V_{BE}=0$

$V_{CC}-V_{BE}= IE\left[ R_C+ \frac{R_B}{\beta+1}\right]$

$I_E=\frac{V_{CC}-V_{BE}}{R_C+}$....

$I_E\approx\frac{V_{CC}}{R_C}$


4. constant current biasing

- current source on emitter independent of $\beta$ etc

-As long ase $V_{CE}$ is larfe enough can create constant currrent source

$I_C=I_S e^{\frac{V_{BE}}{V_{th}}}$

$\frac{I_C}{I_S}=e^{\frac{V_{BE}}{V_{th}}}$

$V_{BE}= V_{th} ln(\frac{I_C}{I_S})$


($I_S$ is saturation current)

---

bandgap

KVL: $V_{CC}-I_CR-V_{BE}=0$

$V_{CC}-I_CR-V_{th}ln(\frac{I_C}{I_S})=0$

5. current mirror

$I_C=I_S e^{\frac{V_{BE}}{V_{th}}}$

$I_{S_Q1} = I_{S_Q2}$

$I_S=f(EBJ_{area})$

if $EBJ_{Q2} = 2 EBJ_{Q1}$






