---
id: mosfet-peak-phase-current-calculation
aliases:
  - mosfet-peak-phase-current-calculation
tags: []
---
# Calculations into estimating peak phase current based on DC bus current

To spec I_d of MOSFET, need to figure out how much your peaks might be

Method:
1. Find desired DC-bus peak continous current (I_dc)
2. Do estimation calculation

I_phase_peak ~= I_dc/(D*sqrt(3)*cos(theta))

    where:
    D = Effective Duty Cycly
    theta = Power Factor

>[!warning] set D -> 1 and cos(theta) -> 0.5, this will give a good overhead

>[!example]
>I want 50A DC bus current continous at peak
>My peak phase current shall be around -> 50/(1*sqrt(3)*0.5) = 57.73 [A]
> Throw a calm 25% Safety factor on it -> 72 [A] <- This is your MINIMUM I_d value
