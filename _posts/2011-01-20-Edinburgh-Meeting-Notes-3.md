---
layout: post
category : lessons
tags : [notes, Edinburgh]
comments: false
---


<!--  -->




<h1>Galina Perelman: 2 soliton collision in NLS</h1>
$$
i \psi_t = - \psi_{xx} + F(|\psi|^2) \psi, ~ x \in R
$$
where $F(\xi) = -2 \xi + O (\xi^2), ~ \xi \rightarrow 0.$

This family of equations has solitary wave solutions
$$
e^{i \theta(x,t) \phi (x - b(t), E)}
$$
where $\theta(x,t) = \omega t + \gamma + v \frac{x}{2}, ~b(t) =vt + c$ (all reall parameters). The profile $\phi$ is the associated ground state, which is $C^2$, decays exponentially, is even, …



If I set $\epsilon^2 = E$ and write $\phi(y, \epsilon^2) = \epsilon \hat{\phi}(\epsilon, \epsilon).$ We have then that $\hat{\phi}(z, \epsilon) = \phi_0 (z) + O(\epsilon^2)$ where $\phi_0$ is the standard soliton for cubic NLS. A calculation shows that
$$\| \phi(\cdot, \epsilon^2) \|_{H^1} = O(\epsilon^{1/2}).$$ Let’s collect the parameters $\sigma = (\beta, E, b, v) \in R^4.$

The question I’d like to address:

<strong>Question:</strong> As $t \rightarrow -\infty$, suppose that $\psi(t) = w(\cdot, \sigma_0 (t)) + w(\cdot, \sigma_1 (t)) + o_{H^1} (1)$. Because of the galilean invariance we can arrange so that $\sigma_0$ does not move and we assume that $v_1 &gt; 0$. So, we can arrange this data to have completely decoupled solitons as $t \rightarrow - \infty$. The question is then to understand the soliton collision and also what happens afterwards.

<strong>Perturbative regime:</strong>
$$\epsilon^2 = E_1 \ll 1, E_0 \thicksim 1, v_1 \thicksim 1.$$

<strong>Collision Scenario:</strong>
<ol>
	<li>$w(\cdot, \sigma_0 (t))$ is ‘preserved’.</li>
	<li>$w(\cdot, \sigma_1 (t))$ splits into two outgoing waves of the cubic NLS. The splitting is controlled by the linearized operator associated to the large soliton $w_{\sigma_0}$.</li>
</ol>
Collision: $|t| \lesssim \epsilon^{-1-\delta}, ~ \delta &gt; 0$.
pre-interaction: $t leq - \epsilon^{-1-\delta}$
post-interaction: $t leq - \epsilon^{-1-\delta}$

She draws a picutre:

Long wide soliton to the left of a big soliton at the origin before the collision. After the collision the small soliton splits into two waves, one moving left and one moving right. The big soliton at the origin is drawn not centered at the origin.

$s = s(\frac{v_1}{2}), r = r (\frac{v_1}{2})$ where $s(k), r(k)$ are the translation and reflection coefficients of the linearized operator corresponding to $w(\cdot, \sigma_0 (t))$. Here we have $|s|^2(k) + |r|^2 (k) =1$. The only trace of nonlinearity appears in the phase.

This phenomena has been observed before by <a href="http://arxiv.org/abs/math/0608510">Holmer-Mazuola-Zworski</a> and earlier by physicists.
H-M-Z conisdered the cubic NLS with an external delta potential. For small incoming solitons, they have observed the small soliton splitting caused by the Dirac function potential.

<strong>Hypotheses:</strong>

<strong>(H0):</strong> $F \in C^\infty, F(\xi) = - 2 \xi + O(\xi^2), \xi \rightarrow 0.$
$F(\xi ) \geq - C\xi^q, C&gt;0, q&lt;2, \xi \geq 1$. (GWP in $H^1$)
$\exists !$ ground state.

Linearization around $w(x, \sigma(t)) = e^{i\theta} \phi(x - b(t), E)$. We substitute $\psi = w + f$ and expand to obtain the following equation for $f$:

