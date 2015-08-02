---
layout: post
category : lessons
tags : [Notes, USA, IAS]
comments: false
---

<!-- Processed by MultiMarkdown -->

<a href="http://www.math.ias.edu/">IAS School of Mathematics</a>

&nbsp;

<a href="https://www.math.ias.edu/pictures/math/simonyi-flowers.jpg"></a><a rel="attachment wp-att-1014" href="http://blog.math.toronto.edu/colliand/2012/03/15/ias-workshop-on-symplectic-dynamics-2-thursday/simonyi-flowers/"><img class="alignnone size-medium wp-image-1014" src="http://blog.math.toronto.edu/colliand/files/2012/03/simonyi-flowers-300x225.jpg" alt="" width="300" height="225" /></a>

<a href="http://www.math.ias.edu/wsd2">Workshop web page</a>
<h2 id="thursday:2012-03-15">Thursday: 2012-03-15</h2>
<ul>
	<li>9:00 - 10:00    Peter Topalov, Northeastern University, “Qualitative features of periodic solutions of KdV”  <a href="https://www.math.ias.edu/files/hofer/topalovab.pdf">abstract</a></li>
	<li>10:15 - 11:15  Jiansheng Geng, Nanjing University, “Invariant tori for the nonlinear lattice one-dimensional Schroedinger equations with real analytic potential”  <a href="https://www.math.ias.edu/files/hofer/gengab_0.pdf">abstract</a></li>
	<li>11:30 - 12:30  Massimiliano Berti, UNINA, “Quasi periodic solutions of Hamiltonian PDEs”  <a href="https://www.math.ias.edu/files/bertiab.pdf">abstract</a></li>
	<li>2:30 - 3:30     Ralph Saxton, University of New Orleans, “The generalized inviscid Proudman Johnson equation”  <a href="https://www.math.ias.edu/files/hofer/saxtonab_0.pdf">abstract</a></li>
	<li>4:30 - 5:30      Dongho Chae, Sungkyunkwan University, “On the blow-up problem for the Euler equations and the Liousville type results in the fluid equations”  <a href="https://www.math.ias.edu/files/hofer/chaeab.pdf">abstract</a></li>
</ul>
<h1 id="petertopalovhttp:www.math.neu.edutopalov:qualitativefeaturesofperiodicsolutionsofkdv"><a href="http://www.math.neu.edu/topalov/">Peter Topalov</a>: <em>Qualitative features of periodic solutions of KdV</em></h1>
<img src="http://www.math.neu.edu/topalov/topalov.jpg" alt="Peter Topalov" />

I need to do some detailed setup to expose the ideas I want to describe. We will discuss the KdV equation.

$$ q_t - 6 q q_x + q_{xxx} = 0.$$

Let’s impose periodic boundary conditions. We impose the initial condition $q|<em>{t=0} = q</em>0 \in H^N (T) $. This parameter $N$ will change at different times in the context of the talk, depending upon the theorem we are considering.

$$
H_{KdV} (q) = \int_0^1 (q^3 + \frac{(q_x)^2}{2} ) dx.
$$

What is the symplectic (more precisely the Poisson) structure? The phase space where the evolution will happen in $H^N$. For two functions $F,G: H^N \rightarrow R,$ we have the <em>Gardner bracket</em>
$$
{ F, G } = \int_0^1 \partial_q F \partial_x (\partial_q G) dx.
$$
(Ack….I am having trouble making curly brackets show up in the Gardner bracket even when I try to escape using a slash.)

Linearizing around $q=0$, we find $q_t =q_{xxx}$ which we can solve explicitly to find the evolution for the Fourier coefficient:
$$
\dot{\hat{q_k}} = - (2 k \pi i)^3 \hat{q_k} = (2 k \pi)^3 i \hat{q_k}.
$$
We can solve this directly to find
$$
\hat{q_k}(t) = \hat{q_k} e^{i (2k\pi)^3 t}.
$$
He draws a collection of complex Fourier planes and draws circles representing the motions of the Fourier coefficients.

Let’s see what the Poisson structure looks like when the dynamics are viewed in terms of the Fourier coefficients.

We compute the Gardner bracket of two Fourier coefficients:
$$
{ \hat{q_k}, \hat{q_l} } = \int_0^1 e^{-2 k \pi i x} (e^{-2 k \pi i x})’ dx = - 2 l \pi i \delta_{k, -l}.
$$
(missing curly brackets on left side.)

We fix attention to zero mean initial data. We will look at $H^N_0$ where the subscript reminds us that we are looking at the zero mean setting.

