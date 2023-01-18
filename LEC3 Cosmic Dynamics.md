# Lecture 3: Cosmic Dynamics
Now that we have an appropiate metric, we can start exploring how the mass-energy content of the universe dictates how spacetime evolves. In classical mechanics, one can use *Poisson's Equation* to describe the Newtonian dynamics:

$$
\nabla^2 \Phi = 4 \pi G \rho
$$

Which relates the gravitational potential to the density in a space. In GR, the equivalent is *Einstein's Field Equation*:

$$
G_{\mu \nu} = \frac{8\pi G}{c^4} T_{\mu \nu}
$$

Where $G_{\mu \nu}$ is the **Einstein Tensor** (a symmetric $4 \times 4$ tensor that depends on the derivatives of the $g_{\mu \nu}$ metric), and $T_{\mu \nu}$ is the **stress-energy tensor** (which depends on the energy density and momentum and how they flow). Though simple looking, Einstein's Field equation actually represents a system of ten nonlinear second-order differential equations. As you might expect, finding solutions to this is quite complicated, but useful, since in GR the energy contents of any location tells spacetime how to curve, and such curvature tells the energy contents how to move.

Fortunately for us, the Cosmological Principle simplify the problem. For that, we are gonna use the FRW metric that we explored in [[LEC2 FRW metric]].

# The Friedmann Equation
The equation of motion for our scaling factor $a(t)$ is known as the **Friedmann Equation**, which we can derive in a semi-classical fashion. Start with a homogeneous and isotropic universe, and imagine a small spherical region of radius $R$ that encloses a mass $M$. Classically, we know that:

$$
\ddot{R} = -\frac{GM}{R^2}
$$

Consequently, the energy $E$ of this test particle is given by:

$$
\frac{1}{2}\dot{R}^2 - \frac{GM}{R} = E
$$

We can now substitute the mass using $M = 4\pi \rho(t) R(t)^3 / 3$, noting that both the density and the radius of the sphere vary with time. This gives us:

$$
\frac{1}{2}\dot{R}^2 - \frac{4 \pi G \rho R^2}{3} = E
$$

Now, we can define $R = a(t)R_0$ such that there is a Hubble Law of the form:

$$
\dot{R} = \bigg( \frac{\dot{a}}{a} \bigg) R
$$

Solving for $\dot{a}/a$ here, replacing for $\dot{R}^2$ using the energy equation and squaring it gives us:

$$
\bigg( \frac{\dot{a}}{a} \bigg)^2 = \bigg( \frac{\dot{R}}{R} \bigg)^2 = \frac{8 \pi G \rho}{3} + \frac{2E}{R^2} = \frac{8 \pi G \rho}{3} + \frac{2E}{R_0^2a^2}
$$

Lastly, we can define a new constant (related to the curvature constant in the FRW metric):

$$
k = -\frac{2E}{c^2} \implies 2E = -kc^2
$$

And we are left with Friedmann's Equation:

$$
\bigg( \frac{\dot{a}}{a} \bigg)^2 = \frac{8 \pi G \rho}{3} - \frac{kc^2}{R_0^2a^2}
$$

This equation is great, as it allows us to describe the expansion of the universe. A derivation using GR gives us the exact same expression. However, there are two relevant differences between the two derivations.

First, a full GR treatment gives us a different expression for the acceleration of the test particle:

$$
\ddot{R} = -\frac{4 \pi G}{3}R\bigg( \rho + \frac{3P}{c^2} \bigg)
$$

Where the term in parenthesis is very important, as $\rho$ is taken to be the energy density of anything (that includes mass energy, radiation and vacuum energy), which implies the need of an ecuation of state $P(\rho)$ for each component if we want to solve for the universe's dynamics. 

The second difference is that the solution that uses GR constrains the value for the curvature $k$ to only $\pm 1, 0$, and is determined by the mass energy contents of the universe. This constrain, which has a deep impact on cosmology, cannot be captured in a semi-classical framework of the problem. 

To understand the physical implications of this, it is useful to define a critical density $\rho_c$ and a density parameter $\Omega(t)$:

$$
\rho_c = \frac{3H^2(t)}{8 \pi G}
$$
$$
\Omega(t) = \frac{\rho}{\rho_c}
$$

Which allows us to rewrite and rearrange Friedmann's Equation to be:

$$
k = [\Omega(t) - 1] \bigg( \frac{R_0 a^2(t)}{cH^{-1}(t)} \bigg)^2
$$

Clearly, the curvature is related to the energy contents, with the three possibilites being:

- **Spatially Open**: if $\Omega(t) < 1$ then $k<0$ and the universe has a negative curvature.
- **Spatially Closed**: if $\Omega(t) > 1$ then $k>0$ and the universe has a positive curvature.
- **Spatially Flat**: if $\Omega(t) = 1$ then $k=0$ and the universe has a flat curvature.

The current measurements of the density parameter indicate that $\Omega_0 = 0.999 \pm 0.002$, meaning that our universe is flat, which means that we get to focus on the simplest form of the FRW metric.

# The Fluid Equation
The Friedmann Equation encapsulates the idea of energy conservation in an expanding universe. Now let us consider another classical manifestation of energy conservation, the first law of thermodynamics:

$$
dQ = TdS = dU + PdV
$$

Where $dQ$ is the heat flow, $U$ is the internal energy, $P$ is the pressure, and $dV$ is the change in volume. The Cosmological Principle requires that $dQ = 0$. Over a differential of time $dt$, this means that:

$$
\dot{U} + P\dot{V} = 0
$$

Now, we want to find proper expressions for the time derivatives of the internal energy and the volume. For that, consider a shpere of comoving radius $r_c$ expanding with the universal Hubble flow, such that its proper radius is $r_p = a(t)r_c$. Then, its volume would be:

$$
V(t) = \frac{4\pi}{3} r_c^3 a^3(t) \implies \dot{V} = \frac{4\pi}{3} r_c^3 [3 a(t) a^2(t)] = V\bigg(3\frac{\dot{a}}{a} \bigg)
$$

As for the internal energy $U$:

$$
U = V \rho(t) c^2 \implies \dot{U} = c^2[V \dot{\rho}(t) + \dot{V}\rho(t)] = c^2V\bigg( \dot{\rho} + 3\rho \frac{\dot{a}}{a} \bigg)
$$

Using these two, our result from the first law of thermodynamics becomes:

$$
\dot{\rho} + 3\frac{\dot{a}}{a}\bigg(\rho + \frac{P}{c^2} \bigg) = 0
$$

Which is known as the **Fluid Equation** or the **Continuity Equation**. The Fluid Equation and the Friedmann Equation together are used for describing the expansion of the Universe. One can physically interpret this equation as providing a type of "energy conservation" in the cosmological context.

We can now try to derive an expression for $\ddot{a}$, that is, an expression for the acceleration of the Universe's expansion. To do that, start with Friedmann's Equation and multiply it by $a^2$:

$$
\dot{a}^2 = \frac{8 \pi G \rho a^2}{3} - \frac{kc^2}{R_0^2}
$$

Now take the time derivative:

$$
2\dot{a}\ddot{a} = \frac{8\pi G}{3}(\dot{\rho}a^2 + 2\dot{a}a\rho)
$$

Divide by $2\dot{a}{a}$

$$
\frac{\ddot{a}}{a} = \frac{4\pi G}{3} \bigg( \dot{\rho} \frac{a}{\dot{a}} + 2\rho \bigg)
$$

Using the Fluid Equation to substitute for the fraction within the parenthesis, finally yields:

$$
\frac{\ddot{a}}{a} = -\frac{4\pi G}{3}\bigg( \rho + \frac{3P}{c^2} \bigg)
$$

Which is known as the **Acceleration Equation**, and shows that pressure and energy (density) are the sources of gravitational acceleration.

# Equations of State and Energy Density Evolution

So far, we have three equations:

- Friedmann Equation

$$
\bigg( \frac{\dot{a}}{a} \bigg)^2 = \frac{8 \pi G \rho}{3} - \frac{kc^2}{R_0^2a^2}
$$
- Fluid Equation

$$
\dot{\rho} + 3\frac{\dot{a}}{a}\bigg(\rho + \frac{P}{c^2} \bigg) = 0
$$
- Acceleration Equation

$$
\frac{\ddot{a}}{a} = -\frac{4\pi G}{3}\bigg( \rho + \frac{3P}{c^2} \bigg)
$$

Out of which, only the first two are independent (we used them to derive the third one). However, we have three unkowns: $a(t)$, $\rho(t)$, and $P(t)$, which means we need another piece of information before we are able to solve this problem. 

Specifially, what we need is a function of the pressure in terms of the density $P(\rho)$, where the relationship is determined by the energy contents of the universe. As it turns out, only three components are important: matter, radiation and dark energy. Thus, we can write the total energy density as:

$$
\rho c^2 = \text{matter} + \text{radiation} + \text{dark energy}
$$
$$
\implies \rho c^2 = \rho_{m}(c^2 + \epsilon) + \frac{4\sigma_{SB}}{c}T^4 + \rho_{da}
$$

Where $\epsilon = 3k_{b}T_{m}/(2m)$ is the internal energy of the matter per unit mass (in this case for a monoatomic ideal gas). The pressure associated with these energy components is expressed as **an equation of state**. Since we are only dealing with dilute gases in cosmology, these equations of state always take the linear form:

$$
P(\rho) = w\rho c^2
$$

Where $w$ is a dimensionless number. Using this in the Fluid Equation gives us:

$$
\dot{\rho} + 3\frac{\dot{a}}{a}\bigg(\rho + \frac{w\rho c^2}{c^2} \bigg) = \dot{\rho} + 3\frac{\dot{a}}{a}\big(\rho + w\rho \big) = 0
$$
$$
\implies \frac{\dot{\rho}}{\rho} = -3(1+w)\frac{\dot{a}}{a}
$$

Assuming that $w$ is constant, then this gives us the following solution:

$$
\rho = \rho_0a^{-3(1+w)}
$$

Where $\rho_0$ is the density at the present epoch ($a_0=1$). Now we can consider each of the three main components with more detail.

## Matter
We can approximate the universe to be an ideal gas consisting of $N$ particles of mass $m$ such that:

$$
P_mV = Nk_bT
$$
$$
\rho_m = \frac{mN}{V}
$$
$$
\implies P_m = \frac{k_b T}{m} \rho_m
$$

While it might be tempting to think that because of this $w = k_bT/m$, in reality this isn't quite the answer, because $\rho_m \neq \rho$. To actually get a correct expression, we have to recall that for an ideal gas:

$$
P_m = (\gamma-1)\rho_m\epsilon
$$

Where $\gamma=5/3$ for a monoatomic ideal gas. Now, to take into account that the rest-mass energy doesn't contribute to the gas pressure, we can write the pressure as:

$$
P_m = (\gamma - 1)(\rho c^2 - \rho_m c^2)
$$

Using this and our first expression for $P_m$ leaves us with:

$$
P_m = \frac{k_B T}{m c^2}\bigg(1 + \frac{1}{\gamma - 1}\frac{k_BT}{mc^2}  \bigg)^{-1}\rho c
$$
$$
\implies w(T) = \frac{k_B T}{m c^2}\bigg(1 + \frac{1}{\gamma - 1}\frac{k_BT}{mc^2}  \bigg)^{-1}
$$

Since $k_BT \ll mc^2$ for a non-relativistic gas, we can conclude that $w\ll1$. In fact, we can consider the matter to be a **dust fluid**, with:

$$
w_{\text{matter}} = 0
$$

## Radiation
We can approximate the radiation's energy density as arising from an ultra-relativistic fluid of particles, for which:

$$
P = \frac{\rho c^2}{3}
$$
$$
\implies w_{\text{radiation}} = \frac{1}{3}
$$

## Dark Energy
Classically, vacuum doesn't have energy. However, quantum fluctuations form particle-antiparticle pairs can create an energy density, which in the case of dark energy, is given by:

$$
P =-\rho c^2
$$
$$
\implies w_{\text{dark energy}} = -1
$$

An interesting result of this is that, if we plug this into the acceleration equation, we get:

$$
\frac{\ddot{a}}{a} = \frac{8\pi G}{3} \rho_{\text{vac}}
$$

Which means that dark energy acts as a type of *anti-gravity*, accelerating the expansion of the universe.

## Summary
Here you can see a summary of the three main components in the universe. The rest of the columns were derived using:

- **Density**: was derived using the relationship between density and $a$ from earlier in these notes.
- **Pressure**: equation of state for each thing, the linearized version I believe.
- **Temperature**: using ideal gas temperature for matter, and black body radiation for radiation.


| Component      | $w$ | $\rho$ | $P$ | $T$ |
|     :----:     |   :----:   |   :----:   |    :----:   |    :----:   |
| matter      | 0 | $a^{-3}$ | $a^{-5}$ | $a^{-2}$ |
| radiation   | 1/3 | $a^{-4}$ | $a^{-4}$ | $a^{-1}$ |
| vacuum energy   | -1 | $a^{0}$ | $a^{0}$ | |


# The Friedmann Equation in terms of $\Omega$s
With the new concepts that we developed in the past section, we can rewrite the Friedmann Equation as the following:

$$
H^2(t) = \bigg( \frac{\dot{a}}{a} \bigg)^2 = \frac{8\pi G}{3} \big[ \rho_{m,0}a^{-3} + \rho_{r,0}a^{-4} + \rho_{A,0} \big] - \frac{kc^2}{R_0a^2}
$$

Where the subscript refers to each of the three main components and the denisities are evaluated at the present epoch. 

### THERE IS OTHER WAYS OF EXPRESSING ALL OF THIS WITH MORE OMEGAS AND STUFF, LOOK INTO THE ACTUAL LECTURE NOTES