$$
i {\bf{f}}_t = L(E) {\bf{f}}.
$$

Here ${\bf{f}}$ is a (column) vector $(f, \overline{f})$.
$$
L(E)= (-\partial_y^2 + E) \sigma_3 + V(E).
$$
Here $\sigma_3$ is the Pauli matrix and $V$ is a certain matrix involving $V_1 = F(\phi^2) + F’ (\phi^2) \phi^2$ and $V_2 = F’ (\phi^2) \phi^2$.

She draws a spectral plane. Essential spectrum along real line in region $|x| &gt; E$ and some eigenvalues drawn as x’s inside the gap and one above and below the real line on the imaginary axis. 0 is an eigenvalue. We have two explicit eigenfunctions $\xi_0$ and $\xi_1$.

$M(E)$ is the generalzied null space of $L(E)$. We have the following equivalence:

$$\sigma(L(E)) \subset R, {\mbox{dim}} M(E) = 4 \iff  \frac{d}{dE} \| \phi(E) \|_2^2 &gt; 0.$$

These conditions imply the orbital stability of $\Phi$.

$Lf = \lambda f, ~\lambda \geq E, \lambda = E + k^2, ~ k \in R$. If $k^2 + I \notin \sigma_p (L(E))$ then $\exists ~! ~ f(x,k) = s(k) e^{i k x} (1, 0)^t + O(e^{-\gamma x})$ as $ x\rightarrow + \infty, ~ \gamma &gt; 0$ and $f(x,k) = e^{ikx} (1,0)^t + r(k) e^{-ikx}(1,0)^t + O(e^{\gamma x}), x \rightarrow - \infty$.

$w(x,\sigma, t), ~ j=0,1$ normalized as before.

<strong>(H1):</strong>
$$\frac{d}{dE} \| \phi(E) \|<em>2^2 |</em>{E=E_0} &gt; 0$$

<strong>(H2):</strong> $\epsilon^2 = E_1$ sufficiently small

<strong>(H3):</strong> $M(E + \frac{v_1^2}{4}) \notin \sigma_p (L(E_0))$ (Nobody knows how to prove no embedded eignevalues.)

<strong>Proposition:</strong> $\exists ~! ~ \psi \in C(R, H^1)$ such that ….

<strong>Theorem:</strong> For $\epsilon^{-1-\delta} \leq t \leq \delta \epsilon^{-2} | \ln \epsilon |$

$$ \psi (t) = w (\cdot, \sigma(t)) + \psi_+ (t) + \psi_{-} (t) + h(t)$$
<ol>
	<li>$\sigma(t) = (\beta(t), E_0, b(t), v_0), ~V_0 = \epsilon \kappa$ where $\kappa$ is an explicit constant and
$$
|\beta(t) - \beta_0  (t)|, |b(t) - v_0 t| \leq C \epsilon^2 t.
$$</li>
	<li>$\Psi_{\pm} (x,t) = ….ack too fast to type…
$$\Psi_{\pm}$$</li>
</ol>
is expressed as an explicit phase times a function $S^{\pm}$ which solves cubic NLS emerging from data built using thre reflection, transmission coefficients and $\phi_0 (y)$.
3. error estimates in terms of $\epsilon.$

<hr />

<h1 id="edrisstiti:lossofsmoothnessin3deulerequations">Edriss Titi: Loss of smoothness in 3d Euler Equations</h1>
(joint work with Claude Bardos)

Overview:
<ol>
	<li>Background
<ul>
	<li>Euler</li>
	<li>Classical</li>
	<li>Nonuniqueness: De Lellis - Sh…</li>
</ul>
</li>
	<li>Shear flow
<ul>
	<li>DiPerna Majda example: weak limit of Euler solutions whose limit is not a solution</li>
	<li>Illposedness of Euler in C^{0,\alpha}</li>
</ul>
</li>
	<li>Vortex sheets induced by 3d shear flows
<ul>
	<li>Examples</li>
	<li>Differences between 2d and 3d Kelvin-Helmholtz problems</li>
	<li>Comments on numerics</li>