We define $z_k = \frac{\hat{q_k}}{\sqrt{|k| \pi}}$ and then observe that $z_k = x_k + i y_k$ gives us Darboux coordinates $x_k, y_k$.

We have a mapping $\Phi_L : H^N_0 \rightarrow  h^{N+\frac{1}{2}}$. Let’s see why this $\frac{1}{2}$. We take an element of phase space $q$ and apply $\Phi_L$ and this takes us to the associated Darboux coordinates $z_k = \frac{\hat{q_k}}{\sqrt{|k| \pi}}$ and the division by $|k|$ explains the $\frac{1}{2}.$

Remarks about this map $\Phi_L$:
<ol>
	<li>diffeomorphism</li>
	<li>canonical</li>
	<li>linearizes the flow</li>
</ol>
Return to KdV.

<strong>Theorem 1:</strong> $\exists ~ \Phi: H^N_0 \rightarrow h^{N + \frac{1}{2}}$ such that
<ol>
	<li>$\Phi$ is a diffeomorphism;</li>
	<li>$\Phi$ is canonical;</li>
	<li>$z_k (t) = z_k e^{i \omega_k (q) t}.$</li>
	<li>(New) $\Phi = \Phi_L + A; ~\Phi^{-1} = \Phi_L^{-1} + B$ where $A$ is 1-smoothing. What this means is that $A, B$ are bounded maps such that
$$A: H^N_0 \rightarrow h^{N + \frac{3}{2}};$$
$$ B: h^{N + \frac{1}{2}} \rightarrow H^{N+1}.$$</li>
</ol>
In 3. the phases depend only upon the initial data but for some reason I don’t want to write $q_0$ right now.

1., 2., 3. were proven by <strong>Kappeler-Poschel-Makarov</strong> for $N \geq 0$. For the interval $-1 \leq N \leq 0$, 1.,2.,3. was established by <strong>Kappeler-Topalov</strong>.

Item 4. is new and recently proven by <strong>Kappeler-Schad-Topalov</strong> (I didn’t catch the name…). This advance may be viewed as a globalization of a local statement obtained by <strong>Kuksin-Perelman</strong>.

Consider the KdV evolution moving through phase space. We can also consider the linearized evolution. We are interested in the difference.  Denote by $S_t (q)$ the KdV evolution. We can do something a little bit different:
$$
S_t (q) - \sum_{k \neq 0} (\hat{q_k} e^{i \omega_k (q) t}) e^{2k \pi i x} = R_t (q).
$$

<strong>Theorem 2:</strong>
<ol>
	<li>$R_t: H^N_0 \rightarrow H^{N+1}_0$ is continuous (even analytic on the Casimir $[q] = 0$).</li>
	<li>$\forall ~ q \in H^N_0$, we can consider the orbit $[R_t(q): t \in R] \subset H^{N+1}_0$ is relatively compact.</li>
	<li>$\forall ~ M &gt; 0, [R_t (q): t \in R, \| q \|<em>{H^N} \leq M] \subset H^{N+1}</em>0$ is bounded.</li>
</ol>
In particular, from 2., the norms are relatively bounded.

I want to say something about the proof. The overview involves an expansion of the flow maps using the structure in Theorem 1, item 4. The core of the analysis is in the spectral theory of the Shcrodinger operator.
<h1 id="jianshenggenghttp:math.nju.edu.cnjgeng:invarianttoriforthenonlinearlatticeone-dimensionalschroedingerequationswithrealanalyticpotential"><a href="http://math.nju.edu.cn/~jgeng/">Jiansheng Geng</a>: <em>Invariant tori for the nonlinear lattice one-dimensional Schroedinger equations with real analytic potential</em></h1>
(joint work with J. You an Z. Zhao)

We study a nonlinear Schrodinger equation on the lattice and show there exist quasiperiodic solutions.
$$
i \dot{q_n} + \delta( q_{n+1} - q_n) + V_n q_n + |q_n|^2 q_n = 0, n \in Z.$$

Here $\delta $ is small. $V_n (x) = V(n \tilde{\alpha} + x)$ with $V$ a nonconstant real analytic function on R/Z and $\alpha$ satisfying a Diophantine equation.

<a href="http://www.springerlink.com/content/8176276j72726392/"><strong>Eliasson 1997, Acta</strong></a>

Slides moving fast…

<strong>Theorem:</strong> For small enough $\delta$, this equation admits a Whitney smooth family of small-amplitude quasi-periodic solutions for a.e. $x \in R/Z$.

Also works in the nonlinear case.

Choffrut: What is Whitney smooth? A: Some discussion… Kaloshin: The function is defined on a Cantor set and you need to define what it means to be smooth. You can’t differentiate so you have to do something to understand smoothness….this is the idea of Whitney smooth.

