---
id: driver-ic-peak-current-calculation
aliases:
  - driver-ic-peak-current-calculation
tags: []
---
# Calculate for Peak Current


$$
I_g = \frac{\Delta V_{gsDatasheet}}{R_{G,datasheet}+R_{G,int}}
$$


where,


$$
\Delta V_{gsDatasheet} = V_{gs(on)} - V_{gs(off)}
$$

$\Delta V_{gs}$ is the difference between the gate (0V) and the amount of Voltage the driver IC
supplies to it.

$R_{G_int}$ is the internal gate resistance of the MOSFET (often found in electrical characteristics section)

$R_{G,datasheet}$ is any added resistance into the circuit via Resistor.

>Set $I_g$ as max source current of driving IC -> let $R_G$ become minimum value that you must
stay above!

A very handy formula is:

$$
I = \frac{\Delta Q}{\Delta t}
$$

Therefore, if a MOSFET needs 50 nC to turn on, and you want to do it in 50ns:
$$
I = \frac {50nC}{50ns} = 1 A
$$
this is obviously without any losses.

[next](driver-ic-gate-resistor-calculation)

