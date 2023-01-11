# Lecture 2: The Robertson Walker Metric
The first key discovery in modern cosmology was made by Hubble, when he realized that the universe was expanding and that the velocity at which galaxies were moving away from our point of view followed a linear relationship $v = Hd$ with respect to their distances. He also made the connection between these observations and theoretical predictions form relativistic cosmology.

# Hubble Expansion and Scale Factor $a(t)$
The first thing to mathematically describe an expanding universe is to create a system of coordinates that follows this behavior. If you imagine a grid that is expanding uniformly, then a change in scale would simply appear like you are zooming in or out of it. In other words, position vectors at a time $t$ are going to be equal to a scale factor $a(t)$ times a referece size at time $t_0$:

$$
x(t) = a(t) x(t_0)
$$
Notice that the scale factor $a$ can vary throughout time. Now, consider taking the derivative with respect to time:

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

This assumption can be thought of as the generalization of the **Copernican Principle**, which states that our place in the universe isn't special. Indeed, the Cosmological Principle gives rise to **fundamental observers**, which are those observers that percieve the univerese as isotropic. These fundamental observers imply a cosmological "rest frame" at each location in space, and this rest frame is defined to be the one that is co-moving with the Universe's expansion. *Another way of thinking about fundamental observers is that they are a kind of inertial frame of reference.*

A good example of the idea of *fundamental observers* is the observation of the CMB from Earth. Without any processing, the CMB looks like a big "yin-yang" dipole pattern of redshifted and blueshifted photons, and it's a consequence of Earth's peculiar velocity with respect to the fundamental observer at its location, caused by the Solar System's velocity as well as the Milky Way's.

## The Robertson-Walker Metric
In General Relativity, the geometry of the four-dimensional spacetime is influenced by the presence of mass within it. Every point in spacetime has a **metric** that describes the geometry at such point. It has been shown that to satisfy the Cosmological Principle, a metric that describes the universe must have the following form, in spherical polar coordinates:

$$
ds^2 = -c^2dt^2 + a^2(t) \big[dr^2 + S_k^2(r)\big( d\theta^2 + sin^2\theta d\phi^2 \big) \big]
$$

Known as the Robertson-Walker or Friedmann-Robertson-Walker metric. Using the definition of a solid angle, $d\Omega^2 = d\theta^2 + sin^2\theta d\phi^2$, we can rewrite the **FRW Metric** as (*always keep in mind that $d\Omega$ is two-dimensional*):

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

Here, the quantity $R_0$ is called the **radius of curvature** of the universe at the present epoch. Now, notice that if we do a change of variables $\rho = S_k(r)$, this metric can be expressed as:

$$
ds^2 = -c^2dt^2 + a^2(t) \bigg[ \frac{d\rho^2}{1-k(\rho/R_o)^2} + \rho^2d\Omega^2 \bigg]
$$

Where the last term in the brackets looks like what one gets in spherical coordinates using Euclidean space.

To understand a bit better, you should now that in GR, $ds^2$ is an invariant interval between two neighboring events in spacetime separated by $dx^\mu$, where each of the four possible $dx$ correspond to the four dimensions, with $\mu=0$ being time. In general cases, $ds^2$ can be written as:

$$
ds^2 = \sum_{\mu \nu} g_{\mu\nu}dx^\mu dx^\nu
$$

Where $g_{\mu\nu}$ is known as the metric tensor, which is described by a symmetric $N\times N$ matrix that expresses the notion of distance between different points in spacetime. Some things to consider about metrics:

- The metric determines the geodesics, which are the trajectories of free-falling objects.
- $ds^2 = 0$ determines how light moves across spacetime.
- Usually metrics are complicated, but that is not the case for a homogeneous and isotropic model of the universe.

## Building Intuation

Look at the notes for the entire explanation, but the main idea here is to try and visualize the FWR metric with lower dimensional analogs. Another important thing is that $k$ describes the geometry of the universe being modeled, with $k=-1$ corresponding to a hyperbolic space, $k=0$ corresponding to a flat space and $k=1$ to a spherical space. Observations show that $k=0$ to a high precision in our universe, so we will stick to this value for most of the course. 

# Proper Distance, Redshift, and Hubble Drag

## Proper Distance
In an expanding universe, the distance between two objects is increasing with time. We can define a proper distance $r_p$ as the *spacelike* distance (i.e. $dt=0$) between two points. If we assume a constant angle along the geodesic, then from the FRW metric we get:

$$
ds^2 = a^2(t)dr^2 \implies ds = a(t)dr
$$

Here, the proper distance $r_p$ is then the integral of the radial comoving coordinate $r$:

$$
r_p(t) = \int_0^r a(t)dr' = a(t)r
$$

Meaning that the comoving coordinate $r$ is independent of time (of course!), while the proper distance $r_p$ does change with time. We can now calculate the rate of change of the proper distance between two points in the following manner:

$$
v(t) = \dot{r}_p(t) = \dot{a}(t)r = \frac{\dot{a}(t)}{a(t)}r_p = H(t)r_p
$$

Where in the last two steps we've done something similar to the first section of these notes. That is not a coincidence, in fact it is pretty much the same result but now shown in terms of the metric. This relationship between the proper distance to a galaxy and its recession speed is known as the **Hubble Flow**.

