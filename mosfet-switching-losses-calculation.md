---
id: mosfet-switching-losses-calculation
aliases:
  - mosfet-switching-losses-calculation
tags: []
---
# MOSFET switching loss calculation
- Two components: Turn-on loss & turn-off loss
$$
E_{on} = 1/2 * V_{ds} * I_d * t_{on}
$$

$V_{ds}$ = Drain-Source Voltage

$I_d$ = Continous Current through MOSFET

$t_{on}$ = time it takes for MOSFET to turn on

$$
E_{off} = 1/2 * V_{ds} * I_d * t_{off}
$$
very similar

Total switching loss = $E_{on} + E_{off}$

so if:
V_ds = 100V
Id = 10A
t_on = 50ns
t_off = 50ns

$$
E_on = 1/2 * 100V * 10A * 50ns = 0.25mJ
E_off = 0.25mJ
$$
P_sw = 0.5mJ voila

$$
P_{sw} = 1/2 V_{ds} * I_d * (t_r+t_f) * f_{sw}
$$