Related works (Linear case):
<ul>
	<li><strong>Belissard-Lima-Scoppola</strong> 1983 CMP</li>
	<li><strong>Fröhlich-Spencer-Wittwer</strong> 1990 CMP</li>
	<li><strong>Chulaevsky-Dinaburg</strong> 1993 CMP</li>
	<li><a href="http://www.springerlink.com/content/8176276j72726392/"><strong>Eliasson</strong> 1997 Acta</a></li>
</ul>
Related works (Nonlinear case):
<ul>
	<li><a href="http://www.springerlink.com/content/tt4m894cndlv5y57/"><strong>Yuan</strong> 2002 CMP</a></li>
	<li><a href="http://www.sciencedirect.com/science/article/pii/S0167278908001942"><strong>Geng-Viveros-Yi</strong> 2008 Physica D</a></li>
	<li><a href="http://www.ems-ph.org/journals/show_abstract.php?issn=1435-9855&amp;vol=10&amp;iss=1&amp;rank=1"><strong>Bourgain-Wang</strong> 2008 JEMS</a></li>
	<li><strong>Geng-Zhao</strong> (preprint, 2011)</li>
</ul>
Töplitz-Lipschitz property
<ul>
	<li><strong>Eliasson-Kuksin</strong> 2010</li>
	<li><strong>Geng-Xu-You</strong> 2011</li>
</ul>
Slides are quite dense, too technical for me to convey here. Abstract KAM theorem.
<h1 id="massimilianobertihttp:www.dma.unina.itberti:quasiperiodicsolutionsofhamiltonianpdes"><a href="http://www.dma.unina.it/berti/">Massimiliano Berti</a>: <em>Quasi periodic solutions of Hamiltonian PDEs</em></h1>
<h2 id="nonlinearwaveequation">Nonlinear Wave Equation</h2>
$$ (NLW):~ u_{tt} - \Delta u + V(x) u = \epsilon f( \omega t, x, u).$$

$\omega$ diophantine.

<strong>Question:</strong> Do $\exists$ quasiperiodic solutions of NLW ro $\epsilon \neq 0$?

Linear wave equation: ($\epsilon = 0$.)

Solutions are built by superposition.
<ul>
	<li>Eigenfunctions are orthonormal in $L^2$: “Normal Modes”</li>
	<li>Eignevalues $\lambda_j \rightarrow + \infty$: the $\sqrt{\lambda_j}$ are the “Normal frequencies”.</li>
</ul>
All these linear soutions are periodic. Their superpositions are quasiperiodic. Do these persist when we turn on the nonlinearity.

We look for quasiperiodoc solutions. This leads to an equation for qp solutions:

$$
(\omega \cdot \partial_\phi)^2 u - \Delta u _ V(x)u = f.
$$

We can approach this existence question as a bifurcation problem.

We make a NON-RESONANT assumption:

$$ | (\omega \cdot l)^2 - \lambda_j | \geq \frac{\gamma}{1 + |l|^\gamma}, ~ \forall (l,j). $$
The inverse operator is unbounded so the classical implicit function theorem fails. We need a replacement, some kind of Quadratic scheme.

We use a Nash-Moser IFT: Newton method + “smoothing”

The advantage is the rapid convergence. The disadvantage is that we have to invert in a whole neighborhood of the expected solution.
<h2 id="literature">Literature</h2>
$d=1$
<ul>
	<li><strong>Kuksin 89, Wayne 90</strong>; 2nd order Melnikov non-resonance conditions OK. Dirichlet conditions to ensure simplicity of eignevalues.</li>
	<li><strong>Craig-Wayne 93</strong> periodic solutions</li>
	<li><strong>Bourgain 94</strong> quasiperiodic solutions</li>
</ul>
Lyapunov-Schmidt, f analytic, Netwon Method. 1st order Melnikov conditions.

$d \geq 2$
<ul>
	<li>Eigenvalues of $\Delta + V(x)$ appear in clusters of increasing size.</li>
	<li>If $d \geq 2$, the eigenfunctions of $-Delta + V(x)$ are NOT localized wrt exponentials! (**Feldman-Knönner-Trubowitz**)</li>
</ul>
Often, these issues motivate the study of “pseudo-PDEs.”

Newton Method
<ul>
	<li><strong>Bourgain 98 Annals 05 Annals</strong></li>
	<li><strong>Wang 10, 11</strong></li>
</ul>
KAM theory
<ul>
	<li>…Processi, Berti…Craig-Wayne…ack slide changged.</li>
</ul>
<h2 id="nash-moser">Nash-Moser</h2>
<strong>Eliasson 89</strong>

