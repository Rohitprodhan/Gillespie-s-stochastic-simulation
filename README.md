# Gillespie-s-stochastic-simulation

Consider the Lotka-Volterra equations for an imaginary predator-prey system. A prey species
Y1 reproduces by feeding on some food (designated X), which is assumed to be available in a
large enough quantity that it is not significantly depleted. A predator species Y2 reproduces by
feeding on the species Y1 and also eventually dies through natural causes.
The reactions describing these coupled processes can be represent by the set of auto-catalytic
reactions,

This is some text ^above the arrow -> and this is text after the arrow.

$$[Food] + Y_1 \xrightarrow{c_1} [Food] + 2Y_1$$

$$Y_1 + Y_2 \xrightarrow{c_2} 2Y_2$$

$$Y_2\xrightarrow{c_3} \phi $$

The deterministic reaction rate equations for the populations of the species Y_1 and Y_2 are
$$\dfrac{dY_1}{dt} = c_1Y_1 − c_2Y_1Y_2$$
$$\dfrac{dY_2}{dt} = c_2Y_1Y_2 − c_3Y_2$$

Now write a code to simulate these coupled reactions through Gillespie’s stochastic simulation
algorithm, for the following choice of the rate constants,
$$c_1 = 10, c_2 = 0.01, c_3 = 10$$
Assume initial conditions,
$$Y_1(t = 0) = Y_2(t = 0) = 1000$$
Perform 3 independent simulations for these initial conditions, and generate plots of Y1 and Y2
as a function of time in the time interval 0 ≤ t ≤ 30. Also plot the trajectory in the Y1 − Y2
phase plane.

Assume another initial condition,
$$Y1(t = 0) = 500, Y2(t = 0) = 200$$
Again, perform 3 independent simulations for these initial conditions, and generate plots of Y1
and Y2 as a function of time in the time interval 0 ≤ t ≤ 30. Also plot the trajectory in the
Y1 − Y2 phase plane
