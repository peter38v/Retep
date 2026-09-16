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

where,

$V_{gs}$ is Voltage difference gate to how much driver IC puts it to

$t_r$ is the variable -> How fast do you want to switch??
>[!Important]:
- Perchance spec it to max Source Current the driver IC can handle [back](driver-ic-peak-current-calculation)

[next](driver-ic-power-dissipation-calculation)
