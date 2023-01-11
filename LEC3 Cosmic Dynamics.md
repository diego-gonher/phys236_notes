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

# The Fluid Equation

# Equations of State and Energy Density Evolution
## Matter
## Radiation
## Dark Energy


# The Friedmann Equation in terms of $\Omega$s