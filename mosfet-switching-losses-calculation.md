---
id: mosfet-switching-losses-calculation
aliases:
  - mosfet-switching-losses-calculation
tags: []
---
# MOSFET switching loss calculation
- Two components: Turn-on loss & turn-off loss

E_on = 1/2 * V_ds * Id * t_on

V_ds = Drain-Source Voltage
Id = Continous Current through MOSFET
t_on = time it takes for MOSFET to turn on

E_off = 1/2 * V_ds * Id * t_off
very similar

Total switching loss = E_on + E_off

so if:
V_ds = 100V
Id = 10A
t_on = 50ns
t_off = 50ns

E_on = 1/2 * 100V * 10A * 50ns = 0.25mJ
E_off = 0.25mJ

P_sw = 0.5mJ voila

>[!note] P_sw = 1/2 V_ds * Id * (t_r+t_f) * f_sw 