## Light Propagation and Redshift
One important consequence from an expanding universe that matters to astronomers is that the light observed has been redshifted as it has traveled from its source to our detectors. We can express this redshift in terms of the comoving factor $a(t)$. First, consider a ray of light that travels along a null geodesic such that $ds^2=0$. Now imagine that the light is emitted at a time $t=t_{em}$ from a positon $r'=r$ and arrives at position $r'=0$ at time $t=t_{obs}$. Say we orient our coordinate system so that the angles are constant. Then, the FRW metric gives us:

$$
ds = 0 = - c dt + a(t)dr \implies \frac{cdt}{a(t)} = -dr
$$

We can integrate both sides and arrive at:

$$
\int_{t_{em}}^{t_{obs}} \frac{c}{a(t)}dt = - \int_r^0dr = r
$$

Now consider a second ray of light emitted slightly later at a time $t=t_{em} + \Delta t_{em}$ and observed at a time $t=t_{obs} + \Delta t_{obs}$. Since it is just slightly later, then the distance $r$ is pretty much the same, giving us:

$$
r = \int_{t_{em} + \Delta t_{em}}^{t_{obs} + \Delta t_{obs}} \frac{c}{a(t)}dt 
$$

We can manipulate the integral such that:

$$
\int_{t_{em} + \Delta t_{em}}^{t_{obs} + \Delta t_{obs}} \frac{c}{a(t)}dt = \int_{t_{em}}^{t_{obs}} \frac{c}{a(t)}dt - \int_{t_{em}}^{t_{em} + \Delta t_{em}} \frac{c}{a(t)}dt  + \int_{t_{obs}}^{t_{obs} + \Delta t_{obs}} \frac{c}{a(t)}dt 
$$
$$
\implies \approx \int_{t_{em}}^{t_{obs}} \frac{c}{a(t)}dt - \frac{c\Delta t_{em}}{a(t_{em})} + \frac{c\Delta t_{obs}}{a(t_{obs})}
$$

Combining the results for both rays of light, we are left with:

$$
r = \int_{t_{em}}^{t_{obs}} \frac{c}{a(t)}dt =  \int_{t_{em}}^{t_{obs}} \frac{c}{a(t)}dt - \frac{c\Delta t_{em}}{a(t_{em})} + \frac{c\Delta t_{obs}}{a(t_{obs})}
$$

Which implies:

$$
\Delta t_{obs} = \frac{a(t_{obs})}{a(t_{em})}\Delta t_{em}
$$

To relate this to wavelengths, imagine that the small time delay is equal to the time between crests in a single electromagnetic wave, such that $\Delta t_{em}$ is equal to the period of the emitted photon $T_{em}$. Since the period is related to the frequency and wavelength of the photon, $T_{em} = 1/\nu_{em} = \lambda_{em}/c$, and choosing $a(t_{obs}) = 1$ (the usual choice to normalize the scale factor at the present epoch), then our previous expression can be rewritten as:

$$
\lambda_{obs} = \frac{\lambda_{em}}{a(t_{em})} = (1+z)\lambda_{em}
$$

Where we have defined $a(t_{em}) \equiv 1/(1+z)$. 

## Peculiar Velocity and Hubble Drag
In reality, objects in the universe don't comove perfectly with the Hubble flow, and have **peculiar velocities** $v_{pec}$. Thus, the proper velocity of any object with respect to a fundamental observer is given by:

$$
\textbf{v}_p = \frac{d\textbf{r}_p}{dt} = \frac{d}{dt}\big[ a(t)\textbf{r(t)} \big]
$$

Using some results from previous sections, we can see that:

$$
\textbf{v}_p = \dot{a}(t)\textbf{r}(t) + a(t)\dot{\textbf{r}}(t) = \textbf{v}_{exp} + \textbf{v}_{pec}
$$

Which shouldn't be surprising. Notice that in this case $r$ did have a non-zero derivative since we are taking into account the presence of peculiar velocities. Now consider the situation from the following diagram:

![[images/lec2fig1.png]]

Here, we have a fundamental observer looking at an object X that moves with a peculiar velocity at time $t$ and a slightly different peculiar velocity at time $t+dt$. We can calculate the effect that the expanding universe has in the object's peculiar velocity by first realizing that the proper velocity $v_p$ must be the same from the fundamental fundamental observer's POV, since there are no forces acting on it from their perspective. That is, $v_p(t) = v_p(t+dt)$. Furthermore, at $t=0$, $v_p(t=0) = v_{pec}(t=0)$ since it is at the fundamental observer's position. 

However, at time $t + dt$, we have:

$$
v_p(t+dt) = v_{exp}(t+dt)+ v_{pec}(t+dt) = H(t+dt)dl + v_{pec}(t+dt) \approx H(t)v_{pec}(t)dt + v_{pec}(t+dt)
$$

Using our previous observation about the proper velocities at the different times, we have that: 

$$
v_{pec}(t+dt) - v_{pec}(t) = -H(t)v_{pec}(t)dt
$$

Reorganizing gives us:

$$
\frac{dv_{pec}}{dt} = -Hv_{pec}
$$

Which means that from the perspective of the fundamental observer, the peculiar velocity of the object decreases with time. This is known as the **Hubble Drag**. As seen on the lecture notes (*which are basically using the chain rule, the deffinition of the Hubble constant and integrating on both sides*), this result can be used to demonstrate that:

$$
v_{pec} \propto a^{-1}
$$

Using GR, this result extends to momentum: $p \propto a^{-1}$. 


### *DIDN'T GET TO COVER THIS DURING THE LAST LECTURE*
# Horizons
## Particle Horizon
## Event Horizon
