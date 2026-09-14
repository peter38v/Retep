---
id: electronics-driver-ic-selection
aliases:
  - electronics-driver-ic-selection
tags: []
---
# How to size and spec driver IC
[Article by infineon](https://community.infineon.com/t5/Knowledge-Base-Articles/Selecting-gate-driver-ICs-a-simplified-guide/ta-p/957353#.)
Everything in 5 steps:

1. Define the needs
Select the MOSFET, select the gate driver configuration (low-side,level-shift,isolated)
and bridge type (hal-bridge,single,etc.)

2. Sizing and selection
[[driver-ic-calculations|Calculate]] IG_max & RG (max current and gate resistor value)
Choose gate-driver that meet the voltage class, IG_max and other features

3. Power dissipation check
Calculate RG and power dissipation -> check against datasheet

4. Verification
Check if Protection features (Miller Clamp etc.) operate as expected

5. Advanced checks
dv/dt and Thermal behaviour <- Verify if reality = expectation

TUNE RG!!!

![[Pasted image 20260914173712.png]]

