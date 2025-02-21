# todo

practice finding thevainin equivalent of transistor base

use poles and zeros if caps are not $\infty$

---

looking into the base, the emmiter current gets miltiplied by $\beta + 1$

---

# Lec - 18

## common base

$R_i = \frac{v_{test}}{i_{test}}$

$i_e =(\beta+1)\cdot i_b$

$i_e=-i_{t}$

KVL: $0-R_Bi_b-r_ei_e=v_t$

$-\frac{R_bi_e}{\beta+1}=v_t$

$-ie[\frac{R_B}{\beta+1}+r_e]=v_t$

Resistance reflection rule 2

$\frac{v_t}{i_t}=re+\frac{R_B}{\beta+1}$

convert above to $r\pi$:

$\frac{v_t}{i_t}=\frac{r\pi}{\beta+1}+\frac{R_B}{\beta+1}$

if $gmv\pi = 0$, dependent current source is open

$G_m = \frac{i_o}{v_t}=-\frac{gmr\pi}{r\pi+R_B}$

$A_V = \frac{v_{out}}{v_s} = =G_m\cdot R_o$

$A_V=(\frac{gmr\pi}{r\pi+R_B})R_C$ Note gain is positive

Common emmiter gives $180^\circ$ phase shift

---

## common collector AKA emmiter follower AKA source follower

R_i= use RR rule #1

$R_i = r\pi+R_i(\beta+1)$ or $(re+R_L)(\beta+1)$

$R_O = re || R_L$

T-model can be easier for common collector Ro

draw both models if not sure

$Gm=\frac{i_o}{v_{test}}$

$ie=-io$

$ie=(\beta+1)ib$

$ib=\frac{v_{test}}{r\pi}$

$io=-(\beta+1)\frac{v_{test}}{r\pi}$

$\therefore GM=\frac{io}{v_t}=\frac{-\beta}{r\pi}\approx=-gm$

$r\pi=\frac{\beta}{gm}$

$gm=\frac{\beta}{r\pi}$

$re=\frac{\alpha}{gm}$

$A_V=-(-gm)\cdot re||R_L=gm\cdot\frac{reRL}{re+R_L}\approx gm\cdot re \approx \alpha$

$A_V\approx\alpha\longrightarrow1$


Common collector is an autenuator

1. Drive large load (ex: speaker)

2. advantage of swing



3. Reduction of supply noise



