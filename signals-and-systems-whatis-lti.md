---
id: signals-and-systems-whatis-lti
aliases:
  - signals-and-systems-whatis-lti
tags: []
---
# LTI for idiots

x(t) -> y(t)
    as per system

if Linear:
A * x(t) = A * y(t)     <- input scaled, outside scaled, by as much
        or
x_1(t) + x_2(t) = y_1(t) + y_2(t) <- addition of two inputs, added output

if Time-invariant:
x(t-tau) = y(t-tau)     <-  Shifted by just as much

# How to solve?
x(t) -|h(t)|-> y(t)

system behaviour is characterized by impulse response h(t)

h(t) <- very sharp input, hammer strike or something
what will the system do to respond?
Impulse is always the [delta function](<signals-and-systems-basics-types-unit-impulse#Unit Impulse function>)


y(t) = h(t) *([[signals-and-systems-convolution|convolution]] ) x(t) = integral(h(t-tau) * x(tau) d_tau)


[[youtube-lti-systems|Learn-more]]
