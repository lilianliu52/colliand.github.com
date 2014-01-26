---
layout: post
category : lessons
tags : [Notes, USA, IAS]
comments: false
---


<!-- Processed by MultiMarkdown -->

<a rel="attachment wp-att-1031" href="http://blog.math.toronto.edu/colliand/2012/03/17/ias-workshop-on-symplectic-dynamics-2-friday/fuld_from_simonyi/"><img class="alignnone size-medium wp-image-1031" src="http://blog.math.toronto.edu/colliand/files/2012/03/fuld_from_simonyi-300x200.jpg" alt="" width="300" height="200" /></a>

<a href="http://www.math.ias.edu/">IAS School of Mathematics</a>

&nbsp;

<a href="http://www.math.ias.edu/wsd2">Workshop web page</a>
<h2 id="friday:2012-03-16">Friday: 2012-03-16</h2>
<ul>
	<li>9:00 - 10:00    James Colliander, University of Toronto, “Big frequency cascades in the cubic nonlinear Schroedinger flow on the 2-torus”  <a href="https://www.math.ias.edu/files/hofer/collianderab.pdf">abstract</a></li>
	<li>10:15 - 11:15   Marcel Guardia, IAS, “Growth of Sobolev norms for the cubic defocusing nonlinear Schroedinger equation in polynomial time”  <a href="https://www.math.ias.edu/files/hofer/guardiaab.pdf">abstract</a></li>
	<li>11:30 - 12:30  Yann Brenier, University of Nice, “Approximate geodesics on groups of volume preserving diffeomorphisms and adhesion dynamics”  abstract</li>
</ul>
<h1 id="jamescollianderhttp:www.math.toronto.educolliand:bigfrequencycascadesinthecubicnonlinearschroedingerflowonthe2-torus"><a href="http://www.math.toronto.edu/colliand">James Colliander</a>: <em>Big frequency cascades in the cubic nonlinear Schrödinger flow on the 2-torus</em></h1>
(chalk talk)

(joint work with <a href="http://www.math.umn.edu/~keel/">M. Keel</a>, <a href="http://www-math.mit.edu/~gigliola/">G. Staffilani</a>, <a href="http://www.math.sci.hokudai.ac.jp/~takaoka/index_en.htm">H. Takaoka</a>, <a href="http://www.math.ucla.edu/~tao/">T. Tao</a>)

I prepared slides but decided to give a chalk talk. The slides are located here: <a href="http://uoft.me/nls-cascade">http://uoft.me/nls-cascade</a>. The paper discussed in this talk is <a href="http://www.springerlink.com/content/v727q748p07r264g/">located here</a>.

(See also: The thesis of <a href="http://www.math.ucla.edu/~zhani/">Zaher Hani</a> has advanced along these lines and is surveyed on <a href="http://www.math.sciences.univ-nantes.fr/handdy/sites/fr.handdy/files/HANDDYhani.pdf">his slides</a> from the <a href="http://www.math.sciences.univ-nantes.fr/handdy/content/workshop-handdy-2011">Ilde de Berder Workshop</a>.)

The construction of the frequency civilization is partly conveyed by the following cartoon. Notice that the underachieving child frequency in the cartoon is always sent to the zero frequency. This violates the injectivity requirements used in our construction of the set $\Lambda$.

<img src="http://www.math.toronto.edu/colliand/images/cartoon_lambda.gif" alt="cartoon_construction" />

The next cartoon is meant to convey a traveling wave through the generations in the civilization. This wave is constructed by concatenating heteroclinic orbits in the toy model evolution.

<img src="http://www.math.toronto.edu/colliand/images/wave_generations.gif" alt="wave_generations" />

The idea that the orbits could be concatenated reminded my coauthors of this famous commercial:

<a href="http://www.youtube.com/watch?v=KXA8g90g7so">http://www.youtube.com/watch?v=KXA8g90g7so</a>

&nbsp;

&nbsp;
<h1 id="marcelguardia:growthofsobolevnormsforthecubicdefocusingnonlinearschroedingerequationinpolynomialtime">Marcel Guardia: <em>Growth of Sobolev norms for the cubic defocusing nonlinear Schrödinger equation in polynomial time</em></h1>
<a rel="attachment wp-att-1027" href="http://blog.math.toronto.edu/colliand/2012/03/17/ias-workshop-on-symplectic-dynamics-2-friday/guardia_small/"><img class="alignnone size-medium wp-image-1027" src="http://blog.math.toronto.edu/colliand/files/2012/03/Guardia_small-300x225.jpg" alt="" width="300" height="225" /></a>

