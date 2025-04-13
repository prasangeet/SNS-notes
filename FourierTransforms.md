### 📚 General Fourier Transform Pairs (Continuous-Time)

1. **Dirac Delta Function**  
   \( x(t) = \delta(t) \)  
   \( X(j\omega) = 1 \)

2. **Constant Signal**  
   \( x(t) = 1 \)  
   \( X(j\omega) = 2\pi \delta(\omega) \)

3. **Complex Exponential**  
   \( x(t) = e^{j\omega_0 t} \)  
   \( X(j\omega) = 2\pi \delta(\omega - \omega_0) \)

4. **Cosine Signal**  
   \( x(t) = \cos(\omega_0 t) \)  
   \( X(j\omega) = \pi[\delta(\omega - \omega_0) + \delta(\omega + \omega_0)] \)

5. **Sine Signal**  
   \( x(t) = \sin(\omega_0 t) \)  
   \( X(j\omega) = j\pi[\delta(\omega + \omega_0) - \delta(\omega - \omega_0)] \)

6. **Unit Step Function**  
   \( x(t) = u(t) \)  
   \( X(j\omega) = \pi \delta(\omega) + \frac{1}{j\omega} \)

7. **One-Sided Exponential (Right-sided)**  
   \( x(t) = e^{-at}u(t),\ \text{Re}(a) > 0 \)  
   \( X(j\omega) = \frac{1}{j\omega + a} \)

8. **Rectangular Pulse**  
   \( x(t) = \text{rect}\left(\frac{t}{T}\right) \)  
   \( X(j\omega) = T \cdot \text{sinc}\left(\frac{\omega T}{2\pi}\right) \)

9. **Sinc Function**  
   \( x(t) = \text{sinc}(t) = \frac{\sin(\pi t)}{\pi t} \)  
   \( X(j\omega) = \text{rect}\left(\frac{\omega}{2\pi}\right) \)

10. **Triangular Pulse**  
   \( x(t) = \text{tri}(t) \)  
   \( X(j\omega) = \text{sinc}^2\left(\frac{\omega}{2}\right) \)

11. **Time Multiplied by Delta Function**  
   \( x(t) = t \)  
   \( X(j\omega) = j \cdot \frac{d}{d\omega} \delta(\omega) \)

12. **Hilbert Transform Kernel**  
   \( x(t) = \frac{1}{\pi t} \)  
   \( X(j\omega) = -j \cdot \text{sgn}(\omega) \)
