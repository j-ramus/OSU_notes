# Final exam:
3/21 at 7:30

---

Small signal analysis needs more accurate modeling than a 0.7v approximation.

dpenedent soyrce behavior is how transistors are analyized as ampifiers.

---

# BJT

$I_E=i_C+i_B$

$I_E = (1 + \beta)\cdot i_B$

$\beta$ is a constant: curretn gain $\beta \approx 50 - 100$ (scalar multiplier)

$i_C = \beta \codt i_B$

$\aplha = \frac{\beta}{\beta + 1} Alpha is a current gain constant $\leq 1$

base curretns are always very small

$\beta = \frac{\aplha}{}$

---

### Example 1

Find RC and RE s.t. $I_E=1mA$

given:

$V_{BE}=0.7v \ \longrightarrow V_B- V_E=0.7v$

$V_C =5v$ on other side of RC from $15v$ input

$\beta = \infty$

$V_E=$?

$I_B = \frac{I_C}{\beta}\therefore I_B=0$

This means no electons folow throgh the base to ground (Base is connected to ground)

if $V_{BE}=0.7$ and $V_B=0$, $V_E=-0.7v$


---

alwasy label NPN points and BCE points

emmiter base junction has to be forward biased

---

### Example 2

given:

$V_B = 1v$ base, ntype

$V_{EB}$ = 0.7v (assumed) EBJ is Forward biased

$V_B = 1v$, and $V_E - V_B =0.7v \ \therefore V_E = 1.7v$

$I_B = \frac{1V}{100k}= 0.01mA$

$I_E = \frac{10-1.7}{5k}=1.66mA$

$V_C$ cannot be calculated because base to collector junction is reverse biased
and any voltage across it can be anything.

Can be indiretly calulated by other volatges

$1.66mA = (\beta+1)\cdot0.01mA \longrightarrow 166=\beta+1$
$\therefore \beta=165$

---

## MOdes of operation


##### NPN

- EBJ Forward bias $V_B \geq V_E +0.7v$...

- see lecture 9b notes

---

1 sided hand written 8.5 by 11
