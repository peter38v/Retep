---
id: electronics-ic-driver-uvlo
aliases:
  - electronics-ic-driver-uvlo
tags: []
---
# UVLO

- Has comparator in chip
- If input voltage becomes lower than the UVLO voltage (on/off)
- Then no propagation from input (PWM) to output

Idea is -> something wrong with system -> doesn't allow switching if $V_g$ 
doesn't go high enough. 

BC lower gate voltage -> higher $R_{dson}$ -> more losses -> higher temperature -> cooked
