# Lecture 2: The Robertson Walker Metric
The first key discovery in modern cosmology was made by Hubble, when he realized that the universe was expanding and that the velocity at which galaxies were moving away from our point of view followed a linear relationship $v = Hd$ with respect to their distances. He also made the connection between these observations and theoretical predictions form relativistic cosmology.

# Hubble Expansion and Scale Factor $a(t)$
The first thing to mathematically describe an expanding universe is to create a system of coordinates that follows this behavior. If you imagine a grid that is expanding uniformly, then a change in scale would simply appear like you are zooming in or out of it. In other words, position vectors at a time $t$ are going to be equal to a scale factor $a(t)$ times a referece size at time $t_0$:

$$
x(t) = a(t) x(t_0)
$$
Notice that the scale facot $a$ can vary throughout time. Now, consider taking the derivative with respect to time:

$$
\dot{x}(t) = \dot{a}(t) x(t_0)
$$

Using our first expression, we can rewrite this as:

$$
\dot{x}(t) = \frac{\dot{a}(t)}{a(t)} x(t)
$$

As you can see, this is the same as Hubble's Law, meaning that:

$$
H \equiv \frac{\dot{a}(t)}{a(t)}
$$

This means that Hubble's constant can actually vary throughout time.

Lastly, we can show that the expansion looks the same from any point by looking at the expansion rate from two points $x_1$ and $x_2$ and looking at their difference:

$$
\dot{x}_2(t) - \dot{x}_1(t) = H(t) \big[ x_2 - x_1 \big] 
$$

# The Robsertson-Walkter Metric

## Assumptions
The main assumption used to create a mathematical framework for the standard model of cosmology is the **Cosmological Principle**, which states that at sufficiently large scales ($\sim 100Mpc$), the universe is spatially homogeneous and isotropic. In other words, we can consider the universe's contents to be an idealized, smooth fluid.

This assumption can be though of as the generalization of the **Copernican Principle**, which states that our place in the universe isn't special. Indeed, the Cosmological Principle gives rise to **fundamental observers**, which are those observers that percieve the univerese as isotropic. These fundamental observers imply a cosmological "rest frame" at each location in space, and this rest frame is defined to be the one that is co-moving with the Universe's expansion.

A good example of the idea of *fundamental observers* is the observation of the CMB from Earth. Without any processing, the CMB looks like a big "yin-yang" dipole pattern of redshifted and blueshifted photons, and its a consequence of Earth's peculiar velocity with respect to the fundamental observer at its location, caused by the Solar System's velocity as well as the Milky Way's.

## The Robertson-Walker Metric
In General Relativity, the geometry of the four-dimensional spacetime is influenced by the presence of mass within it. Every point in spacetime has a **metric** that describes the geometry at such point. It has been shown that to satisfy the Cosmological Principle, a metric that describes the universe must have the following form, in spherical polar coordinates:

$$
ds^2 = -c^2dt^2 + a^2(t) \big[dr^2 + S_k^2(r)\big( d\theta^2 + sin^2\theta d\phi^2 \big) \big]
$$

Known as the Robertson-Walker or Friedmann-Robertson-Walker metric. Using the definition of a solid angle, $d\Omega^2 = d\theta^2 + sin^2\theta d\phi^2$, we can rewrite the **FRW Metric** as:

$$
ds^2 = -c^2dt^2 + a^2(t) \big[ dr^2 + S_k^2(r) d\Omega^2 \big]
$$

Where $S_k(r)$ is defined by the **curvature constant** $k$:

$$
S_k(r) = R_0 sin(r/R_0) \hspace{0.6cm} \text{for} \hspace{0.2cm} k = 1
$$
$$
S_k(r) = r \hspace{0.6cm} \text{for} \hspace{0.2cm} k = 0
$$
$$
S_k(r) = R_0 sinh(r/R_0) \hspace{0.6cm} \text{for} \hspace{0.2cm} k = -1
$$

Here, the quantity $R_0$ is called the **radius of curvature** of the universe at the present epoch.

## Building Intuation

# Proper Distance, Redshift, and Hubble Drag
## Proper Distance
## Light Propagation and Redshift
## Peculiar Velocity and Hubble Drag

# Horizons
## Particle Horizon
## Event Horizon
