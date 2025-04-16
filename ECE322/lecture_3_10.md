small signal assumption assumes $vbe<Vth$

gate volatge must exceed threshold voltage (like barier voltage of diode)
1v, 2v

gate to source volatge can be higher than threshold voltage

VDS > VGS-VT

VGS-VT = overdriver voltage

### Regions of Opertation MOSFET

1. Cutoff: 
- VGS < VT
- VDS =0
- No channel

2. Strong Inversion region

-VGS > VT
- VDS = 0

3. Linear region

- Not the same as BJT, closer to BJT saturation

- VGS > VT
- VDS < VGS -VT
- ID is linearly dependent on VDS (where name comes from)

- NMOS $ID=K'\frac{W}{L}[(VGS-VT)VDS-\frac{VDS^2}{2}]$



4. Saturation region

- Similar to active region of BJT
- VGS > VT
- VDS > VGS-VT
- drain current (ID) saturates and becomes weakly dependent of VDS

-   NMOS $ID=K'\frac{W}{2L}(VGS-VT)^2$

ID to VDS is similar to the IC to vbe graph


---

K or K' = $\mu n Cox$$

$Cox=\epsilon_0-\epsilon_r\frac{A}{d}$

---

- VT is positve for NMOS
- PMOS (linear)   $ID=K'\frac{W}{L}[(VSF-|VT|)VSD-\frac{VSD^2}{2}]$

-   pMOS $ID=K'\frac{W}{2L}(VGS-|VT|)^2$
$\frac{\delta ID}{ \delta VGS}= gm$
$r\pi=\infty$


T-model is not valid for MOSFET, use hybrid pi



