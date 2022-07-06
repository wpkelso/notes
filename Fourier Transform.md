# Fourier Transform
Used to analyze signals in the [[Frequency Domain]].
Goes from time domain to frrquncy domain. To go back you would need to use the [[Inverse Fourier Transform]].

### Definitions
$G(f)=F\{g(t)\}$
$G(f)=\int _{t=-\infty}^{t=\infty}g(t)e^{-j2\pi ft}dt$

$g(t)$ <-> $G(f)$

$g(t)=F^{-1}\{G(f)\}$
$g(t)=\int _{t=-\infty}^{t=\infty}G(f)e^{j2\pi ft}df$

*Note: $s$->$j2\pi t$*

Response of a ____ : Sinc function

### Properties
- Multiplication in the time domain is convolution in the frequency domain
- Convolution in the time domain is multiplication in the frequency domain
- $a(t)+b(t)$ -> $A(f)+B(f)$
- $a(t-T)$ -> $e^{-j2\pi fT}A(f)$