(joint work with Vadim Kaloshin; we have a preprint; <a rel="attachment wp-att-1045" href="http://blog.math.toronto.edu/colliand/2012/03/17/ias-workshop-on-symplectic-dynamics-2-friday/guardia_iastalk/">slides from the talk; 32 pages</a>)

This talk is strongly related with the previous talk.

$NLS_3^+ (T^2)$. Energy and Mass are conserved. The problem is globally well-psed in time <strong>Bourgain 1993</strong>.
<h2 id="transferofenergy">Transfer of Energy</h2>
<ul>
	<li>Fourier series of $u$.</li>
	<li>Can we have a transfer of energy to higher and higher modes ass $ t \rightarrow + \infty$?</li>
	<li>This is quantified with the growth of Sobolev norms.</li>
</ul>
We need to move mass toward high frequencies in a careful way to satisfy the mass and energy constraints.

<strong>Theoreom (Bourgain 1993):</strong> As $t \rightarrow + \infty$, the $H^s$ norm is upper bounded by $\leq t^{2(s-1)+} \| u(0) \|_{{H^s}}.$

This result has been improved or applied to other Hamiltonian PDEs by various authors.

<strong>Question (Bourgain 2000):</strong> Are there solutions $u$ such that for $ s&gt;1$ such that
$$\| u(t)\|<em>s \rightarrow \infty $$
as $ t \rightarrow + \infty? $ Moreover, he conjectured that the growth should be subpolynomial in time: $ \| u(t)\|</em>{H^s} \ll t^\epsilon$.

The second part was partly conjectured because of insights related to Nekoroshev type theorems for NLS.

<strong>Kuksin</strong> studied the growth of Sobolev norms for NLS for large initial condition. For such data, a change of coordinates recasts the dynamics into

$$
- i \dot{w} = - \delta \Delta w + |w|^2 w, ~ \delta \ll 1.
$$

<strong>Theorem (CKSTT 2010):</strong> $\exists $ big frequency cascades in the $NLS_3^+ (T^2)$ flow.

The solutions have small intial mass and energy. They remain small as time involves whereas the s-Sobolev norm grows considerably.

<strong>Theorem:</strong> (long statement, I’m reading instead of typing.)

The mass is small but the $H^s$ norm is initially large. They can then grow it up to any big threshold over a polynomially related time interval.

Remark: One might view this equation as a perturbation (when the data is small) of the (integrable) linear Schr"odinger. It is well know that the Nekoroshov type results for PDEs often loses the exponential estimates and becomes polynomial. Our result is consistent with this.

Remark: Our result deals with a different regime than the Bourgain subpolynomial conjecture. Our result is rather fast, but it could perhaps slow down over infinite time. Our construction involves a finite number of modes. If we try to build something on an infinite number of modes, the transfer mechanism might slow down.

Comments:
<ul>
	<li>One can tensor this up to obtain similar results on $T^d, d \geq 2$.</li>
	<li>We can obtain more detailed information about the distribution of the Sobolev norm of the solution $u$, among its Fourier modes when $t = T$. In particular, the high Sobolev norm is carried by two high achievers at the last stage. The high Sobolev norm is essentially localized in two modes.</li>
</ul>
Main Ideas in the Proof:
<ul>
	<li>$I$-team introduced a finite-d toy model.</li>
	<li>This toy model approximates well certain solutions of NLS</li>
	<li>Our contribution is the analysis of the toy model. Using dynamical system tools, and a careful choice of the initial conditions, we find a faster motion.</li>
	<li>The solutions of NLS can be proven to approximate well the solutions for the toy model for long time.</li>
</ul>
Reduction to the toy model.
<ul>
	<li>$FNLS$</li>
	<li>$RFNLS$</li>
	<li>Construct $\Lambda$.</li>
	<li>Toy Model ODE</li>
</ul>
For $N$ big enough, the set $\Lambda$ can be chosen to have the “wide diaspora property.” This is partly why we don’t have an infinite cascade. The construction only involves a finite number of modes. We want to quantify everything in terms of the number $N$ of generations. At the end we have $N \thicksim \log K$.  We have to quantify everything.