<strong>Berti-Bolle 2011</strong> (to appear in JEMS)

<strong>Existence:</strong> (Summary of statements; slides are more precise)
Under some conditions on $f$, there exists a Cantor like set $C_\epsilon$ of asymptotically full Lebesgue measure. “This is a classical KAM-like statement.”

<strong>Regularity:</strong>

The Cantor-like set is not technical, e.g. <strong>CKSTT 2010 Inventiones</strong>.

Pre-assigned direction of tangential frequencies
<ul>
	<li><strong>Geng-Ren 2010</strong></li>
	<li><strong>Berti-Biasco CMP 2011</strong></li>
	<li><strong>Bambusi-Berti-Magistrelli, JDE 2011</strong></li>
</ul>
Weaker non-resonance condition

simpler technique

Many of these results should carry over to spheres, Zoll manifolds, Lie groups, homogenous spaces: <em>symmertries and properties of eigenfunctions and eigenvalues</em> are key properties! Related to Birkhoff normal form results by Bambusi, Delort, Grebert, Szeftel for spheres and Zoll manifolds.

For periodic solutions, see <strong>Berti-Procesi Duke 2011</strong>
<h2 id="ideaofproof">Idea of Proof</h2>
Small divisors.

Töplitz matrices.

Difficulties:
<ul>
	<li>T has only a polynomial decay off the diagonal.</li>
</ul>
Smoothing operators; finite-d projectors. TAME estimates are needed. We need estimates on the inverse operator on high regularity Sobolev spaces. Counterexaple of <strong>Lojaciewitz-Zehnder</strong>! This example shows identifies a parameter boundary in the Newton iteration scheme.

Step 1. $L^2$-estimates: Lower bounds for the eigenvalues.

Step 2. “Separation Properties” of small divisors

Locations where the divisors are small become more and more rare. There emerge “irrational” conditions on the slope $\omega$. These conditions are not needed for the Schrödinger equation. The dispersive relationship is different and helps you here.
<h2 id="kam">KAM</h2>
Nash-Moser via the 1st Melnikov conditions. This is in some sense the minimal assumption. This approach works well in case of multiple eigenvalues. However, it has the disadvantage that it requires studying the linearized equation with non-constant coefficients.

Other strategy: impose stronger nonresonant conditions of 2nd Melnikov type (as usual in KAM). This has the advantage that we have a linearized equation with constant coefficients. There exists a torus and a reducible normal form.

Question: Do quasiperiodic solutions persist for nonlinearities which involve derivatives? Important physical applications.
<ul>
	<li><strong>Kuksin 1998</strong></li>
	<li><strong>Kappeler-Pöschel 2003</strong></li>
	<li><a href="http://www.springerlink.com/content/73641x366105h81w/"><strong>Liu-Yuan 2010</strong></a> for Hamiltonian DNLS (Benjamin-Ono)</li>
</ul>
<strong>Theorem (Berti-Biasco-Procesi 2011):</strong> DNLW has a Cantor-like family of quasiperiodic solutions. These qp solutions have zero Lyapunov exponents and the linearized equations can be reduced to constant coefficients.

Ideas of proof. View this as an infinite dimensional Hamiltonian system. Use conservation of momentum (<strong>Geng-You</strong>).

Birkhoff Normal form step, reduction to action-angle variables. Then apply an abstract infinite-d KAM theorem.

The Hamiltonian vector field is BOUNDED and “Quasi-Töplitz”.
<ul>
	<li><strong>Procesi-Xu 2011</strong> (introduced Quasi-Töplitz)</li>
	<li><strong>Eliasson-Kuksin</strong> (similar notion Töplitz-Lipschitz)</li>
</ul>
<h2 id="quasi-tplitzfunctions">Quasi-Töplitz functions</h2>
see slides….there is an algebraic closure property of this class under the normal form manipulations.
<h2 id="dnlw">DNLW</h2>
Not Hamiltonian but “reversible” PDE. This is a relaxed setting but which rules out certain nonlinearities like $y_t^3$.

Real coefficients condition which excludes $y_x^3$.

Moser, Arnold, Sevriuk. Algebra of classical reversible KAM theory works out on this PDE as well. The asymptotic expansion of the normal frequencies controlled similarly as in the Hamiltonian case, in analogy with the quasi-Töplitz framework.
<h1 id="ralphsaxtonhttp:mathfac.math.uno.edursaxton:thegeneralizedinviscidproudmanjohnsonequation"><a href="http://mathfac.math.uno.edu/~rsaxton/">Ralph Saxton</a>: <em>The generalized inviscid Proudman Johnson equation</em></h1>
<img src="http://mathfac.math.uno.edu/~rsaxton/rs_clifford07.jpg" alt="Ralph Saxton" />

