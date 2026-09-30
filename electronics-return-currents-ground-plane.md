---
id: electronics-return-currents-ground-plane
aliases:
  - electronics-return-currents-ground-plane
tags: []
---
# Ground planes as return paths

Ground planes can greatly decrease the loop area -> thus lowering EMI

Having a dedicated ground plane below signal plane and routing to ground via vias (hehe), can greatly reduce EMI

NOTE: If you route a signal to another signal plane (maybe other side of PCB), make sure to route a ground via to another ground layer
closer the other signal layer

This applies in a 4 layer stackup where: signal - gnd - gnd - signal is the setup