<strong>Toy Model Theorem:</strong> There exists an orbit in the toy model which moves from the first generation to the last. Their statement includes quantifications! They compute the time of this transfer process.

To make things happen quickly, they want to make the transfers as fast as possible. This development uses a different orbit construction than the one performed by CKSTT.

Dynamics of the Toy Model:
<ul>
	<li>ODE explicitly written out.</li>
	<li>Each 4-d plane is invaraint.</li>
	<li>Dynamics in each 4-d plane is given by a simple Hamiltonian involving nearest neighbor interactions.</li>
</ul>
Nice picture of invariant planes intersecting to form something like a polyhedra with a curve following along nearby invariant lines. “Of course, we are not in the plance but we are nearby it.” Of course to do this, we need to understand the dynamics in each of these planes. To obtain these orbits, we use hyperbolicity. But these planes have certain normal positive Lyapunov exponents so one has to be very careful. If we just move away from these planes, we lose control.

Dynamics in $L_j$:
<ul>
	<li>To construct such orbits, we need to understand dynamics in each $L_j$.</li>
	<li>Hamiltonian $h_j$ and $M_j(b_j, b_{j+1}) = |b_j|^2 + |b_{j+1}|^2$…..ack slide changed.</li>
	<li>Contains two periodic orbits.</li>
	<li>Periodic orbits in $L_j$ are hyperbolic.</li>
	<li>Stable and unstable invariant manifolds of the periodic orbits coincide.</li>
	<li>Call $\gamma_j$ the heteroclinic connection between the two dimensional manifold asymptotic to $T_j$ as $ t \rightarrow - \infty$ and asymptotic to $T_{j+1}$ as $ t \rightarrow \infty$.</li>
</ul>
Key Problem: The Shadowing

(nice picture)
<ul>
	<li>We put sections transveral to the flow.</li>
	<li>We study local maps: dynamics close to the periodic orbits $T_j$. Global maps: study dynamics close to the heteroclinic connections $\gamma_j$.</li>
</ul>
Local and Global Maps:
<ul>
	<li>Shadowing for global map is basically applying (refined) Gronwall estimates.</li>
	<li>Local map is more delicate: periodic orbits are of mixed type. Hyperbolic eigenvalues are resonant.</li>
	<li>This resonance complicates the analysis of the local maps.</li>
</ul>
We need to choose very carefully which orbits we study.

The Model Problem:
<ul>
	<li>After some reductions, we have a Hamiltonian of the form:</li>
</ul>
$$
H(p,q) = p_1 q_1 + p_2 q_2 + H_4 (p,q)
$$
where $H_4$ is a degree 4 homogenous polynomial, the variables “1” correspond to the variable $b_{j-1}$ ….slide changed.

Analysis of map from a section $\Sigma_+$ to $\Sigma_-$.

Dynamics of the linear saddle (Kill the $H_4$ and see what happens.).

Dynamics of the resonant saddle:
<ul>
	<li>System is not well approximated by its linear part due to the resonance.</li>
	<li>For typical initial conditions, we have a resonat affect creating logarithmic (in $\delta$ ) corrections to the transfer across hetereoclinic connections.</li>
	<li>We need $~N$ transitions.</li>
	<li>The number of logarithms becomes exponential in $N$.</li>
	<li>We need to stay close to the periodic orbits to control the shadowing</li>
	<li>This implies we need to start….slide change</li>
</ul>
We use the beautiful <strong>Shilnikov trick</strong>. The worst term that was developing with logarithms is now computed more accurately in terms of some function $g(p_0, q_0)$. This transfers the resonant saddle dynamics into essentially the dynamics of the linear saddle, provided that we carefully choose the domain of the map. This is kind of delicate and needs to be iterated through compositions.

Composing the local and the global maps:
<ul>
	<li>We need to compose the local and global maps.</li>
	<li>We define sets $U_j$ in the transversal secions and we show that the dynamics moves one into the other. (This is the “perfect shot”.)</li>
	<li>To avoid deviations at each local map, we need to impose a restriction at every step.</li>
	<li>“Product-like” step.</li>
</ul>
Product-like structure sets.
<ul>
	<li>We start with a polydisk.</li>
	<li>At each step, we impose a condition on the mode $b_{j-1}$.</li>
	<li>Inductively, we rstrict the domain on previous domains involving conditions on previous mode involving the Shilnikov function $g$.</li>
	<li>Since the restricitons involve a different mode at each step, the conditions are compatible.</li>
