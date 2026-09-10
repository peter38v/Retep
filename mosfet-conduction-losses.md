---
id: mosfet-conduction-losses
aliases:
  - mosfet-conduction-losses
tags: []
---
# Conduction Loss/Thermal Calculation for MOSFET

- Loss is based on current flowing (Id) & RDsON value and Duty cycle(in %)
R_dson * Id^2 * D = Power Loss (in Watts)

Example:
Id = 80 [A] @ Ambient
R_dson = 7.34 [mOhm]
D = 100% / 1

Pd = 80^2 * 0.00734 * 1 = 46.976 Watts
