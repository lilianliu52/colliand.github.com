---
layout: post
category : lessons
tags : [Notes, USA, IAS]
---
<!--   Created by James Colliander on 2011-09-04.   Copyright (c) 2011 University of Toronto. All rights reserved.     -->

I'm participating in a workshop at the Institute for Advanced Study on Symplectic Dynamics. This is part of the special concentration this year organized by Helmut Hofer. I'll try to write notes on the talks I hear. Apologies to the speakers for typos and misquotations.... Comments (pending approval) are open for suggestions and edits.

<a href="http://www.math.ias.edu/">IAS School of Mathematics</a>

<img src="https://www.math.ias.edu/pictures/math/simonyi-blossoms.jpg" alt="Simonyi Hall" />

<a href="http://www.math.ias.edu/wsd2">Workshop web page</a>
<ul>
	<li>10:15 - 11:15  Peter Constantin, Princeton University, “Long time, vanishing viscosity limits”  <a href="https://www.math.ias.edu/files/hofer/constantinab.pdf">abstract</a></li>
	<li>11:30 - 12:30  Steve Preston, University of Colorado, “The inextensible string as a toy model of fluids”  <a href="https://www.math.ias.edu/files/hofer/prestonab.pdf">abstract</a></li>
	<li>2:30 - 3:30       Emanuele Caglioti, University of Rome, “Long time behavior of solutions of Vlasov-like equations”  <a href="https://www.math.ias.edu/files/hofer/cagliotiab.pdf">abstract</a></li>
	<li>4:30 - 5:30       Roberto Camassa, University of North Carolina, “Large amplitude internal waves and their stability”  <a href="https://www.math.ias.edu/files/hofer/camassaab.pdf">abstract</a></li>
</ul>
<h1 id="peterconstantinhttp:www.math.princeton.educonst:longtimevanishingviscositylimits"><a href="http://www.math.princeton.edu/~const/">Peter Constantin</a>: <em>Long time, vanishing viscosity limits</em></h1>
<img src="http://www.math.princeton.edu/~const/pn.jpg" alt="Peter Constantin" width="384" height="288" />

(pdf slides)
<h2 id="navier-stokes">Navier-Stokes</h2>
Navier-Stokes equations. $\nu$ multiplies the damping term. Studying it in $R^d$ or $T^d$, $d=2,3$. We are interested in $T \rightarrow \infty$ and $\nu \rightarrow 0$. (Reynolds number $\frac{UL}{\nu}$.)

Limits: selected stationary statistical solutions.

$$\lim_{Re \rightarrow \infty} \lim_{T \rightarrow \infty} \frac{1}{T} \int_0^T \phi( S^{NS} (t) ) dt.$$

Anomalous dissipation of energy:

$$
\lim_{\nu \rightarrow 0} \lim_{T \rightarrow \infty} \frac{\nu}{T} \int_0^T \int_{R^3} |\nabla u (x,t)|^2 dx dt = \epsilon &gt; 0.$$

(<strong>K41</strong>)
<h2 id="dnavierstokes">2d Navier Stokes</h2>
No anomalous dissipation of energy. Enstrophy balance. Anomalous dissipation of enstrophy? <strong>Kraichnan 68</strong>: Yes. <strong>Bernard 00</strong>: add (extra…to be described…discussion….friction from the bottom) damping and then no.

<strong>Constantin-Ramos 07</strong>: Bernard was right. Heuristics.

We are talking about weak solutions. 2 reasons to talk about these. The singularities really describe the phenomena, e.g. shocks in hyperbolic conservation laws. Deduce from the few conservation laws that solutions exist and they are nice and smooth but we can’t so we content ourselves with what we can build.
<h2 id="activescalars">Active Scalars</h2>
$$\partial_t \theta + u \cdot \nabla \theta = 0$$

Examples: 2d Euler, SQG.

$$ u = \Lambda^\gamma R^\perp \theta. $$

(Here $R$ is the Riesz transform, $\Lambda = \sqrt{-\Delta}$.)

Weak solutions for SQG. <strong>Resnick 95</strong>. Almost Lipschitz on $L^2$. Euler and NS does not have this weak continuity property. We don’t have uniqueness. If you have unique weak solutions, then you are golden. I’m going to talk about statistical solutions eventually.

<strong>Theorem (Chae-C-Cordoba-Gancedo-Wu):</strong> Let $\theta_0 \in L^2 (T^2)$. There exists a global $L^2$-weak solutions of the generalized SQG.

