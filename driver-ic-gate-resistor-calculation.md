---
id: driver-ic-gate-resistor-calculation
aliases:
  - driver-ic-gate-resistor-calculation
tags: []
---
# How to calculate Gate Resistor value for MOSFET

The switching behaviour is influenced by: 
- Gate Resistor
- Input Capacitance ($C_{iss}$) of the power switch

$C_{iss}$ is NON-linear -> easier to calculate with $Q_G$ and switching times.
find $t_r$ and $t_f$ in MOSFET datasheet

$$
R_{G,application} = \frac{\Delta V_{GS,application} * (t_r + t_{d(on)})}{Q_G} - R_{G,int}
$$

>[!Important]:
- Extract $Q_G$ from the gate-charge diagram in the datasheet of MOSFET
- Select the points for voltages $V_{VEE2}$ & $V_{VCC2}$ -> Read values for off and on-state gate charges
- Then calculate $Q_G$ as a difference between the 2 charges

[next](driver-ic-power-dissipation-calculation)
