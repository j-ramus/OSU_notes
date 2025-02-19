# AC ground vs DC ground

- ground has many different meanings

- reference plane against all other voltages are measured

- Ground is the path of least resistance

- In PCB one full layer is dedicated to ground

- AC ground means there is no AC signal, or the signal is zero at that point

- see diagram in lecture 15: the posistive terminal in top left diagram becomes ac ground

- eliminate DC to analyze AC

- with AC in series after DC, the DC source is a zero impedance point which makes it ground

- decopling capacitors stop AC and let pure dc through

- AC ground does not physically exist, but a concept for paper calculations
---

- KVL works for LTI system, if not LTI try to simplify to LTI

$v_o = -(RC||RL)gm\cdot v_{be}$
 $vbe=(\frac{r\pi}{r\pi+RB})\cdot v_i$
 $v_o -(RC||RL)gm\cdot (\frac{r\pi}{r\pi+RB})\cdot v_i$
$\frac{v_i}{v_o}= -(RC||RL)gm\cdot (\frac{r\pi}{r\pi+RB})$

---


for pnp PNP (lecture 15 notes)

- coupling circuit. Bias with voltage divider, then to coupling cap and ac signal

- emmiter capacitor makes sure IE is shorted for dc, but not ac

- t model: $v_{be} = $

$\frac{v_i-vbe}{rs} =\frac{vbe}{RB1||RB2}+\frac{vbe}{re(\beta+1)}$

skiped step

$vbe=\frac{\frac{vi}{Rs}}{[\frac{RB1+RB2}{RB1\cdot RB2}+\frac{1}{re(\beta+1)}+\frac{1}{Rs}]}$

gain: $\frac{vo}{vi}=-\frac{(RC||RL)gm}{RS}[\frac{RB1+RB2}{RB1\cdot RB2}+\frac{1}{re(\beta+1)}+\frac{1}{Rs}]$
- vbe is the last node befor the EBJ


