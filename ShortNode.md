\documentclass[12pt]{article}
\usepackage{amsmath, amssymb}
\usepackage[margin=1in]{geometry}
\usepackage{titlesec}
\usepackage{graphicx}
\usepackage{lmodern}
\titleformat{\section}{\large\bfseries}{\thesection}{1em}{}

\title{\textbf{DTFT Pair Reference Sheet}}
\author{}
\date{}

\begin{document}
\maketitle
\section*{DTFT Pairs}

\begin{itemize}
  \item \textbf{1. Unit Impulse (Kronecker Delta)}\\
  $x[n] = \delta[n] \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = 1$
  
  \item \textbf{2. Delayed Impulse}\\
  $x[n] = \delta[n - n_0] \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = e^{-j\omega n_0}$
  
  \item \textbf{3. Unit Step}\\
  $x[n] = u[n] \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = \frac{1}{1 - e^{-j\omega}}$
  
  \item \textbf{4. Exponential}\\
  $x[n] = a^n u[n],\ |a| < 1 \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = \frac{1}{1 - a e^{-j\omega}}$
  
  \item \textbf{5. Rectangular Pulse (Dirichlet Kernel)}\\
  $x[n] = 1\ \text{for}\ |n| \leq N \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = e^{-j\omega N} \cdot \frac{\sin\left((2N+1)\frac{\omega}{2}\right)}{\sin(\omega/2)}$
  
  \item \textbf{6. Sinc Function}\\
  $x[n] = \frac{\sin(\alpha n)}{\pi n} \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = 
  \begin{cases}
  1, & |\omega| \leq \alpha \\
  0, & \text{otherwise}
  \end{cases}$
  
  \item \textbf{7. Cosine}\\
  $x[n] = \cos(\omega_0 n) \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = \pi\left[\delta(\omega - \omega_0) + \delta(\omega + \omega_0)\right]$
  
  \item \textbf{8. Sine}\\
  $x[n] = \sin(\omega_0 n) \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = \frac{\pi}{j} \left[\delta(\omega - \omega_0) - \delta(\omega + \omega_0)\right]$
  
  \item \textbf{9. Geometric Series}\\
  $x[n] = r^n u[n],\ |r| < 1 \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = \frac{1}{1 - r e^{-j\omega}}$
  
  \item \textbf{10. Constant Function}\\
  $x[n] = 1 \quad \xleftrightarrow{\text{DTFT}} \quad X(e^{j\omega}) = 2\pi \sum_{k=-\infty}^{\infty} \delta(\omega - 2\pi k)$
\end{itemize}

\end{document}
