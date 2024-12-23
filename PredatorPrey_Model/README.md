# Lotka–Volterra Equations

This article is about the predator–prey equations. For the competition equations, see Competitive Lotka–Volterra equations.

The Lotka–Volterra equations, also known as the Lotka–Volterra predator–prey model, are a pair of first-order nonlinear differential equations, frequently used to describe the dynamics of biological systems in which two species interact, one as a predator and the other as prey. The populations change through time according to the pair of equations:

$$
\begin{aligned}
\frac{dx}{dt} &= \alpha x - \beta x y,\\
\frac{dy}{dt} &= -\gamma y + \delta x y,
\end{aligned}
$$

### Where:
- x is the population density of prey (e.g. the number of rabbits per square kilometre)  
- y is the population density of some predator (e.g. the number of foxes per square kilometre)  
- $\frac{dx}{dt}$ and $\frac{dy}{dt}$ are the instantaneous growth rates of the two populations  
- t represents time  
- The prey’s parameters, α and β, describe, respectively, the maximum prey per capita growth rate, and the effect of the presence of predators on the prey death rate  
- The predator’s parameters, γ, δ, respectively describe the predator’s per capita death rate, and the effect of the presence of prey on the predator’s growth rate  
- All parameters are positive and real  

The solution of the differential equations is deterministic and continuous, implying that generations of both predator and prey are continually overlapping.

The Lotka–Volterra system of equations is an example of a Kolmogorov population model which can model ecological systems with predator–prey interactions, competition, disease, and mutualism.

## Biological Interpretation and Model Assumptions
The prey are assumed to have an unlimited food supply and reproduce exponentially, unless subject to predation. This exponential growth is represented by αx. The rate of predation on the prey is assumed proportional to the rate at which predators and prey meet $(βxy)$. If either x or y is zero, then there can be no predation.
 
The term $δxy$ represents the growth of the predator population. The term γy represents the loss rate of the predators due to natural death or emigration. Hence, the rate of change of the predator population depends on the rate at which it consumes prey, minus its intrinsic death rate.

Main assumptions of the Lotka–Volterra predator-prey model:
- Prey find ample food at all times.
- The predator food supply depends entirely on prey size.
- The rate of change of population is proportional to its size.
- The environment does not change in favor of one species; genetic adaptation is inconsequential.
- Predators have limitless appetite.
- Both populations can be described by a single variable (no spatial or age distribution is considered).

### Biological Relevance
Despite assumptions not holding for many natural populations, the model shows:
1. Tendency to oscillate in predator and prey population sizes (e.g. observed in lynx-hare data and Isle Royale moose-wolf data).
2. The equilibrium density of prey depends on predator parameters, and the equilibrium density of predators depends on prey parameters. Improvements in prey growth rate might benefit predators rather than prey (relating to paradox of pesticides, paradox of enrichment).

Iron fertilization experiments also illustrate these model predictions: a short bloom in phytoplankton is quickly consumed, mainly boosting predator density, limiting carbon sequestration.

## Applications to Economics and Marketing
The Lotka–Volterra model applies to economics and marketing,describing dynamics in markets with competitors, complementary platforms, a sharing economy, etc. In some cases, one competitor drives others out; in others, a stable equilibrium or cyclical/chaotic changes can occur.

## History
Alfred J. Lotka proposed the model in 1910 for autocatalytic chemical reactions, effectively the logistic equation originally derived by Verhulst.  
- In 1920, Lotka extended the model to organic systems. 
- In 1925, he analyzed predator–prey interactions. 
- In 1926, Vito Volterra published the same set of equations, inspired by observations of fish catches in the Adriatic Sea by Umberto D’Ancona.  
- This model later became known as the “Lotka–Volterra model.”

It was extended to include density-dependent prey growth and Holling’s functional response, termed the Rosenzweig–MacArthur model. In the late 1980s, the ratio dependent (Arditi–Ginzburg) model emerged. Lotka–Volterra equations have a long history in economic theory.

## Solutions to the Equations
The equations yield periodic solutions without a simple standard trigonometric expression, though they are tractable. One can absorb three of the four parameters into normalizations, leaving a single effective parameter. A linearization yields a solution resembling simple harmonic motion, with the predator population trailing that of prey by 90° in the cycle.

### A Simple Example
Suppose two species, rabbits (prey) and foxes (predator). With initial densities both at 10, and certain growth/death rates (rabbits at 1.1 / 0.4, foxes at 0.1 / 0.4), one can plot populations over time. One may also plot parametric solutions (prey vs. predator) without explicit time, forming closed curves.

$$
\frac{dy}{dx} = -\frac{y}{x} \; \frac{\delta x - \gamma}{\beta y - \alpha}
$$

Integration yields:

$$
\frac{\beta y - \alpha}{y}\, dy + \frac{\delta x - \gamma}{x}\, dx = 0
$$

giving an implicit relationship:

$$
V = \delta x - \gamma \ln(x) + \beta y - \alpha \ln(y).
$$

A known limitation is that some solutions allow prey populations to become extremely small yet recover. Real systems may go extinct if such numbers are too low (the “atto-fox problem”).

## Hamiltonian Structure
Because $V(x,y)$ is conserved, it serves as a Hamiltonian function.Defining:

$$
\{f,g\} = -xy \Bigl(\tfrac{\partial f}{\partial x}\tfrac{\partial g}{\partial y} - \tfrac{\partial f}{\partial y}\tfrac{\partial g}{\partial x}\Bigr)
$$

then Hamilton’s equations become:

$$
\dot{x} = \{x,V\} = \alpha x - \beta x y,\quad \dot{y} = \{y,V\} = \delta x y - \gamma y.
$$

Transformations $p = ln(x)$, $q = ln(y)$ lead to a canonical form of Hamilton’s equations with Hamiltonian

$$
H(q,p) = \delta e^{p} - \gamma p + \beta e^{q} - \alpha q.
$$

## Dynamics of the System
Predators thrive when prey is plentiful but then outstrip the supply and decline. With fewer predators, prey regain numbers. This cycle can continue indefinitely.

## Population Equilibrium
Equilibrium occurs when:

$$
x(\alpha - \beta y) = 0,\quad -\,y(\gamma - \delta x) = 0.
$$

Leading to two solutions:
1. $(x=0, y=0)$
2. $(x=γ/δ, y=α/β)$

The origin is a saddle point (unstable), and the non-zero fixed point can be a center of closed orbits, generating periodic oscillations.

## Further reading:  
• Hofbauer, Josef; Sigmund, Karl (1998). “Dynamical Systems and Lotka–Volterra Equations” …  
• Kaplan, Daniel; Glass, Leon (1995). Understanding Nonlinear Dynamics …  
• Leigh, E. R. (1968). “The ecological role of Volterra’s equations” …  
• Murray, J. D. (2003). Mathematical Biology I: An Introduction …  
• Stefano Allesina’s Community Ecology course notes: https://stefanoallesina.github.io/Theoretical_Community_Ecology/
