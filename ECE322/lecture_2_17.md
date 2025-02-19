file Lec17

# types of amplifier structure

1. common emmiter
2. common base
3. common collector

every amplifer is a combination of these structures

$Gm=\frac{it}{vt}$


---


## common emitter amplifer

### with emitter degeneration

base: signal

add resistance to emmiter RE

take output to collector side

RE i critical for setting gain

find $R_i$ and $G_m$

### steps for finding Ri

- T model

add test source Vt on base, this allows finding it

write KVL from base source to emmiterr ground

$R_i = \frac{\beta+1}{re+RE}$

$re=\frac{\alpha}{gm}=\frac{\beta}{(\beta+1)gm}=\frac{r\pi}{\beta+1}$

$Ri=r\pi +(\beta+1)RE$

$i_b \equiv i_{test}$

- Hybrid $\pi$ model

assume $i_e$ 

write kvl from bas v_test :

KVL $v_t - r\pi\cdot i_{test}-R_E(i_e)=0$

$R_i=\frac{v_{test}}{i_t}=r\pi+(\beta+1)R_E$

- resistance reflection rule
resistance looking into base = base resistance + aplifier emitter resistance

tansistors transfer resistance from one pin to another

small resistance of load = small gain

you dont want the preamp to see small 2 ohm load, it gets multipled by $(\beta+1)$


- find $R_o$ 

kill excitation on base (ground, set to 0)

put test $v_t$ at collector, parallel to $R_c$

if you look at resistance $Ro` || Rc$

current flowing towards emitter: $\frac{v_t}{R_c}$

KVL $0-v\pi -ie\cdot RE =0 $

where $ie = (\beta+1)\cdot i_b$

$0-v\pi-(\beta+1)\frac{v\pi}{r\pi}=0$

$v\pi [1+(\beta+1\frac{RE}{r\pi})]$

$v\pi$ must be 0, $\therefore \ gm\codt v\pi =0$

dependent current spource is 0a, no current, open $\infty$ resistance

$Ro=Rc$

- find $Gm$:

short output to ground

$Gm-\frac{i_o}{v_{test}} \ \therefore i_o=gm\cdot v\pi$

$r\pi+(\beta+1)R_E$


$v\pi$ is voltage drop across $r\pi$

using reflection rule

$v\pi\frac{r\pi}{r\pi+(\beta+1)R_E}\cdot v_i$

$Gm = \frac{i_o}{v_i}= \frac{gm r\pi}{r\pi+(\beta+1)RE}$


---

### find voltage gain

$v_o =-R_c\cdot gm\cdot v\pi$

using RR rule

$v\pi=\frac{r\pi}{r\pi+(\beta+1)R_E}\codt v_i$

$\frac{v_o}{v_i}=-\frac{gm R_C r\pi}{r\pi+(\beta+1)RE}$

simplify: divide numerator and denom by $r\pi$

gm is $\frac{i_c}{v_th}$

$A-V=-\frac{gmRC}{1+\frac{\bet+1}{r\pi}\cdot R_E \approx \frac{-gmRC}{1+\frac{\beta}{r\pi}}\cdot R_E}$

$\approx \frac{-gmRC}{gmRE}$

$gmR_E >> 1$


$A_V \approx -\frac{RC}{RE}$

common emmiter always has negative gain

gain is ratio of resistance

op amps are another example of resistance ratio

anything which opposes a change in feedback

---