</ul>
</li>
</ol>
<h2 id="eulerequations">Euler equations</h2>
Euler equations on the 3-torus. $\omega$ is the vorticity. Recast using Biot-Savart.

Vorticity stretching term distinguishes 2d and 3d.

Classical Wellposedness:
<ul>
	<li>global existence and uniquenes for initial data $\omega_0 \in L^\infty$.
This result is due to Yudovich (1963). Some extension….</li>
	<li>For data in $C^{1,\alpha}$, Euler equations are short time well-posed and the solution conserves energy. [Lictenstein (1925)]</li>
	<li>The same result holds the context of Sobolev spaces $H^s, ~ s &gt; \frac{5}{2}$. (Basically same result in more modern spaces)</li>
</ul>
<strong>Question:</strong> Does there exist a regular solution (say in $C^{1,\alpha}$) of the 3d Euler equation that becomes singular in a finite time (blows up problem)? This is in osome sense as difficult as the millenium problem. There are different opinions….

“I spoke with Necas about this…near end of his life…on Wendesday’s he thinks it blows up and on Thursdays he thinks no…so he has bad dreams about it…”

DeLellis-Szekelyhidi: There exists a set of initial data $u_0 \in L^2 (\Omega)$ (not explicitly constructed, Baire argument) for which the Cauchy problem has, for the same inital data, an infinite family of weak solutiosn of the 3d Euler equations: a residual set in the space $C(R; L^2_{weak} (\Omega))$.

These are also in $L^\infty$ so they have finite energy. (Built on Shnirelman and others….). This is a breakthrough…but it is not so physical. Maybe a selection mechanism….for NS we don’t have such a result. Leray solutions are not known to be unique. Any result like this for NS would be extremely important….connect it with turbulence. The lack of uniqueness, according to Leray, relates to turbulence.
<h2 id="shearflows:">Shear flows:</h2>
$$u(x,t) = (u_1 (x_2), 0, u_3 (x_1 - t u_1 (x_2))).$$

For $u_1, u_3 \in C^1$, the above shear flow is a classical solution of the Euler equations with pressure $p=0$. Yudovich used these to show the existence of solutions with exponentially growing high regularity norms.

This example due to DiPerna-Majda (1987).

<strong>Theorem (DiPerna-Lions):</strong> Norm explosion in $W^{1,p}$ for Euler, for any $p \geq 1$.

Idea of the proof:
$ \partial_{x_2} u_3 (x_1 - t u_1 (x_2))=…$

<strong>Theorem:</strong> The shear flow is a weak solution of the Euler equations in the sense of distribtuions in $R^3$, provided $u_1, u_3 \in L^2_{loc} (R^3)$. On the periodic box, we can do same thing and in this case we have finite energy.

Why do I stress the finite energy? This relates to the Onsager conjecture.

<strong>Theorem</strong> [Ill-posedness of the Euler equations in $C^{0,\alpha}$]:

The shear flow with $C^{1,\alpha}$ components $u_1, u_3$. However, for $u_1, u_3 \in C^{0,\alpha}$ then the above shear flow is always in $C^{0, \alpha^2}$ which is a much larger space. We instantly lose the $C^{0, \alpha}$. There exists a shear flow which starts in $C^{0, \alpha}$ which, at any positive time, is not in $C^{0, \beta}$ for any $\beta &gt; \alpha^2$.

This family of solutions is compactly supported in space and time.

<strong>Other spaces and optimal spaces:</strong>

There are many layers of spaces between these H"older spaes. He writes a tower of inclusions between $C^{1,\alpha } \subset C^{0, \alpha}$. In fact, there is well-posedness
[Pak and Park] vs. failure of wp in $B^1_{\infty, infty}$ (Zygmund class) and failure in certain Triebel-Lizorkin spaces.

<strong>Weak limit of oscillating initial data:</strong>

DiPerna-Majda example…

Shear flow with vorticity interface. Vortex sheet flows are irrotational off an interface. To build such solutions he takes $u_1, u_3$ as (parametrized) Heaviside functions.

