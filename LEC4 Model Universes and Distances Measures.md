# Lecture 4: Model Universes and Distances Measures
The main idea of this lecture is to see ways of determining the densities of the different components in the energy budget of the universe, and how these determine the expansion rate of the universe (which we can do to first order by exploring models with only one of these components). On the second part, we explore different distance definitions that can be used meaningfully in an expanding universe.

# Densities at Present
From [[LEC3 Cosmic Dynamics]], we learned that the Friedmann Equation can be expressed as:

$$
H^2(z) = H_0^2[\Omega_{m,0}a^{-3} + \Omega_{r,0}a^{-4} + \Omega_{\Lambda} + \Omega_{k,0}a^{-2}]
$$

Where each density parameter $\Omega$ is the ratio of the density of each component $\rho$ with respect to the critical density $\rho_c$ (the density required for a flat universe). Since the universe is seen to be flat, $\Omega_{k,0} = 0$, its easy to see that:

$$
\Omega_{m,0} + \Omega_{r,0} + \Omega_\Lambda = 1
$$

From observations, it has been measured that the energy budget of the universe is as follows:

$$
\Omega_\Lambda \approx 0.7
$$
$$
\Omega_{r,0} \approx 0.3
$$
$$
\Omega_{r,0} \approx 10^{-5}
$$

We can now explore each component with a little more detail.

## Radiation
To be more precise, this component considers not only photons, but any relativistic particles (such as neutrinos). As we just saw, this component is basically negligible at present time, at it is currently dominated by the CMB. To a high accuracy, the CMB is a black body with a temperature $T = 2.73 K$. Thus, we can get a value for the current density $\rho_{\gamma, 0}$ using the BB radiation field:

$$
\rho_\gamma c^2 = \frac{4\sigma_{SB}T^4}{c} \implies \rho_{\gamma, 0} \approx 5.1 \times10^{-5}
$$

However, as we just stated, photons aren't the only particles that contribute to this component. Radiation from starlight is in total about an order of magnitude less than the CMB, so we don't need to take it into account. Neutrinos, however, are relevant. Just like the CMB occured after the universe stopped being opaque for photons, there is an equivalent event at a higher redshift in which the universe stopped being opaque for neutrinos, allowing for the neutrino decoupling and causing an equivalent background of relic cosmic neutrinos that we can treat as "radiation" since their mass is small enough to remain relativistic. As we'll see in [[LEC5-7 Thermal History]], one can derive a relationship between the temperature of these relic neutrinos and the temperature of the CMB, which can then be used to calculate the corersponding energy density $\rho_\nu$, which ends up being relevant, allowing us to finally find that:

$$
\rho_{r,0} = 7.8 \times 10^{-34} g \hspace{0.1cm}cm^{-3} \implies \Omega_{r,0} = 8.6 \times 10^{-5}
$$

## Matter Radiation Equality
Even though at present time $\Omega_{r,0} \ll \Omega_{m,0}$ is the case, we would expect a time in which radiation dominated over matter given how their densities scale with the expansion of the universe ($\propto a^{-4}$ and $\propto a^{-3}$ respectively). We can actually determine the redshift at which the transition from radiation-dominated to matter-dominated occurred by doing:

$$
\rho_{m,0}a^{-3} = \rho_{r,0}a^{-4} \implies a_{eq} = \frac{1}{1+z_{eq}} = \frac{\rho_{r,0}}{\rho_{m,0}} = \frac{\Omega_{r,0}}{\Omega_{m,0}}
$$

Which, using current values, gives:

$$
z_{eq} \approx 3400
$$

## Coincidence Problem
Since currently the universe is dominated by the dark energy, we can similarly calculate the redshift at which the transition from the matter-dominated universe occurred:

$$
\rho_{m,0}a^{-3} = \rho_\Lambda
$$

Following a similar procedure, we can estimate the redshift of this transition to be:

$$
z_{m\Lambda} \approx 0.33
$$

Since this is very recent, some have argued that it is a little suspicious, and this is known as the **Coincidence Problem**, though not a lot of astronomers give it much of a thoght.

Here are a couple of plots that illustrate the transitions from radiation-dominated to matter-dominated and then from matter-dominated to dark energy-dominated:

![Lec2Fig1](images/lec4fig1.png)

# Model Universes
If you want to correctly model the expansion of the universe, we clearly have to consider the solutions for the Friedmann Equation using all the relevant components of universe's energy budget. Nevertheless, it is useful to consider simple models of flat universes with only one of the three most important components, as their solutions are analytic and easier to understand.

Remember from [[LEC3 Cosmic Dynamics]] that considering linear equations of state parametrized by variable $w$, the density $\rho_X$ of a single substance $X$ scales as:

$$
\rho_X \propto a^{-3(1+w)}
$$

Using the Friedmann Equation at the start of these notes, we find that the expansion of this single-component universe simplifies to:

$$
H^2(a) = \bigg( \frac{\dot{a}}{a} \bigg)^2 = H_0^2 \Omega_{X,0} a^{-3(1+w)}
$$
$$
\implies \dot{a}^2 = H_0^2\Omega_{X,0}a^{-(1+3w)}
$$

To solve this equation, we assume a power law such that:

$$
a(t) = \bigg( \frac{t}{t_0} \bigg)^q, \hspace{0.5cm} q = \frac{2}{2+3w}
$$

Where $t_0$ is a constant that depends on $w$ and $\rho_{X,0}$. We can use this to understand some of these simple model universes.

## Radiation Dominated
Using $w=1/2$, we get that:

$$
a(t) \propto t^{1/2}
$$

This is valid for $z\ll z_{eq}$.

## Matter Dominated
For matter, $w=0$, and thus:

$$
a(t) \propto t^{2/3}
$$

This is valid for $z_{eq} \ll z$ and $z\ll z_{m\Lambda}$.

## Lambda Dominated
For dark energy, we need a more careful approach. Since $w=-1$, the Friedmann Equation becomes:

$$
\bigg( \frac{\dot{a}}{a} \bigg)^2 = H_0^2 \Omega_{\Lambda,0}
$$

Which can be solved without the need of a power law. In this case, we get that:

$$
a(t) = a_0 e^{H_0\Omega_{\Lambda,0}^{1/2}(t-t_0)}
$$

Which shows that the expansion of the universe is accelerating exponentially.

# Distance Measures in Cosmology
Measuring distance and time can be a little tricky in an expanding universe, so here are some measures that are typically used in cosmology.

## The Line-of-Sight Comoving Distance
Remember that one can relate a differential of proper distance $\delta r_p$ (actual physical distance you would measure) to a comoving distance $\delta r$ (a distance that is defined with the expansion factor) with the following expression:

$$
\delta r = \frac{\delta r_p}{a(t_e)} = (1+z_e) \delta r_p
$$

The total line-of-sight comoving distance is defined as integrating all these small differentials $\delta r$ between closeby events, between the object of emission and the observer. In other words, it is integrating along the null geodesic ($ds^2=0$), which from the FRW metric is:

$$
d_c = \int dr = \int_{t_e}^{t_0} \frac{cdt}{a(t)}
$$

Using the chain rule, we can rewrite $dt/a(t)$ and find the following:

$$
d_c = c\int_0^z \frac{dz'}{H(z')} = d_H \int_0^z \frac{dz'}{E(z')} 
$$

Where $d_H$ is the Hubble distance, and $E(z)$ is defined as before in this lecture. **Note that the line-of-sight distance is not directly observable, but it is useful to define some of the other measures that we'll explore**.

## Angular Diameter Distance

## Luminosity Distance

## Lookback Time

## Comoving Volume



