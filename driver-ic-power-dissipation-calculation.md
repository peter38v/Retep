---
id: driver-ic-power-dissipation-calculation
aliases:
  - driver-ic-power-dissipation-calculation
tags: []
---
# Power Dissipation calculation for Gate Driver IC

>[!note]
This is a simplified formula, it assumes:
- Losses during switching are only dissipated in the output stage of the gate driver ic
- They are dominated by the charging and discharging of gate capacitance

$$
P_D = Q_G * f_{SW} * \Delta V_{GS,application}
$$

After the calculation is done:
- Compare the result to Driver IC datasheet $P_{D,OUT}$ in the output side of the driver at 25C
- It should be smaller or equal to this value

Also consider the fact that this number gets worse as the chip gets hotter

$$
\Delta T_j = P_{D,OUT} * R_{th(j-a)}
$$

Find the value for thermal resistance $R_{th(j-a)}$ in the datasheet of the MOSFET
