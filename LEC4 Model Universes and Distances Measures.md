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

# Model Universes

## Radiation Dominated

## Matter Dominated

## Lambda Dominated




