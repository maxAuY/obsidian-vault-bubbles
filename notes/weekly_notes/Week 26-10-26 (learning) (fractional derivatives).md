> [!note] The Gamma Function
> - The Gamma function, $\Gamma(z)$, is a function of a complex number, $z$, and is used to calculate fractional derivatives.
> - The function is written:
> $$\Gamma(z) = \int_0^\infty{t^{z-1}e^{-t}dt}$$
> - This can be thought of as a correlation between a logarithmically rotating complex number, $t^{z-1} = e^{(z-1)\ln t}$, and and exponential decay window, $e^{-t}$.
> - For all complex numbers, except for negative integers, the function behaves as a continuous factorial:
> $$\Pi(z) = \Gamma(z+1) = z!$$
> where $\Pi(x+1) = (x+1)\Pi(x)$ is what defines a factorial.
> - This is why it can be used to calculate a fractional derivative.

> [!note] The Caputo Fractional Derivative
> - Fractional derivatives are solvable using fractional integrals. 
> - The Caputo fractional derivative does this using the equation:
> $$
> ^CD^\alpha_tf(t) = \frac{1}{\Gamma(n-\alpha)} \int_0^t{\frac{f^{(n)}(\tau)}{(t-\tau)^{\alpha+1-n}}d\tau}
> $$
> - First, the $n$th derivative is calculated where $n$ is the smallest integer greater than $\alpha$, then a fractional integral is performed to partially reverse the last derivative.
> ---
> - This equation uses Cauchy's formula for repeated integrations:
> $$
> J^nf(t) = \int_0^t{\int_0^{t_1}{\dots\int_{0}^{t_{{n-1}}}{f(t_{n})dt_{n}\dots dt_{2}dt_{1}}}} = \frac{1}{(n-1)!}\int_{0}^t{(t-\tau)^{n-1}f(\tau)d\tau}
> $$
> which is written using gamma a gamma function to generalise the function to continuous orders:
> $$
> J^\beta f(t) = \frac{1}{\Gamma(\beta)} \int_0^t{(t-\tau)^{\beta-1}f(\tau)d\tau}
> $$
> $$
> ^CD_{t}^\alpha f(t) = J^{n-\alpha}\left[f^{(n)}(t)\right] = \frac{1}{\Gamma(n-\alpha)} \int_0^t{\frac{f^{(n)}(\tau)}{(t-\tau)^{\alpha+1-n}}d\tau}
> $$

