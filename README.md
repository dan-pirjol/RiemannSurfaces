# RiemannSurfaces
**Mathematica visualisation of Riemann surfaces**

This repository describes a simple method for visualisation of Riemann surfaces in Mathematica using **ParametricPlot3D**. The method is illustrated on the Riemann surface of the inverse of $\sinh(z)/z$ which is described in Section 3 of [Nandori, Pirjol (2022)](https://arxiv.org/abs/2209.09412), also [published version](https://www.sciencedirect.com/science/article/pii/S0377042721004404). 

Denote $f(z) = \frac{\sinh z}{z}$. Denote $f^{-1}(u)$ the inverse of this function. The inverse function $f^{-1}(x)$ is multivalued. For example, the equation $f(z)=1$ has an infinite number of complex solutions in addition to $z=0$ (which gives $f^{-1}(1)=\{ 0, \cdots \}$). This means that $f^{-1}(u)$ has an infinite number of Riemann sheets. On the "principal" sheet we have $f^{-1}(1)=0$. 

The function $f^{-1}(u)$ has branch points $( u_j )_{j\geq 1}$ on the real axis, in the $[-1,+1]$ interval. These points are given by $u_j = \cos \omega_j$ where $\omega_j$ solve $\tan \omega_j = \omega_j$. The first few branch points are $u_i=(-0.2172, +0.1284, -0.0913,\cdots)$. The closest branch point to $u=1$ on the principal Riemann sheet is at $u_1=-0.2172$.

The Riemann sheets are joined at branch cuts, which can be chosen as curves $(u_j, u_{j+1})$, joining two consecutive branch points. The structure of the Riemann sheets is similar to that of an infinite staircase, where one descends to the lower level by crossing a branch cut. This pattern is visible in the plots below.

The code plots the Riemann surface of $z(x)$ where $x = \frac{\sinh z}{z}$. More precisely, the code plots $Re(z^2)$ vs $(Re[x],Im[x])$. Denote $x=u+i v$.

The attached Mathematica code and the resulting evaluations are shown below. The plots take a large amount of memory (500MB) and GitHub does not allow such large files. Therefore I attach the plots as images below. The plots show the same Riemann surface over different regions in $[Re[x],Im[x])$.

<img width="771" alt="RScodep1" src="https://github.com/user-attachments/assets/1f5ad881-1ebd-4f53-883c-9de0eff82b26" />
<img width="763" alt="RScodep2" src="https://github.com/user-attachments/assets/dde96093-69e6-4c3c-8779-e4fef8316742" />
<img width="767" alt="RScodep3" src="https://github.com/user-attachments/assets/17a9bea8-fa32-4813-80b9-9c58401cfb4f" />


