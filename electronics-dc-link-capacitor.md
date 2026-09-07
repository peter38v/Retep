---
id: electronics-dc-link-capacitor
aliases:
  - electronics-dc-link-capacitor
tags: []
---

# DC link capacitors

Breakdown of: [Spectre-Engineering](https://www.specterengineering.com/blog/2019/9/7/dc-link-capacitor-selection-for-your-inverter)

*Jobs*:

- Provide low-impedance path for high-frequency currents (freq up, battery impedance up, cap impedance down)
- Sizing depends on ripple current -> how much ripple current the cap can take 
- Voltage bus is like a rope bridge, the capacitor is the tensioner, bridge has tolerance spec (max DC Voltage ripple)

In conclusion: it must take care of ripple current and ripple voltage

## Types of Caps

Two main ones are a) film b) electrolytic

- Modern inverters use film caps due their low ESR and ESL 
learn more -> [[electronics-esr]] [[electronics-esl]]
- Also film caps have higher working lifetime (10k vs 100k hours)

## Interesting

- Capacitance is inversely proportional to switching frequency
- Capacitor volume is proportional to capacitance
- As switching frequency increases, the capacitance required decreases

THUS if switching freq goes up, power density does as well
Switch faster -> less capacitance required -> volume decreases -> higher kW/L and kW/kg

# Conclusion
Caps have current ripple rating, resonant frequency and dc voltage rating

## Current Ripple: 
Select one with 1.1x the ripple rating of the worst case ripple in system
How to calculate current ripple -> [[electronics-current-ripple-calculation]]

## DC Voltage:
Choose one with 1.1x the voltage of the battery at 100% SOC

## Resonant Frequency:
Should be 2x the switching frequency
