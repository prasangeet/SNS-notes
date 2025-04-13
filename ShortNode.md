# DTFT Pair Reference Sheet

## 1. Unit Impulse (Kronecker Delta)
**Time domain:**  
$x[n] = \delta[n]$

**Frequency domain:**  
$X(e^{j\omega}) = 1$

---

## 2. Delayed Impulse
**Time domain:**  
$x[n] = \delta[n - n_0]$

**Frequency domain:**  
$X(e^{j\omega}) = e^{-j\omega n_0}$

---

## 3. Unit Step
**Time domain:**  
$x[n] = u[n]$

**Frequency domain:**  
$X(e^{j\omega}) = \frac{1}{1 - e^{-j\omega}}$

---

## 4. Exponential
**Time domain:**  
$x[n] = a^n u[n],\ |a| < 1$

**Frequency domain:**  
$X(e^{j\omega}) = \frac{1}{1 - a e^{-j\omega}}$

---

## 5. Rectangular Pulse (Dirichlet Kernel)
**Time domain:**  
$x[n] = 1\ \text{for}\ |n| \leq N$

**Frequency domain:**  
$X(e^{j\omega}) = e^{-j\omega N} \cdot \frac{\sin\left((2N+1)\frac{\omega}{2}\right)}{\sin(\omega/2)}$

---

## 6. Sinc Function
**Time domain:**  
$x[n] = \frac{\sin(\alpha n)}{\pi n}$

**Frequency domain:**  
$X(e^{j\omega}) =
\begin{cases}
1, & |\omega| \leq \alpha \\
0, & \text{otherwise}
\end{cases}$

---

## 7. Cosine
**Time domain:**  
$x[n] = \cos(\omega_0 n)$

**Frequency domain:**  
$X(e^{j\omega}) = \pi\left[\delta(\omega - \omega_0) + \delta(\omega + \omega_0)\right]$

---

## 8. Sine
**Time domain:**  
$x[n] = \sin(\omega_0 n)$

**Frequency domain:**  
$X(e^{j\omega}) = \frac{\pi}{j} \left[\delta(\omega - \omega_0) - \delta(\omega + \omega_0)\right]$

---

## 9. Geometric Series
**Time domain:**  
$x[n] = r^n u[n],\ |r| < 1$

**Frequency domain:**  
$X(e^{j\omega}) = \frac{1}{1 - r e^{-j\omega}}$

---

## 10. Constant Function
**Time domain:**  
$x[n] = 1$

**Frequency domain:**  
$X(e^{j\omega}) = 2\pi \sum_{k=-\infty}^{\infty} \delta(\omega - 2\pi k)$