….too fast to type. Generalizes result of Resnick. Remarks…fast. <strong>Friedlander-Vicol</strong>. <strong>Moffat</strong>.
<h2 id="acommutatorestimate">A commutator estimate</h2>
Summarizes the ideas of the proof. Stream function representation. Cancellations….end up with a commutator….end up with a weak vs. strong.
<h2 id="dampeddrivennavier-stokesequation">Damped Driven Navier-Stokes Equation</h2>
Standard Navier-Stokes with forcing and an added term $+ \gamma u$, which represents the damping.

You get some a priori bounds which are independent of the viscosity by following the usual arguments.
<h3 id="stationarysolutionsawarmup">Stationary Solutions (a warm up)</h3>
$$ \gamma \omega + u \cdot \nabla \omega - \nu \Delta \omega - g =0.$$
<h3 id="absenceofanomalousdissipation">Absence of anomalous dissipation</h3>
<strong>Theorem:</strong>
$$ \lim_{\nu \rightarrow 0} \nu \int_{R^2} |\nabla \omega^\nu |^2 dx = 0.$$

The key idea is to extract extra structure by taking limits.
<h3 id="statisticalstationarysolutions">Statistical Stationary Solutions</h3>
<strong>Definition:</strong> A stational statisitcal solution (SSS) of the damped, driven NS equation on the phase space of vorticity is a probability meausre $\mu^\nu$ on $L^2 (R^d$ such that )…..some conditions indicating that the equation holds in a weak sense against “cylindrical test functions”.

Ideas of proof….pretty fast….hard to keep up while typing. He emphasizes the role of a nonlinear function $\beta$ which he uses to map from “$L^2$ to $L^\infty$”

One Key idea. Use $J(u \omega) - J(u) J(\omega)$ when you are considering a mollifier $J$. This is a useul trick. “Quadratic flux formula”

The hard part of the proof is to prove the enstrophy balance.

The delicate dance of the $\beta$ parameter reminds me of the role of the smoothing operator $I_N$ in the $I$-method. I’d like to understand this better….

The punch line is that you only need this “old language” for the proof. At the end, we obtain a proof of the absence of anomalous dissipation. I’d like to prove corresponding results for quasigeostrophic.

<strong>Remarks:</strong>
<ul>
	<li>The existence of weak solutions for damped, driven Euler equations: <strong>Barcilon-Constantin-Titi</strong></li>
	<li>For absence of anomalous dissipation: Renormalized weak solutions. Enstrophy balance.</li>
	<li>Results for gSQG. Mentions <strong>Caffarelli-Vasseur</strong>, <strong>Nazorov-Volberg-?</strong> on this equation.</li>
</ul>

<hr />

Questions/Discussion

<hr />

A suggested direction: Stability implies regularity. If you assume that NS solutions are $L^2$ stable then you should be able to prove regularity. <strong>Conjecture:</strong> Fix viscosity. Imagine you have a time horizon and you have a constant. Lipschitz regularity of the flow map implies regularity.
<h1 id="steveprestonhttp:math.colorado.eduprestos:theinextensiblestringasatoymodeloffluids"><a href="http://math.colorado.edu/~prestos/">Steve Preston</a>: <em>The inextensible string as a toy model of fluids</em></h1>
<img src="http://math.colorado.edu/~prestos/steveface.jpg" alt="Steve Preston" />

(pdf slides talk; joint work with Ralph Saxton)

The original idea that the inextensiblestring might have soemthing to do with fluids was due to V. Yudovich. This problem was introduced to the speaker by A. Shnirelman. The part of fluids I want to have a toy model for is the geometric viewpoint.
<h2 id="geometricaspectsoffluidmechanics">Geometric aspects of fluid mechanics</h2>
At a point in a fluid, you have a velocity felid and we minagine this vector pushes a fluid element along that direction. You put an $L^2$-Riemannian metric on the space of maps $C^\infty (M, M)$ and you define geodesics wrt this metric.

Volumorphisms. He views this as a “submanifold” in the space of all maps. A lot of things break down here but formally we think of this curve of volume preserving maps inside the larger flat space of all maps. Hodge decomposition allows us to decompose an arbitrary map into one along the volumorphism submanifold and another involving a divergence.

Misiolek-Himonas

Ebin-Marsden

Riemannian exponential map.

Eulerian viewpoint is easy to formulate, but the Lagrangian form is more convenient for geometry. He emphasized the loss of dierivatives.

“Smoothness of the exponential map is the most basic requirement for doing infinite-dimensional Riemannian geometry rigorously.”

