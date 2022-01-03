# Harmonic Analysis

## Cosine and sine transforms

$$\mathscr{C}\{{x(t)}\} = \int \limits_{t=-\infty}^{+\infty} {x(t)\cos{(\omega t)}dt}$$

$$\mathscr{S}\{{x(t)}\} = \int \limits_{t=-\infty}^{+\infty} {x(t)\sin{(\omega t)}dt}$$

## Fourier transform

$$\mathscr{F}\{x(t)\} = \mathscr{C}\{{x(t)}\} - j\mathscr{S}\{{x(t)}\} =
\int \limits_{t=-\infty}^{+\infty} {x(t) e^{-j\omega t} dt} $$

The Fourier transform of a periodic signal is also called a Fourier series.

The Fourier transform of a sampled signal is also called the discrete-time Fourier transform (DTFT)

The Fourier transform of a periodic, sampled signal is also called the discrete Fourier transform (DFT). This is also commonly referred to by the name of its algorithm, the fast Fourier transform (FFT).