(joint work with Aleajandro Sarria)

This is the Proudman-Johnson (PJ) equation:

$$ (\partial_t + u \partial_x) \partial_x u = \lambda u_x^2 - (\lambda+1) \int_0^1 u_x^2 .$$

This equation comes from the n-dimensional Euler equations. The solutions we consider coming from Euler are unbounded as we go toward spatial infinity so these are infinite energy. He describes some further modeling assumptions culminating into a collapse of Euler into the Proudman-Johnson equation.

History:
<ul>
	<li><strong>Childress, Lerley, Spiegel, Young 1989</strong></li>
	<li><strong>Saxton-Tiglay 2008, Okamoto 2009</strong></li>
	<li><strong>Okamoto-Zhu 2000</strong></li>
	<li><strong>wunsch 2009</strong></li>
	<li><strong>A. Constantin 2000</strong></li>
</ul>
Diverse phenomena as $\lambda$ varies.
<h1 id="donghochaehttp:wiz.skku.educhae:ontheblow-upproblemfortheeulerequationsandtheliouvilletyperesultsinthefluidequations"><a href="http://wiz.skku.edu/chae/">Dongho Chae</a>: <em>On the blow-up problem for the Euler equations and the Liouville type results in the fluid equations</em></h1>
<img src="http://cau.ac.kr/~dchae/dchae.bmp" alt="Dongho Chae" />

Contents
<ol>
	<li>On the blowup problem for Euler</li>
	<li>Liouville type equations for fluids</li>
</ol>
<h2 id="eulerblowupproblem">Euler Blowup Problem</h2>
<strong>Euler 1757</strong>

Euler equation on $R^N$.

<strong>Kato, Temam, Bouguignon-Brezis</strong>. Local existence in $H^m (R^3)$ with $m&gt;5/2$. Do singularities form?
<ul>
	<li><strong>Beale-Kato-Majda 84</strong> Critereon: If there is blowup at time $ {T^*}$ then$$
\int_0^{T^*} \| \omega (s) \|_{L^\infty} ds = \infty.
$$</li>
	<li><strong>Constantin-Fefferman-Majda 1996</strong> critereon.</li>
	<li>Refinements using Triebel-Lizorkhin type spaces. Interpolations.</li>
</ul>
On the self-similar blowup scenarios:
<ul>
	<li>Self-similar blowup is a popular scenario in search for finte time singularity in nonlinear PDE.</li>
	<li>E has a scaling property:
$$ v^{\lambda, \alpha} = \lambda^\alpha v(\lambda x, \lambda^{\alpha + 1}t), ~ p = \lambda^{2\alpha} (same).$$</li>
</ul>
We consider the possibility of self-similar blowups for E.

Energy conservation suggests choosing $\alpha = \frac{N}{2}

Substitute a self-similar ansatz into E to obtain a system called SSE, the self-similar Euler equation. In the Navier-Stokes case, this system is called the <em>Leray system</em>. Leray asked if there exist self-similar blowup solutons for the Navier-Stokes equations in 1930.

Negative answers to Leray’s questions.
<ul>
	<li>$V \in L^3 (R^3)$. <strong>Necas-Ruzicka-Sverak 1996</strong></li>
	<li>$V \in L^p (R^3), p&gt;3$. <strong>Tsai 1998</strong>.</li>
	<li>Theproofs rely upon maximum principle based arguments, which are not available in the context of the Euler equation.</li>
</ul>
<strong>Theorem (Chae 2007):</strong>

Let $V$ be a solution of SSE satisfy
<ol>
	<li>$V \in [C^1 (R^3)]^3$ vanishing near infinity.</li>
	<li>There exists $p_1 &gt;0$ such that $\Omega - \nabla \times V \in \bigcap_{0&lt;p&lt;p_1} L^p (R^3).$ Then $V=0.$</li>
</ol>
The proof of this theorem used the “back to label map” due to Constantin. Recently, I found a much simpler elementary proof.

<a href="http://arxiv.org/abs/1201.6009">Chae-Shvydkoy 2012</a>

This is the Euler version of the Navier-Stokes $L^3$ result of Necas-Ruzicka-Sverak.

Nonexistence of asymptotically self-similar blowup <strong>Giga-Kohn 1985</strong>. See <strong>Chae 2007</strong>.
<h2 id="liouvilletyperesultsfornavier-stokes">Liouville Type Results for Navier-Stokes</h2>
Compare with <strong>Galdi</strong>. Slides are very detailed, provides a survey of the field.