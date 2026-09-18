---
id: electronics-miller-plateu
aliases:
  - electronics-miller-plateu
tags: []
---
# Da miller plateu

MOSFET turn on has 3 stages:

- Initial increase -> $V_{gs}$ reaches the turn-on threshold
- Miller Plateu -> $V_{ds}$ drops to near zero, lowering $R_{ds(on)}$ in the meantime
- Saturation region -> $V_{gs}$ keeps increasing to final drive level

![[Pasted image 20260918112920.png]]

## Effects
If there is no ringing during turn-on, there will be no ringing in the miller-plateau

During the plateau, the opposing MOSFET low/high side will get a nice [[electronics-miller-injection|miller injection]]