…wow…this talk is coming pretty fast, slides are changing…I stop typing and start to just try to keep up.
<h2 id="numericalinvestigationofblowupforthe3deuler">Numerical investigation of blowup for the 3d Euler</h2>
John Gibbon gave a talk a few years ago on the history of these investigations. Tom Hou and Bob Kerr are competing and disagreeing in this direction….is there a singularity…maybe not?

<strong>Question:</strong> Does the soluton of the following PDE blow up?
$$
\partial_t u - \nu \Delta u = |\nabla u |^4?
$$

What would you try numerically to determine if it blows up or not? You can even collapse it to the corresponding 1d problem?

<strong>Postlude Discussion:</strong>
Yudovich explored the DiPerna-Lions shear flow examples to see that norms measuring high regularity can grow exponentially in time. Chemin has studied the vortex patch and shown some measures of regularity of the boundary of the patch grow doubly exponentially fast. It was not explicitly clear to me yet how to relate Chemin’s rough patch boundary example to the growth of norms measuring regularity of the solution. Also, Chemin’s examples emerge from non-smooth initial data. I remain interested in the question: Does there exist nice data for 2D Euler which evolves with high regularity norms growing doubly exponentially?

<hr />

<h1 id="benoitgrberthttp:www.math.sciences.univ-nantes.frgrebert:hamiltonianinterpolationforapproximationofpdes."><a href="http://www.math.sciences.univ-nantes.fr/~grebert/">Benoit Grébert</a>: Hamiltonian Interpolation for Approximation of PDEs.</h1>
(joint work [<a href="http://www.irisa.fr/ipso/perso/faou/publis/beaHPDE7.pdf">Grébert-Faou</a>] with <a href="http://www.irisa.fr/ipso/perso/faou/">Erwan Faou</a>)

<strong>Aim:</strong>

Take a PDE with solution u. Consider a numerical approximation $u^n$ built with a <em>symplectic integrator</em> which approximates $u(nh)$. We build a hamiltonian $H_h$ such that
$$u^n = \Phi_{Hh}^{nh}(u_0) + very ~small.$$

I am concerned with the <strong>long time behavior of the numerical trajectory</strong>.

My concern right now is not in estimating the quality of the approximation. Instead, I want to understand the <em>numerical flow</em>.

<strong>Outline:</strong>
<ol>
	<li>Finite dimensional Context (ODE)</li>
	<li>PDE Context</li>
	<li>Ideas of the proof (time permitting)</li>
</ol>
<h2 id="finitedimensionalcontext">Finite Dimensional Context</h2>
We go back to Moser’s theorem. A discrete symplectic map close to the identity can be approximated by a Hamiltonian flow. Consider an analytic symplectic map
$$
R^{2n} \ni (p,q) \longmapsto \Psi(p,q) \in R^{2n}
$$
with $\Psi = Id + O(\epsilon)$. Then $\exists~ H_\epsilon$ such that
$$\Psi = \Phi_{H\epsilon}^\epsilon + O(e^{-\frac{1}{c\epsilon}}).$$
([Moser 1968], [Benettin-Giorgilli 1994])

Numerical Context: Suppose I have a Hamiltonian ODE system
$$ (\dot{p}, \dot{q}) = X_H (p,q)
$$
and an associated numerical discrete-time-step symplectic integrator
$$
(p_n, q_n)= \Psi_h^n (p_0, q_0).
$$
We then have that $\Psi_{h} = \Phi_{Hh} + O(e^{-1/ch}).$ We obtain that $H_h (p_n, q_n) = H_h (p_0, q_0) + n e^{-1/ch}$. So, we are observing that the modified energy is essentially conserved for exponentially long times.

<strong>Backward Error Analysis</strong>
<ul>
	<li><a href="http://www.springerlink.com/content/l687gym3wxgx5f07/">[Hairer-Lubich 1997]</a></li>
	<li>[Reich 1999]</li>
</ul>
<h2 id="pdecontext">PDE Context</h2>
$$ H = H_0 + P$$
Here we imagine $H_0$ is the linear part and P is the nonlinear part. As an example, consider the cubic NLS on $T^d$. We can treat other equations as well. Let’s recall the <em>Hamiltonian formalism</em> in the Fourier variables:

