>[!note] Taylor Expansion
> - The Taylor expansion is derived by assuming that the function can be written as a polynomial:
> $$
> F(x) = \sum_{n=0}^\infty{c_n(x-h)^n} \tag{1}
> $$
> @ $x=h$:
> $$
> c_0 = F(h)
> $$
> differentiating wrt. $x$:
> $$
> F'(x) = n\sum_{n=1}^\infty{c_n(x-h)^{(n-1)}}
> $$
> @ $x=h$:
> $$
> c_1 = \frac{F'(h)}{n}
> $$
> differentiating repeatedly wrt. $x$:
> $$
> c_n = \frac{F^{(n)}(h)}{n!} \tag{2}
> $$
> substitute Eq. 2 into Eq. 1 gives the equation for the Taylor expansion:
> $$
> F(x) = \sum_{n=0}^\infty{\frac{F^{(n)}(h)}{n!}(x-h)^n} \tag{3}
> $$

> [!note] Finite Difference Methods
> - Finite difference formulas aim to use a chosen value, $F(x_i)$, to estimate the value of a nearby point, $F(x_i + \Delta x)$.
> 
> 	let $\Delta x$ be a small perturbation from $x$ and evaluating at $h=x_i$, the value of the function at a neighbouring point $x_i + \Delta x$:
> $$
> F(x_i+\Delta x) = \sum_{n=0}^\infty{\frac{F^{(n)}(x_i)}{n!}(x_i+\Delta x-x_i)^n}
> $$
>  $$
> F(x_i+\Delta x) = F(x_i) + F'(x_i)\Delta x + \mathcal{O}(h^2) \tag{4}
> $$
> Solving for the gradient, $F'(x)$, gives the **forwards difference approximation**:
> $$
> F'(x_i) = \frac{F(x_i+\Delta x) - F(x_i)}{\Delta x} \tag{5}
> $$
> and similarly, for a point behind $x_i$ at $x_i - \Delta x$:
> $$
> F(x_i-\Delta x) = \sum_{n=0}^\infty{\frac{F^{(n)}(x_i)}{n!}(x_i-\Delta x-x_i)^n}
> $$
>  $$
> F(x_i-\Delta x) = F(x_i) - F'(x_i)\Delta x + \mathcal{O}(h^2) \tag{6}
> $$
> Solving for the gradient, $F'(x)$, gives the **backwards difference approximation**:
> $$
> F'(x_i) = \frac{F(x_i) - F(x_i-\Delta x)}{\Delta x} \tag{5}
> $$
> Subtracting Eq. 6 from Eq. 4 gives:
> $$
> F(x_i+\Delta x) - F(x_i-\Delta x) = 2 F'(x_i)\Delta x + \mathcal(O)(h^3)
> $$
> Solving for the gradient, $F'(x_i)\Delta x$, gives the central difference approximation:
> $$
> F'(x_i) = \frac{F(x_i+\Delta x) - F(x_i-\Delta x)}{2\Delta x}
> $$
> ---
> - Forward and backward finite difference approximations are 1st order accurate because they ignore 2nd order and above. This means that the error scales linearly with the step size, $\Delta x$.
> - Central difference is 2nd order accurate because the even powers cancel out in the derivation. This makes the error magnitude much smaller than forward and backward difference methods.

