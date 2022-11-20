# Signals, Systems, and Information

## Signals and distributions

:::{panels}

**Gaussian**
^^^
$$ g(t,\sigma) = \frac{1}{\sigma\sqrt{2\pi}} \exp\left( \frac{-t^2}{2\sigma^2} \right) $$
---

**Dirac delta**
^^^
$$ \delta(t) = \lim_{\sigma \to 0}{g(t,\sigma)} $$

---

**Kronecker delta**
^^^

$$\delta[n] = \mathbf{1}_{\{n=0\}} = \begin{cases} 1 & \text{if } n=0 \\ 0 & \text{otherwise}\end{cases}$$

---

**Impulse train**
^^^
$$ \text{Ш}(t,T) =  \sum_{k=-\infty}^{\infty} \delta(t - k T) $$

:::

(sampling)=
## Sampling

$$x[n] = \left. x(t) \right|_{t=nT_s} = x(t) Ш(t,T_s)$$

(quantization)=
## Quantization

$$Q(x) = \Delta \text{ round} \left( \frac{x}{\Delta} \right) $$

(theorem-of-interpolation)=
## Cardinal theorem of interpolation

If a signal $x(t)$ contains no frequencies higher than B hertz, it is completely determined by giving its values at a series of points spaced $\frac{1}{2B}$ seconds apart.
