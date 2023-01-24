#signal_analysis
0 Order Hold is not a good function to reconstruct a function with, because it'll create harmonics in the spectrum; better to use a $sinc$$ function in the time domain, which'll create a square function in the frequency domain (this violates causality).
### Nyquist Reconstruction
- If the Nyquist rate frequency = $2B$, then the reconstruction is a Nyquist reconstruction
### Aliasing
If the sampling frequency is less than the Nyquist rate frequency, then the replicas will overlap, and create distortion