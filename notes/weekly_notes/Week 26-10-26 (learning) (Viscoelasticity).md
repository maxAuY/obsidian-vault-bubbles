>[!note] Standard Form of the Constitutive Equations of Linear Viscoelastic Models
> - The standard form for linear viscoelastic models is:
> $$\sigma + \tau_\sigma\dot\sigma = E_R\epsilon + E_R\tau_\epsilon \dot\epsilon$$
> where $\tau_\sigma$ is the relaxation time, $E_R$ is the relaxed modulus, and $\tau\epsilon$ is the retardation time.
> - These three parameters have physical significance in determining the response of the materials:
> 	- **Relaxed modulus**, $E_R$: the long-term equilibrium stiffness of the material. This is the stiffness of the material if you stretched it out to a constant strain and waited an infinitely long time.
> 	- **Relaxation time**, $\tau_\sigma$: the time taken for the internal stress to decay to $\frac{1}{e}$ (around $36.8\%$) of its peak value when the material is held at a constant strain.
> 	- **Retardation time**, $\tau_\epsilon$: the time taken for the material to rise to $1-\frac{1}{e}$ (around $63.2\%$) of its eventual creep deformation when it is held at a constant stress for infinite time.
> - Each linear model can be compared with the standard form to calculate each property.
> - These properties are summarised below:
> 
| Viscoelastic Model | Mechanical Component Layout | Relaxed Modulus ($E_R$) | Relaxation Time ($\tau_\sigma$) | Retardation Time ($\tau_\varepsilon$) | Long-Term Behavior |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Maxwell** | 1 Spring, 1 Dashpot (in **series**) | $0$ | $\frac{\eta}{E}$ | $\infty$ | Viscous liquid (flows forever under load) |
| **Kelvin-Voigt** | 1 Spring, 1 Dashpot (in **parallel**) | $E$ | $0$ | $\frac{\eta}{E}$ | Viscoelastic solid (delayed deformation to a cap) |
| **Zener (Maxwell form)** | 1 Spring parallel to a Maxwell arm | $E_1$ | $\frac{\eta}{E_2}$ | $\frac{\eta}{E_2} \left(1 + \frac{E_2}{E_1}\right)$ | Viscoelastic solid (instant response + relaxation) |
| **Zener (Kelvin form)** | 1 Spring in series with a Kelvin unit | $\frac{E_1 E_2}{E_1 + E_2}$ | $\frac{\eta}{E_1 + E_2}$ | $\frac{\eta}{E_2}$ | Viscoelastic solid (instant response + delayed creep) |

> [!note] Fractional Kelvin-Voigt
> - Fractional Kelvin-Voigt has the same setup as the Kelvin-Voigt model but swaps the dashpot for a springpot, a component which has both dissipative and energy-storing properties.
> - The constitutive equation for a springpot is:
> $$\sigma = c_\alpha\frac{d^\alpha\epsilon}{dt^\alpha}$$
> where $0<\alpha<1$ is the fractional order of the time derivative and $c_\alpha$ is the springpot material constant.
> - This model represents deformation history and can model complex behaviour with very few parameters.
> ---
> - Fractional Kelvin-Voigt is used to model soft tissues, biological cells, and shear wave attenuation in biological materials.
> ---
> - The constitutive equation is the same as Kelvin-Voigt but replaces the derivative with a fractional derivative:
> $$
> \sigma = E\epsilon + \eta \frac{d^\alpha\epsilon}{dt^\alpha}
> $$
> ---
> - The main advantage of using this model for soft tissues is that it can accurately model power-law creep and attenuation.
> - Attenuation in biological tissues can be modelled as follows:
> $$
> a_{k}(\omega) = a_{0}\omega^y
> $$
> where $a_{k}(\omega)$ is the imaginary part of the wave number, $k$, $a_0$ is the absorption coefficient, $\omega$ is the angular frequency, and $y$ is the power law exponent. 
> - For low $\omega\tau$, where $\tau$ is the characteristic relaxation time of the medium, the relationship between the power law exponent, $y$, and $\alpha$ is:
> $$
> y=\alpha+1
> $$
> - For high values of $\omega\tau$, the relationship changes to:
> $$
> y=1-\frac{\alpha}{2}
> $$

[![Schematic representation of the fractional Kelvin-Voigt model. | Download  Scientific Diagram](https://www.researchgate.net/publication/378952982/figure/fig2/AS:11431281229472141@1710454753806/Schematic-representation-of-the-fractional-Kelvin-Voigt-model.png)](https://www.google.com/url?sa=t&source=web&rct=j&url=https%3A%2F%2Fwww.researchgate.net%2Ffigure%2FSchematic-representation-of-the-fractional-Kelvin-Voigt-model_fig2_378952982&ved=0CBcQjRxqFwoTCPCQsOHW2pcDFQAAAAAdAAAAABA4&opi=89978449)

>[!note] Complex Dynamic Modulus
> - The complex dynamic modulus, $G$, is written:
> $$
> G^* = G' + iG''
> $$
> where $G'$ is the elastic modulus, measuring the energy stored by the material, and G'' is the loss modulus, measuring the energy dissipated.
> - This is useful for modelling sinusoidal inputs where the stress will lag behind the strain by a phase angle, $\delta$.
> 	- When the material is purely elastic, the stress and strain are in phase $(\delta = 0\text{\textdegree})$.
> 	- When the material is purely viscous, the stress lags behind by $(\delta = 90\text{\textdegree})$.
> 	- Viscoelastic materials sit in between with $0\text{\textdegree} < \delta <90\text{\textdegree}$
> - A generalised Hooke's law for dynamic testing can be written:
> $$
> \sigma = G^*\epsilon
> $$
> where $\sigma$ and $\epsilon$ are written as complex numbers in the frequency domain. 
> ---
> - The absolute modulus represents the overall stiffness to dynamic deformation and is written:
> $$
> \lvert{G*}\rvert = \sqrt{(G')^2+(G'')^2}
> $$
> - The loss factor is the ratio between the energy lost and energy stored at a given frequency and is written:
> $$
> \tan{\delta} = \frac{G''}{G'}
> $$