</ul>
Composing the local and global maps produces the toy model result. The detailed discussion partly explains the time quantification.

Approximating solutions of NLS:
<ul>
	<li>Last step obtain a solution of NLS close to the solution of the toy model.</li>
	<li>We modify the set $\Lambda$ from the $I$-tema so that the modes out of $\Lambda$ only gets influenced by few modes in $\Lambda$.</li>
	<li>Each $b_j$ is excited only for a short period of time.</li>
	<li>A mode out of $\Lambda$ only receives mass from $\Lambda$ during a short time.</li>
	<li>This implies that the spreading of mass to modes out of $\Lambda$ is very slow.</li>
	<li>We obtain an orbit for NLS that undergoes the growth of Sobolev nroms in polynomial time.</li>
</ul>
<h1 id="yannbrenier:approximategeodesicsongroupsofvolumepreservingdiffeomorphismsandadhesiondynamics"><a href="http://math.unice.fr/~brenier/">Yann Brenier</a>: <em>Approximate geodesics on groups of volume preserving diffeomorphisms and adhesion dynamics</em></h1>
(chalk talk; but here are <a rel="attachment wp-att-1036" href="http://blog.math.toronto.edu/colliand/2012/03/17/ias-workshop-on-symplectic-dynamics-2-friday/ias-2012-dust/">the slides</a>.)

It’s a good time for all of us to thank the organizers for this meeting. (Applause!)

Related to a question posed by <strong>Shnirelman</strong> from 1985.

System of interacting particles along the real line with sticky collisions. When the particles hit, they merge and continue with the same momentum. This is an inelastic, sticky collision. This is clearly
<ol>
	<li>dissipative</li>
	<li>nonreversible in time</li>
</ol>
<strong>Shnirelman’s Question (1985)</strong>: Can we modify the action principle to handle these dissipative collisions?

Unfortunately, the paper is hard to find. You can think of the collision in a higher dimensional space and keep track of the energy in the extra variables.

<strong>G. Wolansky (2008 ?)</strong>

In this talk, I want to provide some ideas that come from ideal fluids. This seems strange because this problem is highly compressible, etc.

This talk is about a proposal for a modified action suggested by ideal fluid mechanics.

Arnold’s geometric interpretation (1966) of Euler equation for incompressible fluids (1755).

Let $D = [0,1]^3$. Let $VPM (D) = [ volume ~ preserving ~ maps ~ of ~ D]$. This may be viewed as a subset of $H = L^2 (D, R^3)$. Geodesics along VPM are (formally) the solutions of the Euler equations.

There is a discrete subset of $VPM (D)$ are the permutation maps $S =P_N (D)$. Partition the unit cube into a collection of $N$ subcubes $Q_i$ each with center of mass $A_i$. You would like to do some kind of discrete fluid mechanics by exchanging these cubes. There is a folklore of approximating geodesics with these kinds of maps. This is used in some works in computational geometry. How to define approximate geodesics along $P_N (D)$?

More generally, let $H$ be a Euclidean (or Hilbert) space. You have a closed bounded subset $S$. Introduce a potential
$$\Phi [x] = \frac{d^2}{2} (x,s) = \inf_{s \in S} \frac{|x-s|^2}{2} = \frac{|x|^2}{2} - R(x).
$$
Here $R$ is the Legendre transform:
$$
R(x) = \sup_{s \in S} (x|s) - \frac{1}{2} |s|^2.
$$
Convex, Lipschitz, usually not smooth.

Approximate minimizing geodesics are found by minimizing between two given points $A, B \in H$ by
$$
\int_0^1 (\frac{1}{2} |\frac{dx}{dt} (t)|^2 + \frac{1}{2\epsilon} \Phi [x(t)] ) dt
$$
satisfying $X(0) = A, X(1) = B$. If $S$ is a smooth manifold this converges to geodesics <strong>Rubin-Ungar 1957</strong> (Yann’s birth year!).

These ideas were applied by <strong>David Ebin</strong> to fluids.

A simpler example than the one appearing in Shnirelman’s question…

Take $H = R^2$. Let $S$ be the St. George cross. He writes the coordinate axes in $R^2$ in red and forecasts that a joke will soon come up…

