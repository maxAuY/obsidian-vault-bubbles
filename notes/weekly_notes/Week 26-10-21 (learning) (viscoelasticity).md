>[!note] Viscoelastic Materials
> - A viscoelastic material is a substance that combines elastic and viscous properties. 
> - Viscoelastic materials store energy like a spring and dissipate some energy like a dashpot.
> - There are four core behaviours:
> 	- **Time and rate dependence**: materials will act differently depending on the rate of loading. Fast loading induces elastic behaviour and slow loading makes it flow like a liquid.
> 	- **Creep**: the material continues to deform at constant stress.
> 	- **Stress relaxation**: the stresses drop over time at a constant strain.
> 	- **Hysteresis**: hysteresis is caused by the above behaviours as well as heat dissipation during loading and unloading.
> - Polymers such as rubber, nylon, and plastics are viscoelastic.
> - Biological tissues are also viscoelastic.

>[!NOTE] Springs and Dampers
> - Springs and dampers are modelled as linear components when modelling linear viscoelastic materials.
> - Constitutive equations for **springs**: 
> $$\sigma=E\epsilon$$
> where $\sigma$ is the stress in the material, $\epsilon$ is the strain, and $E$ is the Young's modulus.
> - Constitutive equation for **dampers**: 
> $$\sigma=\eta\dot{\epsilon}$$
> where $\eta$ is the damping coefficient.

>[!note] Components in Parallel
> - The total displacement or velocity, $d$, is the same as the displacement of each component:
> $$d_T = d_1 = d_2 = ... = d_n$$
> - The total force is equal to the sum of forces in each component:
> $$F_T = F_1 + F_2 + ... + F_n$$
> - The effective spring or damping constant, $K$, is equal to the sum of the separate constants:
> $$K_e = K_1 + K_2 + ... + K_n$$
> - The total response is the response of the component with the highest force?

>[!note] Springs in Series
> - The total displacement or velocity, $d$, is the sum of the displacements or velocities of each component:
> $$d_T = d_1 + d_2 + ... + d_n$$
> - The total force is the same across each component:
> $$F_T = F_1 = F_2 = ... = F_n$$
> - The reciprocal of the effective spring or damping constant, $K$, is equal to the sum of the reciprocals of the separate constants:
> $$\frac{1}{K_e} = \frac{1}{K_1} + \frac{1}{K_2} + ... + \frac{1}{K_n}$$
> - The total response is equal to the sum of responses of each separate component.

>[!note] Maxwell Model
> - The Maxwell model consists of a spring and a damper in series.
> - Materials modelled this way are called **Maxwell bodies**.
> - This model captures an initial displacement from the spring and a displacement over time from the damper.
> - The material will only partially recover when the force is removed.
> - This model captures **stress relaxation** but doesn't accurately model **creep**.
> ---
> - This behaviour is seen in thermoplastic polymers near their melting point, biological tissue, and fresh concrete.
> - The model is used most often for viscoelastic fluids.
> ---
> - Written in terms of stress, $\sigma$, and strain $\epsilon$, the constitutive relation is:
> $$\sigma + \frac{\eta}{E}\dot{\sigma}=\eta \dot{\epsilon}$$
> where $\eta$ is the damping coefficient of the dashpot and $E$ is the spring constant.
> - This is derived by equating the total strain, $\epsilon$, to the sum of the strains in each component.
> $$
> \dot\epsilon = \dot\epsilon_\mathrm{damper} + \dot\epsilon_\mathrm{spring} \\
> \dot\epsilon = \frac{\sigma}{\eta} + \frac{\dot\sigma}{E} \\
> \sigma + \frac{\eta}{E}\dot{\sigma}=\eta \dot{\epsilon}
> $$

**Diagram of Maxwell model:**
![[Pasted image 20261021171312.png|533]]

**Output of Maxwell model for a step input and release:**
![[Pasted image 20261022154747.png|433]]

>[!note] Kelvin-Voigt Model
> - The Kelvin-Voigt model consists of a spring and a damper in parallel.
> - Materials modelled this way are called Voigt bodies.
> - The response is smoother than in a Maxwell body and the body will return to its initial state once the force has been removed.
> - This model is good for modelling **creep** in materials but does not accurately model **stress relaxation**.
> ---
> - This can be used to model fluid-filled elastic shells, organic polymers, rubber, and wood at low loads.
> - This model is used most often to model viscoelastic solids.
> ---
> - The constitutive relation is written:
> $$\sigma = E\epsilon + \eta \dot{\epsilon}$$
> - This is derived by equating the total stress, $\sigma$, to the stresses in each component.

**Diagram of Kelvin-Voigt model:**
![[Pasted image 20261022175900.png|379]]

**Output of Kelvin-Voigt model for a step input and release:**
![[Pasted image 20261022155119.png|444]]

>[!note] Standard Linear Model (Voigt Representation)
> - The Voigt representation of the standard linear model consists of a Voigt body in series with a spring.
> - This is also known as the Zener model.
> - In response to a step input, there is a sudden displacement followed by an exponential decrease in strain.
> - This is the simplest model that predicts both **creep** and **stress relaxation** accurately.
> - It predicts material responses better than the Maxwell and Kelven-Voigt representations.
> ---
> - This is used to model materials that have exhibit elastic recovery.
> - Examples include rubbers, elastomers, polymers, and biological tissue.
> ---
> - The constitutive equation is written:
> $$
> \sigma + \frac{\eta}{E_1 + E_2}\dot\sigma = \frac{E_1E_2}{E_1+E_2}\epsilon + \frac{E_1\eta}{E_1 + E_2}\dot\epsilon
> $$
> - This is derived ... somehow?
> $$
> \sigma = E_2\epsilon_{kv} + \eta\dot\epsilon_{kv} = E_1\epsilon_s \tag{1} $$
> $$
> \epsilon = \epsilon_{kv} + \epsilon_s \tag{2}
> $$
> $$
> \epsilon_s = \frac{\sigma}{E_1} \tag{3}
> $$
> Substituting Eq. 2 into Eq. 1:
> $$
> E_2 (\epsilon - \epsilon_s) + \eta (\dot\epsilon - \dot\epsilon_s) = E_1 \epsilon_s
> $$
> $$
> E_2 \epsilon + \eta\dot\epsilon = (E_1 + E_2) \epsilon_s + \eta\dot\epsilon_s \tag{4}
> $$
> Substituting Eq. 3 into Eq. 4:
> $$
> E_2 \epsilon + \eta\dot\epsilon = (E_1 + E_2) \frac{\sigma}{E_1} + \eta \frac{\dot\sigma}{E_1}
> $$
> $$
> \frac{E_1E_2}{E_1+E_2}\epsilon + \frac{E_1\eta}{E_1 + E_2}\dot\epsilon = \sigma + \frac{\eta}{E_1 + E_2}\dot\sigma
> $$

**Diagram of Zener model:**
![[Pasted image 20261022173353.png|370]]

**Output of Zener model for step input:**
![[Pasted image 20261022175224.png|418]]