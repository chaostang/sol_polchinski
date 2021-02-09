# A. A Short Course on Path Integrals

###### A.1

**(a).** Choose a complete orthonormal basis $\{\mathsf\Phi_j\}$ of periodic eigenfunctions such that $\Delta\mathsf\Phi_j=(-\partial_u^2+\omega^2)\mathsf\Phi_j=\lambda_j\mathsf\Phi_j$:
$$
\mathsf\Phi_0(u)=\left(\frac1U\right)^{1/2},\\
\mathsf\Phi_{+j}(u)=\left(\frac2U\right)^{1/2}\sin\frac{2j\pi u}U,\quad j=1,2,\cdots\\
\mathsf\Phi_{-j}(u)=\left(\frac2U\right)^{1/2}\cos\frac{2j\pi u}U,\quad j=1,2,\cdots
$$
Using the Pauli-Villars regulator ($\Omega\gg\omega$), the functional determinant is (up to a formal constant):
$$
\det\Delta=\omega^2\left(\prod_{j=1}^\infty\frac{4j^2\pi^2+\omega^2U^2}{U^2}\right)^2\\
\leadsto\omega^2\left(\prod_{j=1}^\infty\frac{j^2\pi^2+\omega^2U^2/4}{j^2\pi^2+\Omega^2U^2/4}\right)^2=\omega^2\left(\frac{\Omega\sinh\frac{\omega U}2}{\omega\sinh\frac{\Omega U}2}\right)^2.
$$
Including the counterterms, asymptotically as $\Omega\rightarrow\infty$, the periodic path integral is of the following form:
$$
{\rm Tr}\exp(-\hat HU)=\int[{\rm d}q]_P\exp(-S_E)\\
\sim\left(\det\Delta\right)^{-1/2}=\frac{1}{2\sinh\frac{\omega U}2}\exp\left(-S_\text{ct}+\frac12\Omega U-\ln\Omega\right).
$$
Finally, the normalization is fixed by requiring ${\rm Tr}\exp(-\hat HU)\rightarrow\exp(-E_0U)$ as $U\rightarrow\infty$, which implies ${\rm Tr}\exp(-\hat HU)=(2\sinh\omega U/2)^{-1}$. Indeed,
$$
{\rm Tr}\exp(-\hat HU)=\sum_{j=0}^{\infty}\exp\left(-(j+1/2)\omega U\right)=\frac1{2\sinh\frac{\omega U}2}.
$$

**(b).** For anti-periodic configurations, a basis of eigenfunctions is:
$$
\mathsf\Phi_{+j}(u)=\left(\frac2U\right)^{1/2}\sin\frac{(2j+1)\pi u}U,\quad j=1,2,\cdots\\
\mathsf\Phi_{-j}(u)=\left(\frac2U\right)^{1/2}\cos\frac{(2j+1)\pi u}U,\quad j=1,2,\cdots
$$

$$
\det\Delta=\left(\prod_{j=1}^\infty\frac{(2j+1)^2\pi^2+\omega^2U^2}{U^2}\right)^2\leadsto\left(\frac{\cosh\frac{\omega U}2}{\cosh\frac{\Omega U}2}\right)^2.
$$

$$
\int[{\rm d}q]_A\exp(-S_E)\sim\frac1{2\cosh\frac{\omega U}2}\exp\left(-S_\text{ct}+\frac12\Omega U\right),\quad\text{as }\Omega\rightarrow\infty.
$$
The normalization is fixed by ${\rm Tr}\left[\exp(-\hat HU)\hat R\right]\rightarrow\exp(-E_0U)=(2\cosh\omega U/2)^{-1}$ as $U\rightarrow\infty$.
$$
{\rm Tr}\left[\exp(-\hat HU)\hat R\right]=\sum_{j=0}^{\infty}(-)^j\exp\left(-(j+1/2)\omega U\right)=\frac1{2\cosh\frac{\omega U}2}.
$$