There is a gap between the topology and geometry of volumorphisms.
<ul>
	<li>Topology. We want the volumorphisms to be a smooth submanifold of the space of smooth maps from $M$ to $M$. We can make this rigorous if we enlarge to Sobolev $H^s$ diffeomorphisms with $s &gt; \frac{1}{2} {\mbox{dim}}(M) + 1$ to ensure that $\eta \in C^1$. For smaller $s$, we don’t get a smooth submanifold.</li>
	<li>Geometry. The metric is defined only in terms of $L^2$ distance. So geometrycially, we should consider measureable maps $\eta: M \rightarrow M$ which preserve the measure. These may not even be bijections so that manifold structure fails (not all tangent spaces are isomorphic).</li>
</ul>
If $M$ is three-dimensional, the $L^2$ closure of smooth volumorhpisms is the space of all measure-preserving measureable maps (<strong>Shnirelman</strong>). Fluids should not behave like that! Or maybe they could come close?

In 2d, we don’t understand this so well.
<h2 id="lagrangianaveragedeulerequations">Lagrangian Averaged Euler equations</h2>
We introduce a parameter $\alpha$ and define an alternative Riemannian metric which has an $H^1$ inner product (time $\alpha$) and we consider this only on the Volumorphism “submanifold”. The associated geodesic equation leads to the LAE-$\alpha$. “The idea is to average over small scales of a fluid; as $\alpha \rightarrow 0$ we expect the solutions to approach the usual Euler equation solutions.” When these were introduced, it was expected that 3d global existence would be easier than for Euler but this has not turned out to be the case.

To better understand what is going on, we want simpler one dimensional examples.
<ul>
	<li>Camassa-Holm: $ u_t - u_{txx} + 3 u u_x - 2 u_x u_{xx} - u u_{xxx} = 0$</li>
	<li>Constantin-Lax-Majda: $\omega_t = \omega H \omega, ~ u_x = H \omega$$</li>
</ul>
In the CLM equation $H$ is the Hilbert transform. Modified: $\omega_t - \frac{1}{2} u \omega_x = \omega u_x, ~ u_x = H \omega$.
This is a geodesic equation on the space of diffeomorphisms on $S^1$ with a right-invariant $H^{1/2}$ metric.

….quick transition to the inextensible curves…..moving faster….

Unit speed parametrization. This constraint forces the curve the generate its own tension to satisfy the constraint. This is similar to the pressure which results from the zero divergence condition.
<h3 id="geodesicequationforl2string">Geodesic equation for $L^2$ string</h3>
Orthogonal acceleration $\implies$

$$ \eta_{tt} = \partial_x (\sigma \eta_x)$$

where
$$
\sigma_{xx} - |\eta_{xx}|^2 \sigma = - |\eta_{xt}|^2.
$$
“Here the tension $\sigma$ is analogous to the pressure in the Euler equation, determined nonlocally by a purely spatial differential equation.

WE can think of this as an approximation of the nonlinear wave quation, in the same way as the incompressible Euler equation is an approximation of the compressible Euler equation.”

(This is an interesting nonlocal equation so it should be mentioned on the developing nonlocal equations wiki.)

Finite-d approximate model through a system of rigid rods oscillating like coupled pendula.

In $R^2$, we can write $\eta_x = (\cos \theta, \sin \theta)$ (which enforces the constraint) and rewrite the equations. Some discussion of boundary conditions. The boundary conditions then determine nonlinear constraints on the parameter $\theta$.
<ul>
	<li><strong><a href="http://www.ams.org/mathscinet/search/publdoc.html?arg3=&amp;co4=AND&amp;co5=AND&amp;co6=AND&amp;co7=AND&amp;dr=all&amp;pg4=AUCN&amp;pg5=TI&amp;pg6=PC&amp;pg7=ALLF&amp;pg8=ET&amp;r=1&amp;review_format=html&amp;s4=&amp;s5=motion%20of%20whips%20and%20chains&amp;s6=&amp;s7=&amp;s8=All&amp;vfpref=html&amp;yearRangeFirst=&amp;yearRangeSecond=&amp;yrop=eq">Motion of whips and chains</a>. Preston JDE 2011</strong></li>
	<li><strong>Bootstrap</strong> <strong>Chao Ma, PhD thesis</strong> forthcoming.</li>
</ul>
Movie:
<ul>
	<li>$L^2$ whip. The whip cracks. The curvature becomes singular. <strong>Thess-Zikanov-Nepomnyashchy</strong> The loops make the crack!</li>
