> [!note] Flow in a Fluid Element
> - We consider a fluid element in the shape of a cube with dimensions $dx$, $dy$, and $dz$ to align with cartesian coordinate system $(x,y,z)$.
> - The inflow rate into the cube in the $x$ direction is equal to the product of the fluid velocity in the $x$ direction, $u$, and the cross-sectional area, $dy\,dz$:
> $$Q_{\mathrm{in},x} =  u\,dy\,dz \tag{1}$$
> - Using the first-order Taylor expansion, the outflow rate in the x-direction is equal to:
> $$Q_{\mathrm{out},x} = u\,dy\,dz + \frac{\partial u}{\partial x}\,dx\,dy\,dz \tag{2}$$
> - The net flow rate is equal to:
> $$\Delta Q_{x} = Q_{\mathrm{out},x}-Q_{\mathrm{in},x} = \frac{\partial u}{\partial x}\,dx\,dy\,dz \tag{3}$$
> - In 3D, the net volumetric flow out of the fluid element becomes:
> $$\Delta Q = \nabla \cdot \mathbf{V}\,dx\,dy\,dz \tag{4}$$
> where $\mathbf{V}(x,y,z)=(u,v,w)$ is the velocity vector of the fluid.

> [!note] Conservation of Mass
> - The mass contained inside a fluid element is equal to its density multiplied by its volume:
>   $$m = \rho \,dx\,dy\,dz \tag{1}$$
> - For unsteady flow, the rate at which mass accumulates inside the fixed control volume is:
>   $$\frac{\partial m}{\partial t} = \frac{\partial \rho}{\partial t}\,dx\,dy\,dz \tag{2}$$
> - By the principle of conservation of mass, any mass accumulation must be balanced by the net mass flow rate entering or leaving across the boundaries:
>   $$\frac{\partial m}{\partial t} = \frac{\partial \rho}{\partial t}\,dx\,dy\,dz = - \boldsymbol{\nabla} \cdot (\rho\mathbf{V})\,dx\,dy\,dz$$
> - Dividing through by the element volume ($dx\,dy\,dz$) yields the differential continuity equation:
>   $$\frac{\partial \rho}{\partial t} + \boldsymbol{\nabla} \cdot (\rho\mathbf{V}) = 0 \tag{3}$$

> [!note] Conservation of Momentum
> - Navier-Stokes extends conservation of momentum to a 3d fluid.

>[!note] Boundary Layers
> - A boundary layer is a section near a surface where the velocity of a fluid slows down. It can have laminar and turbulent sections.
> - The layer is typically modelled with a no-slip condition where the velocity of the fluid is zero at the wall.
> - There will always be a viscous sub-layer where the flow is laminar and viscosity and friction dominate.

> [!note] The wave equation
> -



>[!note] Viscosity
> -

>[!note] Surface Tension
> -



>[!note] Rayleigh Plesset
> -

