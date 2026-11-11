> [!note] The Material Derivative
>  - The material derivative (also known as the Lagrangian derivative) tracks the change of a property in a single particle along its streamline.
>  - This is contrasted by the Eulerian derivative which tracks the change of a property at a fixed point in space.
>  - They can be equated as follows:
>  $$\frac{D}{Dt} = \frac{\partial}{\partial t} + \mathbf{u} \cdot \nabla$$
>  where the LHS is the material derivative and the RHS is the Eulerian derivative.

>[!note] Extensive and Intensive Properties
> - An extensive property, $B$, is a property that changes depending on the amount of material present.
> - An intensive property, $b = \frac{B}{m}$, is a property that does not change depending on how much of the material is present.

>[!note] Reynolds Transport Theorem
> - The material derivative can be written for an **extensive** property, $\mathbf{f} = \mathbf{f}(\mathbf{x},t)$ within a control volume, $\Omega$, bounded by $\partial \Omega$.
> - This is written as:
> $$
> \frac{d}{dt} \int_{\Omega(t)}{\mathbf{f}\,dV} = \int_{\Omega(t)}{\frac{\partial\mathbf{f}}{\partial t}\,dV} + \int_{\partial\Omega(t)}{(\mathbf{v}_{b}\cdot\mathbf{n})\,\mathbf{f}\,dA}
> $$
> where $\mathbf{v}_b$ is the volume of the geometric boundary and $\mathbf{n}$ is the normal vector to the boundary. 

>[!note] Continuity Equations
> - Continuity equations (conservation laws) state that the rate of change of an integrated property, $\psi$, defined over a fixed control volume, $\Omega$, must be equal to the rate that it is lost or gained at the boundaries, $\Gamma$, plus the rate it is created or consumed by sources or sinks within the control volume.
> - This is expressed with the equation:
> $$
> \frac{d}{dt}\int_{\Omega}{\psi\,d\Omega} = -\int_{\Gamma}{\psi\,\mathbf{u}\cdot\mathbf{n}\,d\Gamma} - \int_{\Omega}{s\,d\Omega} \tag{1}
> $$
> - For a fixed control volume, Reynolds transport theorem simplifies to:
> $$
> \frac{d}{dt}\int_{\Omega}{\psi\,d\Omega} = \int_{\Omega}{\frac{\partial\psi}{\partial t}\,d\Omega} \tag{2}
> $$
> - Applying divergence theorem allows us to change the first term on the RHS to a volume integral. Combined with Reynold's transpor theorem, the equation becomes:
> $$
> \int_{\Omega}{\frac{\partial\psi}{\partial t}\,d\Omega} = - \int_{\Omega}{\nabla\cdot(\psi\mathbf{u})\,d\Omega} - \int_{\Omega}{s\,d\Omega}
> $$
> $$
> \int_{\Omega}{\left(\frac{\partial\psi}{\partial t}\,d\Omega+\nabla\cdot(\psi\mathbf{u})+s\right)\,d\Omega} = 0
> $$
> $$
> \frac{\partial\psi}{\partial t}\,d\Omega+\nabla\cdot(\psi\mathbf{u})+s = 0 \tag{3}
> $$