</ul>
So, I’d like to revisit the Lagrangian averaging in the setting of the inextensible string. He again adds the $H^1$ inner product to the Riemannain metric on the space of curves. This produces a new geodesic equation, which does not resemble the earlier wave equation. It does still have the nonlocal $\sigma$,…technical slide….

<strong>Preston-Saxton, DCDS-A</strong> (to appear) Some GWP results.

Movie:
<ul>
	<li>Same initial condition and the loops don’t get pinched.</li>
</ul>
<h1 id="emanuelecagliotihttp:sites.google.comsiteecaglioti:longtimebehaviorofsolutionsofvlasov-likeequations"><a href="http://sites.google.com/site/ecaglioti/">Emanuele Caglioti</a>: <em>Long time behavior of solutions of Vlasov-like equations</em></h1>
<img src="http://sites.google.com/site/ecaglioti/_/rsrc/1229459087305/Home/ec.jpg?height=200&amp;width=181" alt="Emanuele Caglioti" />

(pdf slide talk)
<h2 id="outline">Outline</h2>
one slide, overview of the talk.
<h2 id="vlasov-poissonand3deuler">Vlasov-Poisson and 3d Euler</h2>
The Vlasov equation
$$\partial_t f + v \partial_x f + F_f \partial_v f = 0$$

Here $f(x,v): S^1 \times R$ is the phase space density:
$$
\rho (x) = \int dv f(x,v)
$$
is the space density
$$
F_f (x) = \int dy \rho(y) \mathcal{F} (x-y)
$$
is the force.

Vlasov-Poisson Equation (VPE)

$\mathcal{F} = \partial_x \mathcal{V}, ~ \mathcal{V} = \partial_{xx}^{-1} \delta$. For $x \in [0, 2 \pi)$….ack slide change….

2d Euler equation is another example. The vorticity $\omega$ is transported along the flow.

The density $f(x,v,t)$ is transported along the trajectories of an Hamiltonian system:
$$
\dot{x} = v, \dot{v} = F_f (x).
$$

The hamiltonian is a functional of the density $f$ itself: self-consistent force field. Therefore the area of the level sets of $f$ is conserved. Same for 2D Euler the vorticity is tranported along the trajectories of an Hamiltonian system.

Mather: What does that mean “self-consistent force field”? Answer: Some discussion about the mean field limit and statistical mechanics. Here is a <a href="http://en.wikipedia.org/wiki/Hartree%E2%80%93Fock_method">link to related discussion</a>.
<h2 id="possiblebehaviors">Possible behaviors</h2>
<h3 id="stablestationarysolutionsofvpe.">Stable stationary solutions of VPE.</h3>
<strong>Marchioro-Pulvirenti (1986)</strong>

$f = g(v) $ is an example.
<h3 id="bgkwaves">BGK waves</h3>
<strong>Bernstein, Greene, Kruskal (1957)</strong>

$ f = f_0 (x - u_0 t, v - u_0).$

These solutions satisfy some conditions related to the Hamiltonian.

I try to make a parallel with 2D Euler.

Any radial vorticity: $ \omega = g(\rho), ~ \rho = \sqrt{x^2 + y^2}$
is a stationa soution of 2D Euler.

<strong>Kirchoff (1876)</strong> showed that elliptiacl patches are rotating solutions of 2D Euler. The patch is stable if $a &lt; 3b$ (parameters refer to the geometry of the ellipse.)
<h3 id="landaudamping">Landau Damping</h3>
Landau, on the basis of the analysis of the VPE linearized around an equilibrium conjectured that for initial data close to equilibrium
$$
f_0 = f(v) + \epsilon g(x,v)
$$
asymptotically the electric field will vanish and the phase space density will become homogeneous. The linear case has ben fully characterized (Maslov- and Fedoryuk.)

Existence of a class of damped analytic solutions has been proved with a scattering approach by <strong>Caglioti-Maffei (1998)</strong>. <strong>Hwuang-Velasquez (2009)</strong> extended this result to situations close to equilibrium solutions. Initial data cannot be characterized.

<strong>Mouhot-Villani (2009)</strong> proved that close to equilibrium initil data are exponentially damped (Landau Damping). The result is proved in an analytic framework (also Gevray type regularity).

Lin-Zeng (Recently) have shown that BGK exists for small regularity: $W^{s,p}, ~ s&lt; 1 + \frac{1}{p}$. Therefore, there is NO LANDAU DAMPING for small regularity. This is interesting to me….a long time behavior which is dependent upon regularity.

<strong>Matthaeus (1991)</strong> simulation.

….Constantin: this is probably hyperviscosity. ok, but the point he wants to convey is not dependent on this issue.
Shnirelman: this is a very robust picture. When you simulate NS on 2D torus, it always emerges that there are two vortices like this.