Expand $u$ to get
$$
u = \sum \xi_j e^{ijx}, ~ {\overline{u}}= \sum \eta_j e^{-ijx}.
$$
We can then write, for each $j \in Z^d$,
$$
{\dot{\xi}} = -i \frac{\partial H}{\partial \eta}
$$
$$
{\dot{\eta}} = i \frac{\partial H}{\partial \xi}.
$$
For the cubic NLS case, we obtain
$$
H = \sum |j|^2 \xi_j \eta_j + \sum^* \xi_{k_1} \xi_{k_2} \eta_{l_1} \eta_{l_2}
$$
where $\sum^*$ is the sum over all the parameters subject to the constraint $k_1 + k_2 = l_1 + l_2$.

The problem we face here is that the linear part is unbounded, and we have infinitely many dimensions as first obstructions in passing from the ODE to the PDE context.

<strong>Splitting Method:</strong>
$$\Phi_{P+H0 } \thicksim \Phi_p^h \circ \Phi_{H0}^h =^? \Phi_{Hh}^h.$$

First naive idea: Use the Baker-Campbell-Haussdorf formula. We can then expand as a Lie series…
to write
$$\Phi_p^h \circ \Phi_{H0}^h = e^{h\mathcal{L}p}e^{h\mathcal{L}H0} = e^{h\mathcal{Hh}}
$$
with $H_h = H_0 + P + \frac{h}{2}{ P, H_0 } + \dots.
$$

To proceed, we will need conditions $small = h^N C(N,, \| num sol \|_H^N)$ NOT FAIR! So we need to work harder.

<strong>First Idea:</strong>
Replace $hH_0$ by $A_0$ by cutting off to low frequencies. We can splt and impose the CFL condition.
Midpoint + split. He considers different cutoffs.

We then consider $\Phi_p^h \circ \Phi_{A_0}^1$.

<strong>Second Idea:</strong> Use the Wiener Algebra. Space of functions with Fourier coefficients in $l^1$.

<hr />

<strong>Theorem (<a href="http://www.irisa.fr/ipso/perso/faou/publis/beaHPDE7.pdf">Grébert-Faou</a>):</strong> For the approximation scheme $\Phi_p^h \circ \Phi_{A_0}^1$ there exists a (polynomial) modified energy $H_h$ such that

$$
\| \Phi_p^h \circ \Phi_{A_0}^1 (\xi, \eta) - \Phi_{Hh}^h(\xi, \eta) \|_{l^1} \leq h^{N+1} (cN)^N
$$

uniformly for $\|(\xi, \eta)\|_{l^1} \leq M.$

So, assuming that the numerical trajectory is bounded in $l^1$ (as opposed to the stronger claim that it is bounded in $H^k$ for $k$ large) then
$$
H_h (u^n) = H_h (u_0) + Cn h^{N+1}.
$$

<hr />

Of course, I have to explain: what is $N$? This is related to a regularization condition. We know that $N = \frac{r-2}{r_0 - 2}$ where $r_0$ is the degree of $P$ (so 4 for cubic NLS). The parameter $r$ is determined by the condition:
$ \forall ~ j = 1, \dots, r$ and for any $j$-tuple of integers $(k_1, \dots, k_j) \in Z^d$, we have
$$|\lambda_{k1} \pm \lambda_{k2} \pm \dots \pm \lambda_{kj}| \leq 2 \pi.$$

CFL: $|\lambda_k | \leq C$.

He describes some examples where $N = 3, 4$ and $N=7$.

For cubic NLS, we end up obtaining
$$Hh = \frac{1}{h} A_0 + Z_1 + h Z_2 + \dots
$$
where
$$
Z_1 = \sum^* \frac{e^{i(\lambda_{k1} \pm \lambda_{k2} \pm \dots \pm \lambda_{kj})}}{e^{i(\lambda_{k1} \pm \lambda_{k2} \pm \dots \pm \lambda_{kj})} - 1}.
$$
You can now see how the zero divisor issue emerges and is resolved.

<hr />

<!--#include virtual="${Base_URL}/templates/footer.html" -->