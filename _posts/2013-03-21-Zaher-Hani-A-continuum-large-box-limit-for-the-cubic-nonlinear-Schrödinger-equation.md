---
layout: post
author: James Colliander
tags : [notes, seminar]
---


Analysis &amp; Applied Math Seminar 2013-03-21

Speaker: <strong><a href="http://cims.nyu.edu/~hani/Zaher_Hani_-_Personal_Webpage/Welcome.html">Zaher Hani</a></strong>

Institution: <a href="http://cims.nyu.edu">New York University</a>
<blockquote><strong>Abstract</strong>: Inspired by the general paradigm of weak turbulence theory, we consider the 2D cubic nonlinear Schrödinger equation on a box of size L with periodic boundary conditions. In an appropriate “large box regime” (L very large), we derive a continuum equation on ℝ2 that governs the dynamics of the discrete frequency modes over nonlinear time scales. This equation turns out to satisfy many surprising symmetries and conservation laws, as well as several families of explicit solutions. (This is joint work with Erwan Faou (INRIA, France) and Pierre Germain (Courant Institute, NYU)).</blockquote>
<img id="zaherhani" src="http://cims.nyu.edu/~hani/Zaher_Hani_-_Personal_Webpage/Welcome_files/shapeimage_1.png" alt="Zaher Hani" />

#Introduction#

<h2 id="setup">Setup</h2>
2d cubic defocsusing or focusing NLS on a box of size $L$. Energy and mass conservation. NLS is GWP for small data in $H^s$ for $ s \geq 1$. We are not concerned with the existence issue. We are working in the setting of global-in-time solutions.

Physical and mathematical setup: weak nonlinearity.
<ul>
	<li>Aim: understand out-of-equilibrium dnamics of small solutions. e.g. CKSTT</li>
	<li>Take small data….nonlinear time scale is $\epsilon^{-2}$ where we imagine $ u \thicksim \epsilon v$ and we study $v$ with an $\epsilon^2$ coefficient and the data is of the size 1.</li>
	<li>Fourier ansatz, transfer dynamics onto the coefficients. Comments on the $L^2$ norm dependence upon the box size parameter $L$.</li>
	<li>Express the dynamics in terms of the $a_k (t)$.</li>
	<li>Define the 4-frequency convolution hypersurface. He calls that $S_K$.</li>
	<li>Interaction Representation. Conjugate by the fast linear dynamic….remove the linear dynamics. The new Fourier variable is called $\tilde{a}_k (t).$</li>
</ul>
All that has happened was a change of variables enabling us to view the dynamics on the Fourier side.
<h2 id="weakturbulenceparadigm">Weak turbulence “paradigm”</h2>
<ul>
	<li>Aim: statistical description of out-of-equilibrium dynamics of small solutions (Zakharov 60s, Kolmogorov 50s)</li>
	<li>RPA rand phase and amplitude.</li>
	<li>$n(K,t) = {\mathbb{E}} |a_k (t)|^2$ is the wave spectrum or mass density.</li>
	<li>propagation of chaos assumption. True at $t=0$, but not propagated.</li>
	<li>Roughly, we have three main steps:
<ol>
	<li>Statistical and time averaging.</li>
	<li>large-box limit $L \rightarrow \infty$.</li>
	<li>weak nonlinearity limit $\epsilon \rightarrow 0$ to arrive at a continuum equation for $n(K), ~ K \in {\mathbb{R}}^2.$</li>
</ol>
</li>
</ul>
The Kolmogorov-Zakharov kinetic equation. Long convolution equation localized on the convolution hypersurvface and further localized on the resonant set.
<ul>
	<li>Admits explicit stationary solutions called <strong>KZ spectra</strong>. These solutions are thought to offer some explanation to some cascade phenomena.</li>
	<li>Non-rigorous, KZ spectra are not integrable, negliects some finite-size effects, some numerical discrepancies, the appearance of some coherent structures called “quasi-solitons” even in defocusing problems.</li>
</ul>
<h1 id="anewlimitingequation">A New Limiting equation</h1>
Statistical averaging was causing problems. Let’s dispense with that but still take the large box and weak nonlinearity limits.

