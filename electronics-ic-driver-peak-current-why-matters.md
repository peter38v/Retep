---
id: electronics-ic-driver-peak-current-why-matters
aliases:
  - electronics-ic-driver-peak-current-why-matters
tags: []
---
# Why does peak current matter?

> If peak current too small
- Rise/fall time increases (more slope)
- Switching energy increases (Vds and Ids overlap more -> (SW_e & temp up)
- More losses in deadtime due to diode conduction
- Lower PWM resolution -> less control

> If peak current too large
- dv/dt & di/dt increase -> more parasitics and more emissions
- Ringing & overshoot increase 
- Higher false turn-on risk
- Lower reliability long term due to overshoot/undershoot challenges

> How to balance?
- Split the on and off resistance -> independent tuning of turn-on and off
- Limit parasitics -> watchout for [[electronics-loop-inductance|loop inductance]] and set good layout
- Tuning tf & tr

> Are you goated with it?
- Rise time/fall <= **X** ns at operating point
- VGS overshoot <= **Y**V and undershot >= **-Z**V 
- EMI margin >= **N** dB at required standard
- Driver [[electronics-supply-droop|supply-droop]] <= **M** V during switching bursts 