Whenever $\Phi$ is smooth about $X$, we have $\nabla \Phi (x) = x - \pi_S (x)$ (the closes point to $x$ inside $S$, not necessarily unique). The bad set $N$ where differentiability fails is both meager and has lebesgue measure zero in finite-d case. This has to do with the regularity of Lipschitz functions.

What is the bad set related to the St. George cross? Of course, it is the St. Andrew cross, the flag of Scotland! (He draws that in blue.) You can also reverse the picture so that the bad set becomes the St. George cross if you prefer to view it that way…..

If $x \in H \backslash N$, we have $\phi (x) = \frac{1}{2} |x - \pi_S (x)|^2 = \frac{1}{2} |\nabla \phi (x)|^2$.

Look at the action (for simplicity $\epsilon = 1$) for a “good curve” $ t \rightarrow x(t)$. Namely a curve for which $x(t) \in H \backslash N$ for a.e. time, the action reads
$$
\int_0^t (\frac{1}{2} |\frac{dx}{dt}|^2 + \frac{1}{2} |\nabla \Phi [x(t)]|^2 ) dt.
$$

So, obvious minimizers are those good curves that satisfy the first order equation
$$
(FO) ~ \frac{dx}{dt} = \nabla \Phi [x] = x - \nabla R [x].
$$

This is a so-called <em>gradient flow of a Lipschitz convex function</em> (up to the first term which can be absorbed). These objects have been studied.

The theory of maximal monotone operators does the job (cf <strong>H. Brezis book</strong>) in the sense that this is completely well-posed in $H$. We know from that theory that $ x \in C(R_+; H)$, Lipschitz in $t$, and
$$
\frac{dx}{dt} (t+0) = x(t) - {d^0 R[x]}
$$
which is sometimes called the minimal selection gradient or “mean” gradient (studied in the Italian school).

Example. Differentiate $|x|$. The subgradient fills in the vertical line. The minimal gradient has value zero at $x=0$. This is a nice theory but it gives us very bad curves.

If you start on this St. George cross example, he describes the dynamics and interprets this as a dissipative mechanism. This has little to do with the action principle but it does have dissipation. So, we might take some inspiration from this example….this is a proposal for a modified action.

Modified action:

$$
\int_0^t \frac{1}{2} |\frac{dx}{dt} - d^0 \Phi [x(t)]|^2 dt.
$$
Minimizers of the modified action are very likely to be bad curves.
<blockquote>Some rats were confined in a box by electric shocks and another which is very hot. But, if you dig a small channel between the other two boxes. It turns out the rats can survive longer by moving back and forth between the two boxes. I hope it is not a true story….</blockquote>
The dissipation is not incompatible with the arrow of time if you order the data.

Now, I’d like to go back to permutations and fluids. What kid of equation do I get?

Remember the box, broken up into the subcubes. Consider the set $S$ to be the permutations of all the centers. Let $H$ denote $R^{dN}$. In the $d=1$ case, you get a friendly approximate geodesic equation through the classical (nonmodified) action. We are then describing $N$ particles on the line.
$$ \epsilon \frac{d^2 x_i}{d t^2} = x_i - \frac{1}{2N} \sum_{j=1}^N ~{\mbox{sgn}} (x_i - x_j).
$$
This is like a gravitating parallel pancackes according to Newton gravity plus a repulsive background. This type of model was studied by people like Zeldovich. The repulsive effect is natural in that context. By approximating the incompressible Euler this way, it is nice that you get a model that is reasonable from the point of gravity.

In higher dimensions, the model is NOT consistent with Newtonian gravitation but is instead consistent with a Monge-Ampere correction to Newton’s gravitation. You get something like $\Delta \phi = \rho -1$ and then eventually find something like $ {\mbox{det}} (I + D^2 \phi) = \rho.$ I am not yet certain if this is geometrically reasonable. It is related to Born-Infeld correction to Maxwell’s equations.

So, what is the point? If you modify the action, you can recover interaction with sticky collision.

This is the so-called “Dust” in the Russian literature. These are elementary ideas that explain why matter has clumped in cosmology. Sluggish motions in the early universe moves like honey. Tiny fluctuations of qunatum origin and these create a Jeans instability which tends to concentrate matter. This is at a very large scale and concentrated on a llower dimensional fractal set.