---
id: mosfet-conduction-losses
aliases:
  - mosfet-conduction-losses
tags: []
---
# Conduction Loss/Thermal Calculation for MOSFET

- Loss is based on current flowing (Id) & RDsON value and Duty cycle(in %)
R_dson * Id^2 * D = Power Loss (in Watts)

$$
R_{ds(on)} * I_d^2 * D = P_D [W]
$$

Example:
$I_d = 80A$
$R_{dson}$ = 7.34 [mOhm]
$D = 1$ == 100%

$$
P_D =  80^2 * 0.00734 * 1 = 46.976 W
$$
