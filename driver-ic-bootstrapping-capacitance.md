---
id: driver-ic-bootstrapping-capacitance
aliases:
  - driver-ic-bootstrapping-capacitance
tags:
  - formulas
---
# Bootstrapping Capacitance formula

$$
C >= 2 * \frac {(2*Q_G)+(\frac {I_{qbs(max)}}{f_{sw}})+Q_{ls}+(\frac {I_{cbs(leak)}}{f_sw})}{V_{cc}-V_f-V_{ls}-V_{min}}
$$

where,

Qg = Gate charge of high-side FET (fet datasheet) \
f_sw = Frequency of operation (lower freq -> bigger cap) \
Icbs(leak) = Bootstrap capacitor leakage current ($I_{GSS}$ in capacitor datasheet)\
Iqbs(max) = Maximum VBS quiescent current (gate driver datasheet!)\
Vcc = Gate driver supply Voltage(down to your application)\
Vf = Forward voltage drop across the bootstrap diode(diode datasheet)\
VLS = Voltage drop across the low-side FET or load \
VMin = Minimum voltage between VB and VS \
Qls = Level shift charge required per cycle (typically 5 nC for 500 V/600 V MGDs and 20 nC for 1200 V MGDs) \


