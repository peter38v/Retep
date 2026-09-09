---
id: electronics-inverter-low-side-current-sensing
aliases:
  - electronics-inverter-low-side-current-sensing
tags: []
---
# Low side current sensing in 3 Phase Inverters using Shunts

- Shunt Resistors are placed between Low-Side MOSFET and DC ground
- Triple-Shunt or Dual-Shunt variation exist
- Cannot sense current when low-side MOSFET is open, instead phase current is measured
from assumption of symmetrical inverter load (i_a + i_b + i_c = 0) (2 other phase currents
must be known)

## Triple-Shunt configuration


>[Pros]
- Allows for full DC Bus Voltage utilization (100% Duty Cycle)
- Requires only 2 ADC modules to obtain motor currents simultaneously
- Could revert to Dual-Shunt operation if one circuit fails

>[Cons]
- Higher Cost, more circuitry required

![[Pasted image 20260908125536.png]]

## Dual-Shunt configuration

>[Pros]
- Lower Cost, less circuitry

>[Cons]
- Cannot Operate with 100% duty cycle:
Duty cycle has to be limited -> low-side MOSFET minimum ON time > ADC conversion time
MOSFET ON time >= 2*ADC conversion time due to symmetrical PWM pattern

>[!warning]
In a real system -> Transient settling & deadtime must be considered 