Possible limiting behaviors.
<ul>
	<li>Stationary (stable) solution for VPE and for 2D Euler</li>
	<li>time periodic solutions for BGK and Kirkhoff Ellipses for 2D Euler</li>
	<li>Landau damping</li>
	<li>Is it possible to prove damping to BGK solutions?  Many people are working on this.</li>
</ul>
(This theory seems to be quite analogous to the state of the art in nonlinear Schrodinger and wave equations.)
<h2 id="whatcanwesayingeneral">What can we say in general?</h2>
<strong>Shnirelman ICM 2010</strong> Mixing operators in $L^2$. Shnirelman’s construction. Bistochastic operators.

Partial ordering, minimal flows.

It is possible to prove that minimal flows are stationary stable solutions of 2D Eler.

A first conjecture: The set of minimal flows is an attractor for the 2D Euler flow (essentially Landau damping conjecture)

Motivation: If the fluid does not go to stationary solutions level lines of vorticity are stretched and stretched and therefore the solution reaches a minimal element.

The conjecture is probably wrong because more complicated behaviors are expected from simulations.

Brenier: True with probability 1. Caglioti: probably not.

Generalized minimal flows (Shnirelman):

The Navier-Stokes equation with random forcing in the null viscosity limit has an attractor which is concentrated on generalized minimal flows. We reformulate this conjecture in the language of Landau Damping from Vlasov.

A strictly related conjecture.

Given $f_0$, let us define
$$
\Omega (f_0) = [ \mbox{weak limit points of} f(x,v,t): t \rightarrow + \infty ]
$$

Then it is reasonable that generically:
<ul>
	<li>$S(g) \geq S(f_0)$</li>
	<li>If $g_1$ and $g_2$….ack slide changed.</li>
</ul>
<h2 id="constructionofperiodicsolutionsforthehmfmodel">Construction of periodic solutions for the HMF model</h2>
<strong>Morita-Kaneco PRL (2006)</strong>

See also <strong>Antoniazzi-Fanelli-Barre-Chavanis-Dauxois-Ruffo, PRE (2007)</strong>

work in progress with <strong>D. Benedetto</strong> and <strong>P. Butta</strong>.

Conclusions:

We might reasonably expect that asymptitocally the dynamics will become a simple motion. It might even be chaotic but with a few degrees of freedom involved.
<h1 id="robertocamassahttp:www.amath.unc.edufacultycamassa:largeamplitudeinternalwavesandtheirstability"><a href="http://www.amath.unc.edu/Faculty/camassa/">Roberto Camassa</a>: <em>Large amplitude internal waves and their stability</em></h1>
<em><a rel="attachment wp-att-973" href="http://blog.math.toronto.edu/colliand/2012/03/13/ias-workshop-on-symplectic-dynamics-2-monday/3132_wave2_small/"><img class="alignnone size-full wp-image-973" src="http://blog.math.toronto.edu/colliand/files/2012/03/3132_wave2_small.jpg" alt="" width="300" height="181" /></a>
</em>

<a href="http://www.dailytarheel.com/index.php/article/2010/11/uncs_new_wave_tank_will_help_with_experiments_interdisciplinary_studies">Article about Carolina Wave tank</a>

(Collaboration with A. Almgren, S. Chen, R. Tiron, C. Viotti.)

Somewhat soft…..filled with movies…..suitable for the end of the day.

Outline

Motivation: practical (quantitative) vs. “paradigm” (qualitative)  significance of simple models of wave motion in fluids?

Three examples:
<ul>
	<li>Two layer Euler vs. strongly nonlinear models</li>
	<li>Wave induced instabilities</li>
	<li>Integral equations:</li>
</ul>
Introduction. Fluids lab experiments. Cool movie.

Stratified incompressible Euler equations. 2 layer model. As you saw in the movie, diffusion can be ignored on the time scale of the movie.

<strong>Grue et. al JFM 1999</strong> (Norway experimental group)

<strong>Stanton-Ostrovsky 1998</strong> (Oregon Coast), 150m

<strong>ASIAEX 2004</strong> (340m)

<strong>Helfrisch-Melville 2006</strong>

These papers reveal that large amplitude internal waves exist.

<strong>Miyata 1998</strong>, <strong>Choi-Camassa JFM 1999</strong>

Shallow water strongly nonlinear models.

Pictures….pictures….movies.

Richardson Number.

Taylor-Goldstein Eigenvalue problem controls stability.

&nbsp;