Resonant cutoff/normal forms transformation. He goes to the board and describes the separation. On the non-resonant portion, he makes a stationary phase type integration by parts, and then makes a crude estimate using the equation. This shows the non-resonant portion contributes at size $\epsilon^4 L^2$. Therefore, we concentrate our attention on the resonant terms.

(slide 12/37 and we are 20 minutes into the talk….)

He analyzes the convolution + resonance condition and identifies orthogonality properties based on the pythagorean relationship among frequencies.

Parametrization of rectangles in $\mathbb{Z}^2 / L$.

A lattice point $ J \in \mathbb{Z}^2 / L$ is called <strong>visible</strong> if $z = (p,q)/L$ with $gcd (|p|, |q|) =1. $ These points can be connected by a straight to the origin without hitting another point in the lattice.

Some new coordinates involving an $\alpha$ and $\beta$.

Co-prime equidistribution:

You can, in certain circumstances, replace sums by corresponding integrals with bounds. A classical number theory result establishes the <strong>density of visible lattice points</strong> in $\mathbb{Z}^2 / M$ is $\frac{6}{\pi^2}$. This lets you translate equidistribution into a co-prime equidistribution statement enabling us to replace sums by corresponding integrals with bounds.

<strong>Q:</strong>…interesting, I wonder to what extent similar ideas can be used on the sums we have omitted earlier in the argument. Perhaps those sums can also be represented as integrals with appropriate bounds?

Continuum limit.

Following these formal arguments leads to an integral equation resembling the KZ equation. <strong>Q:</strong> What are the differences/similarities with the KZ equation? One difference is that it preserves the Hamiltonian structure and has a positive definite Hamiltonian. He calls this equation $*$.

Symmetries lead to conserved quantities.

He writes the trilinear term in the equation as $\mathcal{T}(f,g,h)$.
<ul>
	<li>Hamiltonian</li>
	<li>Mass</li>
	<li>Momentum</li>
	<li>Position</li>
	<li>Second momentum</li>
	<li>Kinetic energy</li>
	<li>Angular momentum</li>
</ul>
A scaling property.

Invariance under Fourier transform.

If $g$ solves $*$ then $\hat{g}$ also solves $*$.
<h1 id="propertiesofthecontinuumequation">Properties of the continuum equation</h1>
Boudedness properties and well-posedness. He reports on LWP and GWP properties of the equation $*$.

Gaussian family is a family of explicit stationary solutions. Gaussians are the unique maxima of the Hamiltonian functional.

Heavy tailed solutions.

Are there more?

Invariance of Harmonic oscillator eigenspaces. Hermite polynomials. The associated linear spans are invariant under the nonlinear flow $*$. The Hamiltonian of the harmonic oscillator is an integral of motion so the two flows commute and you get this easily.

<strong>Question:</strong> Is this equation $*$ completely integrable?
<h1 id="rigorousapproximateresults">Rigorous Approximate Results</h1>
In analogy to the CKSTT cascade result, there is a reduction to an equation related to NLS. Can we transfer information from $*$ back to learn something about NLS?

Three difficulties:
<ol>
	<li>Pass to the resonant sum.</li>
	<li>Obtain good discrete to continuum error estimates.</li>
	<li>Trilinear estimates on resonant sums.</li>
</ol>
….discussion of these issues…. identifies the <strong>small nonlinearity regime</strong> characterized by the condition
$$ \epsilon^4 L^2 \ll \frac{\epsilon^2 \log L}{L^2}.$$

Möbius inversion formula.

<strong>Convergence Theorem:</strong> ….long statement. He gets a convergence statement on an interval that is <em>longer</em> than the nonlinear time scale by a factor $ M \leq \log \log L$.
<h1 id="furtherquestions">Further Questions</h1>
<ul>
	<li>Numerical study comparing NLS and $*$.</li>
	<li>Other explicit solutions of $*$? Cascading solutions? Videos.</li>
	<li>Is $*$ completely integrable?</li>
	<li>Similar continuum limit for other equations?</li>
</ul>