# Signals, Systems, and Information

## Continuous signals and distributions

### Gaussian

$$ g(t,\sigma) = \frac{1}{\sigma\sqrt{2\pi}} \exp\left( \frac{-t^2}{2\sigma^2} \right) $$

### Dirac delta

$$ \delta(t) = \lim_{\sigma \to 0}{g(t,\sigma)} $$

### Impulse train

$$ \text{Ш}(t,T) =  \sum_{k=-\infty}^{\infty} \delta(t - k T) $$

(sampling)=
## Sampling

$$x[n] = \left. x(t) \right|_{t=nT_s} = x(t) Ш(t,T_s)$$

(quantization)=
## Quantization

## Information theory

(theorem-of-interpolation)=
### Cardinal theorem of interpolation
