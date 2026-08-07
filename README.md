\documentclass[12pt]{article}
\usepackage{amsmath, amssymb, amsthm, physics}
\usepackage{geometry}
\geometry{margin=1in}

\title{Analytical Mechanics: Rigorous Evaluation of Central Inverse-Square Central Trajectories}
\author{Ali Hamadu Assumi}
\date{}

\begin{document}
\maketitle

\section*{System Formulation}

A point mass $m$ operates within a conservative central potential field governed by the inverse-square force formulation:

\[
\mathbf{F}(\mathbf{r}) = -\frac{k}{r^2}\hat{\mathbf{r}} \implies V(r) = -\frac{k}{r}
\]

The Lagrangian setup using standard planar coordinates $(r, \theta)$ is formalized as:

\[
L = T - V = \frac{1}{2}m\left(\dot{r}^2 + r^2\dot{\theta}^2\right) + \frac{k}{r}
\]

Applying the Euler-Lagrange equations for the angular coordinate $\theta$:

\[
\frac{d}{dt}\left(\frac{\partial L}{\partial \dot{\theta}}\right) - \frac{\partial L}{\partial \theta} = 0 \implies \frac{d}{dt}\left(mr^2\dot{\theta}\right) = 0
\]

This confirms that the generalized angular momentum $p_\theta$ is a strict constant of motion:

\[
p_\theta = mr^2\dot{\theta} = L_{\text{const}}
\]

\section*{The Binet Dynamic Transformation}

Invoking the differential substitution operator $u = \frac{1}{r}$, the time-dependent velocity component transforms as:

\[
\dot{r} = \frac{dr}{dt} = \frac{dr}{d\theta}\dot{\theta} = \frac{d}{d\theta}\left(\frac{1}{u}\right)\frac{L_{\text{const}}u^2}{m} = -\frac{L_{\text{const}}}{m}\frac{du}{d\theta}
\]

Differentiating a second time and substituting into the total energy equation yields the non-linear differential equation of motion:

\[
\frac{d^2u}{d\theta^2} + u = \frac{mk}{L_{\text{const}}^2}
\]

The exact analytical evaluation of this second-order system resolves cleanly into a general conic section:

\[
u(\theta) = \frac{mk}{L_{\text{const}}^2} \left[ 1 + e\cos(\theta - \theta_0) \right] \implies r(\theta) = \frac{\alpha}{1 + e\cos(\theta - \theta_0)}
\]

Where the system eccentricity tensor scaling properties are directly bounded by:

\[
\alpha = \frac{L_{\text{const}}^2}{mk}, \quad e = \sqrt{1 + \frac{2EL_{\text{const}}^2}{mk^2}}
\]

\end{document}# advanced-physics-solutions
