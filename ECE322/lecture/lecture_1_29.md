# Solving BJT

---

####Example 1: 

###### NPN

Given $\beta=100$

- Determine mode of operation

Is EBJ or CBJ forward biased

First identify EBC points and what kind it is (npn vs pnp)

- ultimately what is $V_B$ and what is $V_C$

When EBJ is FB for NPN assume $V_{BE} =0.7v$

For PNP $V_{EB}=0.7v$


What is $V_B$?

Need to find volute drop across $R_B$

if $I_B$ is 0, base volatge is $0v$

$V_B$ is 0.7v

find collector current

$I_B=\frac{10-0.7}{100k}=0.093mA$ and $\beta=100$, $I_C=\beta\cdot I_B \ \therefore I_C=9.3mA$

KVL: $10-1k\codt I_C =V_C$

$10-9.3 = V_C \ \therefore V_C=0.7v$

$V_C \geq V_B$ boundry condition, still considered reverse biased

EBJ = fb, CBJ =rb: it is in the active region

---

### example 2

$V_B =0.7v \quad I_B=0.093mA /quad I_C = \beta\cdot I_B = 9.3mA$

$V_C = 10 -0.5k\codt 9.3 = 5.4v$

EBJ= fb; CBJ= rb; In acitve region

- increat $R_C$ to $2k\omega$:

$V_B=0.7v \quad I+B = 0.093mA$

$I_C=\beta\cdot I_B = 9.3ma$

$10-18.6=-8.6v$?? This cannot be true. you cannot get negative volatge between ground and a negative supply

In this sxenarrio the volatge on the collector starts to go down, but cannot go below zero

$\vert VCE_{min}\vert = given=02.v$ if not given, assume $\vert VCE_{min}\vert=0$

What has gone wrong

$I_C=\beta\cdot I_B$ is not holding

if ebta is constan this is not holding

if beta has dropped to lower value

int this example EBJ = fb; CBJ = fb

for npn we dont want current to flow from base to collector


---

### example 4 (from 2022 midterm)

Given: $\vert V_{BE}\vert = 0.7v$

1. Identify what type of transistor : PNP; CEB

- current flowing though 1k at bottom not $I_E$, it is the current thought the junction

- never **assume** any voltage drop across a ideal current source

- don't assume the -5v is the same on other side of current source

- use given 

- use kvl to solve unknowns (path in red on lecture notes)

- KVL: $5v-10k\cdot I_B -0.7v -1k(I_E - 1mA)=-5v$

- two unknowns, how to solve? $I_E=(\beta + 1)\cdot I_B$

- KVL: $5v-10k\cdot I_B -0.7v -1k(10\codt I_B - 1mA)$

$5-0.7+1 = 10k I_B +10kI_B+10kI_B$

$5+5.3=20kI_B$

$I_B\frac{10.3}{20k}=515\mu A$

$I_C=\beta I_B$

i$V_C =10-2k I_C=0.73$

$V_E-1k(I_E-1mA)=-5v \quad \therfore V_E=-0.85v$

$\alpha = \frac{\beta}{1+\beta}=\frac{9}{10}=0.9$

Remaining current $I_E
