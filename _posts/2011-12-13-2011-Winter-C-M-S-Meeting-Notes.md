---
layout: post
author: James Colliander
published: true
tags : [Notes]
comments: false
---


<!-- -->

This past weekend, I attended the <a href="https://camel.math.ca/Events/winter11/">2011 Winter meeting</a> of the Canadian Mathematical Society. I have posted below some (often rough) notes on the talks that I attended.
<h1 id="robertmccannhttp:www.math.toronto.edumccann"><a href="http://www.math.toronto.edu/mccann/">Robert McCann</a></h1>
(joint work with <a href="http://www.math.utk.edu/~denzler/">J. Denzler</a> and <a href="http://www.math.uni-bonn.de/~koch/">H. Koch</a>)

<hr />

ROBERT MCCANN, University of Toronto
Higher-order asymptotics of fast diffusion in Euclidean space: a dynamical systems approach.

With Denzler and Koch, we quantify the speed of convergence and higher-order asymptotics of fast diffusion dynamics on Rn to the Barenblatt (self similar) solution. Degeneracies in the parabolicity of this equation are cured by re-expressing the dynamics on a manifold with a cylindrical end, called the cigar. The nonlinear evolution semigroup becomes differentiable with respect to H"older initial data on the cigar. The linearization of the dynamics is given by the Laplace-Beltrami operator plus a transport term (which can be suppressed by introducing appropriate weights into the function space norm), plus a finite-depth potential well with a universal profile. In the limiting case of the (linear) heat equation, the depth diverges, the number of eigenstates increases without bound, and the continuous spectrum recedes to infinity. We provide a detailed study of the linear and nonlinear problems in H"older spaces on the cigar, including a sharp boundedness estimate for the semigroup, and use this as a tool to obtain sharp convergence results toward the Barenblatt solution, and higher order asymptotics. In finer convergence results (after modding out symmetries of the problem), a subtle interplay between convergence rates and tail behavior is revealed. The difficulties involved in choosing the right functional spaces in which to carry out the analysis can be interpreted as genuine features of the equation rather than mere annoying technicalities.

<hr />

Nonlinear diffusion Equation

$$ \rho_t = \frac{1}{m}\Delta (\rho^m) = \nabla \cdot (\rho^{m-1} \nabla \rho) $$
<ul>
	<li>Heat Equation: ($m=1$) Spreads out at rate $\tau^{1/2}$.</li>
	<li>Porous Medium regime: ($m&gt;1$). Rate of diffusion $\rho^{m-1}$ varies directly with density $\rho$ of diffusing materiel.</li>
	<li>Fast Diffusion regime: ($m&lt;1$). He rewrites $m = m_p = 1 - \frac{2}{n+p}$ with $ p&gt;0$. This leads to tails of algebraic thinckness which decay fast enough to stay in $L^1$. The size of the support grows like $\tau^{\frac{1}{2}[1 + \frac{n}{p}]} = \tau^\beta$.</li>
</ul>
We are interested in the convergence to a characteristic shape called the Barenblatt solution.

McCann-Slepcev 06: An $L^1$ convergence result for general conditions in the case where $p \geq n$. The rate of convergence is $\tau^{-\beta}$ with constant related to the initial first moments.

<strong>Main Goal:</strong> Slide change…ack. It involves an estimate showing that $\frac{\rho}{\rho_B}$ goes where it should.

Friedman-Kamin 80, CarilloToscani 99, Dolbeault-del Pino 00, Otto 01.

Blanchet, Bonforted, Dolbeault, Grillo, Vazquez 07, ….

There are other norms that can be studied besides $L^1$. A nice choice is the so called <em>relative $L^\infty$</em>.

Vazquez 03

Kim-McCann 05

Denzler-Koch-McCann 11  Higher order asymptotics.

Using an infinite dimensional analog of a finte dimensional dynamical systems approach.

A time-dependent rescaling of space. This is explicit because they know the rate of spreading of the solution.

Otto 01. Gradient flow structure and linearization. Rescaled dynamics is the steepest descent of the energy $E(u)$ with respect to an infinite-d heurisitic Riemannian structure whose intrinsic distance is the $L^2$-Wasserstein distance.

<strong>Theorem</strong> pretty long….can’t type it fast enough. Seems quite strong. It captures the convergence up to exponetially small errors and they can improve the exponent by adding more terms to their formula for the asymptotic corrections.

This is different than solitary wave resolution. The conclusion reports that there is one big Barenblatt that describes the asymptotic behavior. The spreading is faster than any translation and eventually it absorbs everything in the wings. In contrast, soliton equations have solutions with long time asymptotic descriptions involving widely separated non-interacting bump functions.
<h1 id="mostaphafazlyhttp:www.math.ubc.cafazly"><a href="http://www.math.ubc.ca/~fazly/">Mostapha Fazly</a></h1>

<hr />

MOSTAPHA FAZLY, UBC
Liouville-type theorems for some elliptic equations and systems

In this talk, we consider the problem of non-existence of solutions for some basic elliptic equations and systems with weights. Starting with Henon-Lane-Emden system, we present a Liouville-type theorem for bounded solutions in dimension N=3 as well as the statement for the full Henon-Lane-Emden conjecture in higher dimensions. Since systems are normally much more complicated than equations, in higher dimensions we back to single equations (both second order and fourth order) to prove such theorems under some additional assumptions on solutions. This work has been done under supervision of N. Ghoussoub.

<hr />

<a href="http://arxiv.org/abs/1107.5611">arXiv1</a>

<a href="http://arxiv.org/abs/1109.5138">arXiv2</a>

Liouville’s Theorem: Any bounded entire function is a constant.

For PDEs, any bounded harmonic funciton is a constant.

Lane-Emden equation. $-\Delta u = u^p$ on $R^N$.

Gidas-Spruck 1981:
Assume $N \geq 3$. Let $u$ be a nonnegative solution of L-E with $ 1 &lt; p &lt; \frac{N+2}{N-2}$. Then $u=0$.

For the critical exponent, there is an explicit solution.

C.S. Lin 1998, similar result for a 4th order generalization. In the critical case, there is an explicit solution.

<strong>Lane-Emden system:</strong> On $R^N$, consider
$$ -\Delta u = v^p, -\Delta v = u^q$$

<strong>Lane-Emden conjecture:</strong> Suppose $(p,q)$ lies under the critical hyperbola
$$ \frac{N}{p+1} + \frac{N}{q+1} &gt; N-2 .$$
Then there is no positive solution for the above system.

Mitidieri 1996, Serrin-Zou 1996, Serrin-Zou, Polacik-Quittner-Souplet 2007, Souplet 2009.

Known to be sharp for radial solutions. $N=3$ True for polymomially bounded solutions. Condition removed. $N=4$ done. $N \geq 5$ is open.

<strong>Henon Equation:</strong> On $R^N$, we consider

$$-\Delta u = |x|^a u^p$$

<strong>Conjecture:</strong> Assume $ N \geq 3$. Let $u$ be a nonnegative solution of the above euqtion with $1 &lt; p &lt; \frac{N+2 + 2a}{N-2}$. Then $u=0$.

Some partial results listed….

<strong>Fourth order Henon equation.</strong>

Also open for $N \geq 5$. There is a stability condition in this context. Methods are linked to ideas used to prove the De Girogi conjecture.

<strong>Henon-Lane-Emden System and conjecture</strong>

….some details.
<h1 id="marypughhttp:www.math.toronto.edumpugh"><a href="http://www.math.toronto.edu/mpugh/">Mary Pugh</a></h1>

<hr />

MARY PUGH, University of Toronto
A new result in blow-up for long-wave unstable thin film equations

This talk will provide an introduction to long-wave unstable thin film equations of the form
$$u_t = −(u^n u_xxx)<em>x−B(u^m u</em>x)_x
$$
The exponents n and m determine whether or not finite-time blow-up of the solution might occur. In this talk, we present new results for the critical $(m=n+2)$ and supercritical cases $(m&gt;n+2)$ on the line. This is joint work with Marina Chugunova (University of Toronto) and Roman Taranets (University of Nottingham).

<hr />

(joint work with Chunganova and Taranets)

<a href="http://arxiv.org/abs/1008.0385">arXiv</a>

$$
u_t = - (u^n u_{xxx})<em>x -  B(u^m u</em>x)_x
$$

This is a long wave unstable thin film equation.

Consider data $u_0 (x) = \overline{u} + \epsilon u_1 (x,0) + \epsilon \cos (\xi x + \phi)$.

The small perturbation $u_1$ will approximately satisfy a related equation and the cosine perturbation generates a low frequency instability.

Critical regimes:

Compare height scales and length scales. Cannot have finite-mass blowup if $m &lt; n+2$.

Another path is to plug in a self-similar ansatz and look. Eventually, you find this relationship.

Bertozzi-Pugh (CPAM) 1998:
<ul>
	<li>$m&lt; n+2$ subcritical</li>
	<li>$m = n+2$ critical</li>
	<li>$m&gt; n+2$ supercritical.</li>
</ul>
Dissipated energy. Can it somehow be related to a useful norm like $H^1$? Could it ever go to $-\infty$?.

(Analogous somehow to the Weinstein threshold.)

Noviick-Cohen+Shishkov 2010.

Critical regime involves an $L^4$  potential energy. The main difference is that the $L^1$ norm here plays the role of the $L^2$ norm in the NLS setting. Therefore, 4 turns out to be the critical potential energy power whereas in NLS criticality occurs when potential energy is $u^6$. There is an optimal mass threshold. For mass less than this value, there is a spreading of the dsolution. At equality, there is a blowup.

Witelski+Bernoff_Bertozzi did a simulation with two disjoint subcritical mass droplets whose joint mass is supercritical. Computationally, they see a focusing one point blowup effect.

In the critical and supercritical regimes (Bertozzi+Pugh 2000, building on a formal argument by Bernoff only for $n=1$). There is a variance equality, analogous to the Glassey identity, which eventually proves the existence of finite time blowup solutions.

“This is not a hugely strong statement.” It does not prove what happens but does show that blowup occurs.

In the case $ n \in (0,2)$, Chugunova+Pugh+Taranets managed to find an obstructive argument implying blowup.

<hr />

OK, so it seems they have found a flexible virial-type structure governing the blowup phenomena for this problem. In principle, there should be next steps towards a definitive understanding of the blowup. For example, one should be able to prove an $L^1$ concentration result with lower bound of on concentrated mass in terms of the optimal constant in their interpolation inequality. It seems that all the pieces are in place to prove the analog of the Merle-Tsutsumi concentration result. I find the exponential weights intriguing. What is the meaning of these in this setting?
<h1 id="alexeif.cheviakovhttp:math.usask.cacheviakov"><a href="http://math.usask.ca/~cheviakov/">Alexei F. Cheviakov</a></h1>
<img src="http://math.usask.ca/~cheviakov/pic/a_chev_photo2.jpg" alt="Alexei Cheviakov" />

<hr />

ALEXEI F. CHEVIAKOV, University of Saskatchewan
Conservation Laws of Surfactant Transport Equations

We present interfacial convection and convection-diffusion equations which model the transport of surfactants in an incompressible two-phase flow. The model employs the level set formulation of the interface. In both convection and convection-diffusion settings, in three dimensions, we derive infinite families of conservation laws for these equations. Using these conservation laws, surfactant transport equations can be written in a fully conserved form. This is a joint work with C. Kallendorf, M. Oberlack, and Y. Wang (TU Darmstadt).

<hr />

<h3 id="whatisasurfactant">What is a surfactant?</h3>
Surfactant is a furface active agent. They are molecules with a hydrophobic tail and a hydrophili head. Examples include shampoos and fatty oils. These molecules have various interesting properties. They have many interesting industrial and medical applications. Bilayer sheets arise in soap films. Micelle. Liposome. Soap bubbles.

Wang-Oberlack 2011

Governing equations. Euler, Navier-Stokes, incompressibility condition and surfactant transport equation involivng the surface laplacian.

To do numerical modeling, we require that our equations are discretized into a fully conserved form. Can the surfactant transport equation be written in conservation law form.
<h3 id="conservationlaws">Conservation laws</h3>
Divergence expression equal to zero.

Simple PDE example. 1d wave equation. Conservation of momentum and conservation of energy. Both can be derived from a multiplier calculation.

Noether’s thoerem. Direct construction method is sometimes more flexible. Introduces the notion of an <em>Euler operator</em> with respect to $U^j$. (This discussion seems to involve the same notions as the geometric description of Noether’s equation involving killing and conformal killing fileds.)

Completeness.

For the majority of physical DE systems all conservation laws follow from linear combos of equations derived in this way.

This provides a path to build conservation laws that is different from Noether’s theorem, placing the equation as the primary object instead of the Lagrangian. This is all reminiscent of the Friedrichs ABC method as described by Morawetz. What about monotone formulae? Does thhis general theory lead us to any new monotone quantities?

Differential Grobner basis….other methods allow us to reduce the number of equations encountered here.

Applications.

Using this direct method machinery, he derives some conservation laws. The method emplys mulipliers and Euler operators. The method is implemented in a symbolic package GeM for Maple. There emerges an infinite faily of $c$-dependent conservation laws for cases with and without diffusion. Surfactant dynamics can be written ina fully conserved form.

Open problems.

Higher order conservation laws? Can we get more by including fluid dynamics equations?

References.

Anco-Bluman 1997

Anco-Bluman 2002

Bluman-Cheviakov-Anco 2010

Kallendorf-Cheviakov-Oberlack-Wang 2011
<h1 id="gideonsimpsonhttp:www.math.toronto.edusimpson"><a href="http://www.math.toronto.edu/simpson/">Gideon Simpson</a></h1>

<hr />

GIDEON SIMPSON, University of Minnesota
On the Well and Ill-Posedness of Degenerately Dispersive Equations

In some physical problems, such as granular media, sedimentation, and magma dynamics, the leading order continuum model is a degenerately dispersive equation. A rigorous analysis of equations of this type has only recently begun and remains incomplete. Though some cases are locally, and globally, well-posed, others may be ill-posed.
In this talk, we consider the Rosenau-Hyman compacton equations. Inspired by a proof of ill-posedness for a surrogate equation, we present robust numerical evidence that the $K(2,2)$ compacton equation is ill-posed for data about the zero background state. The mechanism of ill-posedness is an observed loss of continuity of the solution operator; arbitrarily small data may become arbitrarily large at a fixed time $T&gt;0$. We also explore the equation about a nonzero background state, and examine the limit as this reference value goes to zero.

This work is in collaboration with D.M. Ambrose, J.D. Wright and D.G. Yang (Drexel University).

<hr />

(joint work with D. Ambrose, J.D. Wright, D.G. Yang)
<h3 id="degeneratedispersion">Degenerate Dispersion</h3>
The magma equations. When $\phi$ vanishes, the dispersion turns off.

The Rosenau-Hyman compacton equations. Again, we have a nonlinear prefactor appearing inside the third order derivative term.

In both cases, we can observe the nonlinear term influencing the dispersion relation.

Danger of Heuristics.

Camassa-Holm, 1993. CH has a term $u u_{xxx}$ which looks scary. But, this is a completely integrable system so we should not be scared about the degenerate nonlinear dispersive equations.

Origins of the Magma equations.

Origins of the $K(2,2)$ compacton equation. Solitons have exponential tails. In nature, we don’t have exponential tails. We need to have localized pulses.

Granular chains have similar properties.
<h3 id="rigorousprogressonwell-posedness">Rigorous progress on well-posedness</h3>
Analytical alternatives in studying degenerate dispersion.

Self regularizing well-posedness.

Assume the initical conditions are nondegenerate; the data is strictly positive. Prove that the flow preserves nondegeneracy for some time; the solution remains striclty positive.

Accept degeneracy.

Develop a motion law for the boundary of the support….ack slide change.

For the magma equation, assume that we have data which looks like 1 + $H^1$. Then the solution exists uniquely on a positive time interval and remains bounded away from zero.

Ambrose-Wright 2010: $C^3$ solutions of the Compacton equations preserve their support.
<h3 id="compuatationalresultsonwp">compuatational results on wp</h3>
To justify the simulation, the equation should be well-posed. We don’t know that yet. So, we regularize by adding on a 4th order regularizing term. Inverting that smoothing operator helps tame the nonlinearity. He calls the regularized equation $K_\delta (2,2)$ and studies this in the limit as $\delta \rightarrow 0$.

He forecasts a wp result for positive data for $K(2,2)$.
<h3 id="rigorousresultsonill-posedness">Rigorous results on ill-posedness</h3>
Hints of ill-posedness. Backwards diffusion effect?

Surrogate equation. $u_t = 2 u u_{xxx}$. Differentiating this wrt x leads to a backwards diffusion term. The backwards diffusion effect inside the surrogate equation might give us a hint toward proving ill-posedness.

Describes a sequence of steps leading to the conclusion that the surrogate equation has a norm inflation effect driven by the backwards diffusion effect. These steps suggest that one might expect an ill-posedness result.
<h3 id="compuationalresultsonill-posedness">compuational results on ill-posedness</h3>
Interesting simulations involving the collision of two compactons for small diffusive regularization parameter $\delta$. It appears to be very sensitively dependent upon $\delta$ and creates a wildly oscillatory effect when $\delta$ is small.
<h1 id="fridolintinghttp:math.lakeheadu.cafridolin-ting"><a href="http://math.lakeheadu.ca/fridolin-ting/">Fridolin Ting</a></h1>

<hr />

FRIDOLIN TING, Lakehead University
Nonradial solutions to magnetic Ginzburg-Landau equations on the whole plane

We show that there exists non-radial, degree-changing, finite-energy solutions to the magnetic Ginzburg-Landau equations on the whole plane. These solutions are polygonal type configurations with $2\pi k$ symmetry for $k\geq 7$. This is joint work with J. Wei.

<hr />

Magnetic vortices.

Plohr 78, Berger-Chen 89.

Stability, Gustafson-Sigal 2000.

Effective dynamics, Gustafson-Sigal 2006.

Bethuel,  Brezis, Helein 1993.

Sandier-Serfaty 2007

Gustafson-Sital-Tzaneteas 2010

Ovchinnikov-Sigal 2004.

Main theorem. Construction of a bunch of new vortex configurations! The construction is almost in equilibrium.

Kapouleas 1991. Idea came from here. Finding compact constant mean scurvature surfaces.

Musso-Pacard-Wei 2010. Finite energy sign changing solutions of the NLS with dihedral symmetry.
<h1 id="ehsankamalinejadhttp:www.math.toronto.educmskamalinejad-ehsan"><a href="http://www.math.toronto.edu/cms/kamalinejad-ehsan/">Ehsan Kamalinejad</a></h1>

<hr />

EHSAN KAMALINEJAD, University of Toronto
Gradient flow methods for thin-film and related higher order equations

We will discuss recent results on a class of higher-order evolution equations that can be viewed as gradient flows on the space of probability measures with respect to the Wasserstein metric. The simplest of these equations is the thin-film equation ∂tu=∂x(u∂3xu), which corresponds to the Dirichlet energy. We will consider questions of existence and uniqueness of these gradient flows. A key probem in the analysis is the lack of convexity of the relevant energy functionals.

<hr />

(Joint work with Almut Burchard).

Existence and uniqueness of fourth and higher order nonlinear evolution equation

Powerpoint slides actually slide in this talk. General overview of gradient flow on the space of probability measures wrt the Wasserstein metric.

Ask for energy to be convex along geodesics. This is the notion of displacement convexity.
<h1 id="kumarmurtyhttp:www.math.toronto.edumurty"><a href="http://www.math.toronto.edu/murty/">Kumar Murty</a></h1>

<hr />

KUMAR MURTY, University of Toronto
The Tau of Ramanujan

The mathematical work of Srinivasa Ramanujan is striking for its originality and insight. But these very qualities also make it hard to understand. In this talk, we shall look at one aspect of Ramanujan’s legacy and use it as a backdrop to more generally discuss creativity and discovery in mathematics.

<hr />

This was an interesting public lecture held at Ryerson University. The talk addressed the ideas of creativity and genius in mathematics.
<h1 id="dmitrypelinovskyhttp:dmpeli.math.mcmaster.ca"><a href="http://dmpeli.math.mcmaster.ca/">Dmitry Pelinovsky</a></h1>
<img src="http://dmpeli.math.mcmaster.ca/ImageBank/photoDP2.jpg" alt="Dmitry" />

DMITRY PELINOVSKY, McMaster University
Rigorous justification of the short-pulse equation

We prove that the short-pulse equation, which is derived from Maxwell equations with formal asymptotic methods, can be rigorously justified. The justification procedure applies to small-norm solutions of the short-pulse equation. Although the small-norm solutions exist for infinite times and include modulated pulses and their elastic interactions, the error bound for arbitrary initial data can only be controlled over finite time intervals. This is the joint work with Guido Schneider, University of Stuttgart.

(joint work with Guido Schneider)

$$
u_{xt} = u + \frac{1}{6} (u^3)_{xx}
$$

Schafer-Wayne 2004

Stefanov et. al. 2010

Pelinovsky-Sakovich 2010

Liu-Pelinovsky-Sakovich 2010

Liu-Pelinovsky-Sakovich 2010

This model is integrable. The short pulse equation is closely related, via coordinate trnasformations, to the sine-Gordon equation. This relationship was observed by Sakovich-Sakovich 2005, 2006. The transformation is not globally well-defined. Not all solutions can be generated in this way. For example, short pulse equation does not have a solution in anlogy with the loop soliton solution of sine-Gordon. sine-Gordon breathers spawn 2-soliton solutions of short pulse.

Alterman-Rauch 2003

Barrailh-Lannes 2002; Colin-Galice-Laurioux 2005

Colin-Lannes 2009; Lannes 2011.

For the short pulse equation, only linearized equations were justifed from Maxwell equations using oscillatory integrals and Fourier analysis. Chung-Jones-Schafer-Wayne 2005.

Toy problem—quasilinear Klein-Gordon equation:

$$u_{tt} - u_{xx} + u + (u^3)_{xx} = 0.$$

Justification theorem. A good ($H^s$, $s&gt;7/2$) solution of the short pulse equation valid on a time interval of size 1 with small data is close to a solution of the quasilinear K-G equation on the same time interval. (theorem statement is actually more involved but this appears to capture the jist of it.)

Brunelli 2005

Using integrable structure, small $H^2$ data for short pulse equation evolves globally in time.

Blowup alternative.

<hr />

I am a bit confused. Here we have a completely integrable pde which forms singularities in finite time? After the talk, Dmitry pointed out that the integrable structure involved here is revealed via changes of variable to convert the short pulse equation into the sine-Gordon equation. The changes of variable become singular at blowup.
<h1 id="antonsakovichhttp:www.math.mcmaster.casakoviasindex.html"><a href="http://www.math.mcmaster.ca/~sakovias/index.html">Anton Sakovich</a></h1>
<img src="http://www.math.mcmaster.ca/~sakovias/anton.jpg" alt="Anton" />

ANTON SAKOVICH, McMaster University
Wave breaking in the short-pulse equation

In this talk, we discuss sufficient conditions for wave breaking in the short-pulse equation describing wave packets of few cycles on the ultra-short pulse scale. Our analysis relies on the method of characteristics and conserved quantities of the short-pulse equation and holds both on an infinite line and in a periodic domain. We provide numerical illustrations of the finite-time wave breaking in a periodic domain.
This is a joint work with Yue Liu and Dmitry Pelinovsky.
<h1 id="magdalenaczubakhttp:www.math.binghamton.educzubakresearchindex.html"><a href="http://www.math.binghamton.edu/czubak/research/index.html">Magdalena Czubak</a></h1>
MAGDALENA CZUBAK, SUNY Binghamton
On some properties of the Navier-Stokes equation on the hyperbolic space.

Contrary to what is known in the Euclidean case, finite energy and finite dissipation solutions to the Navier-Stokes equation on a two dimensional hyperbolic space are nonunique. We review the nonuniqueness result and discuss possible ways to arrive at uniqueness of solutions in the hyperbolic setting. This is based on joint works with Chi Hin Chan and Pawel Konieczny.

(joint work withChi Hin Chan, Pawel Konieczny)

<a href="http://front.math.ucdavis.edu/1006.2819">arXiv</a>
<h3 id="l-hsolutions">L-H solutions</h3>
NS on $R^n$. Vector valued unknown. $P$ is the pressure. $u$ is divergence free.

<strong>Theorem:</strong> Leray-Hopf solutions on $R^n$. Energy inequality.

Goal: investigate how geometry (of the underlying space) affects the uniqueness of the L-H solutions of NS equation.
<h3 id="nsonmanifolds">NS on manifolds</h3>
What is the equation on a Riemannian manifold? What happens with the Laplacian?

Ebin-Marsden 1970. Laplace beltrami works well on functions be we have a vector valued unknown. Hodge laplacian? E-M say no…the right thing to use is the <em>deformation tensor</em>. We get the hodge laplacian witha correction. Basically, you soulnd also introduce a term associated with the Ricci curvature. In this setting, it is more natural to work with one-forms than with vector fields. This can be done easily by raising and lowering indices using the metric.

On the hyperbolic space, we can identify the Ricci term very nicely. It produces $Ric (U^<em>) = - a^2 (n-1) U^</em>.$ On a general manifold, the Ricci formula is not as nice.

$NS_M$ is then expressed as an equation on one forms with an additional terma ssocatiated with the Ricci curvature. T

Ebin-Marsden 1970

Priebe 1994

Mazzucato 2003

Dindos-Mitrea 2004

Q.S. Zhaing 2006: also gets nonuniqueness using a connected sum of two copies of $R^3$.

(without the Ricci term)

Avez-Bamberger 1978

Filatov-Il’in 1989

Ilin 1991

Temam-Wang 1993
<h3 id="nonuniquenessofthel-hsolutions">Nonuniqueness of the L-H solutions</h3>
<strong>Theorem (Chan-Czubak 2010):</strong>

There exists infinitely many smooth solutions of Navier-Stokes on the hyperbolic 2d space which satisfy finite energy, bounded $L^2$, …

On a general negatively curved manifold, the modified NS equation (drop the Ricci term), with a certain nonpinching condition on the manifold, there is nonuniqueness.

Anderson 1983, Sullivan 1983. Anderson-Schoen 1985.

There is an abundance of nontrivial harmonic functions on negatively curved manifolds. (Actual statement is more precise.)

The idea of using harmonic functions to build nontrivial solutions of NS goes back to Serrin but, because of the Liouville theorem, these solutions are not interesting in the $R^n$ case.

Solution Pairs.

Using the nontrivial harmonic functions, we can build solution pairs $(U^*, P)$.

<a href="http://en.wikipedia.org/wiki/W._V._D._Hodge">Hodge</a> was a Scottish mathematician who defined the structures required to define the Laplacian on one forms.

S.-T. Yau 1975

description of gap preventing extension to 3d hyperbolic space.

Martin Boundary
<h3 id="lackofliousvilletheoremsinahyperbolicsetting">Lack of Liousville theorems in a hyperbolic setting</h3>
Koch-Nadirashvili-Seregin-Sverak 2009.

Let $u$ be a bounded weak solution of NS on $R^2$….ack slide changed…..liouville theorem.
<h3 id="uniqueness">Uniqueness?</h3>
Work in progress.

Heywood 1976 shows that there is an interesting separation of natural versions of $H^1$ zero divergence vector fields on manifolds.
<h1 id="xiaoliuhttp:www.math.toronto.educmsliu-xiao"><a href="http://www.math.toronto.edu/cms/liu-xiao/">Xiao Liu</a></h1>
XIAO LIU, University of Toronto
Numerical simulation for Derivative Nonlinear Schrodinger Equation

We present the numerical simulation of generalized Derivative Nonlinear Schrodinger Equation (gDNLS):
$$i\phi_t + \phi  <em>{xx}+ i|\phi|^{2\sigma} \phi</em>x=0.$$
In the case of σ=1, it describes the long wavelength dynamics of dispersive Alfven waves propagation. We observe that for σ&gt;1, solutions may develop a singularity after a finite time, and we give a precise form of the blow up rate and the solution profile.

Blowup for derivative NLS. Very nice talk with simulations probing the generalized DNLS. Current studies investigating what happens as the parameter $\sigma \searrow 1$.

<hr />

Followup discussion considered the idea to prove LWP for the quintic DNLS. Fractional powers would involve another layer of difficulty, but the quintic case might be accessible using $X^{s,b}$-type spaces and multilinear tools.
<h1 id="waltercraighttp:www.math.mcmaster.cacraig"><a href="http://www.math.mcmaster.ca/craig/">Walter Craig</a></h1>
<img src="http://www.math.mcmaster.ca/craig/Walter_01-03-02.jpg" alt="Walter" />

WALTER CRAIG, McMaster University
On the size of the Navier - Stokes singular set

Consider the hypothetical situation in which a weak solution $u(t,x)$ of the Navier-Stokes equations in three dimensions develops a singularity at some singular time $t = T$. It could do this by a failure of regularity, or more seriously, it could also fail to be continuous in the strong $L^2$ topology. The famous Caffarelli Kohn Nirenberg theorem on partial regularity gives an upper bound on the Hausdorff dimension of the singular set $S(T)$. We study microlocal properties of the Fourier transform of the solution in the cotangent bundle $T^* (\mathbb{R}^3)$ above this set. Our first result is that, if the singular set is nonempty, then there is a lower bound on the size of the wave front set $WF(u(T,.))$, namely, singularities can only occur on subsets of $T*(\mathbb{R}^3)$ which are sufficiently large. Furthermore, if the solution is discontinuous in $L^2$ we identify a closed subset $S^{L^2}(T)$ of $S(T)$ on which the $L^2$ norm concentrates at this time $T$. We then give a lower bound on the microlocal manifestation of this $L^2$ concentration set, which is larger than the general one above. An element of the proof of these two bounds is a global estimate on weak solutions of the Navier-Stokes equations which have sufficiently smooth initial data.

(joint work with Maxim Arnold [UIUC] and Andrei Biryuk [U. Krasnodar])

<a href="http://ams.org/mathscinet/search/publdoc.html?arg3=&amp;co4=AND&amp;co5=AND&amp;co6=AND&amp;co7=AND&amp;dr=all&amp;pg4=AUCN&amp;pg5=TI&amp;pg6=PC&amp;pg7=ALLF&amp;pg8=ET&amp;review_format=html&amp;s4=Craig%2C%20Walter&amp;s5=&amp;s6=&amp;s7=&amp;s8=All&amp;vfpref=html&amp;yearRangeFirst=&amp;yearRangeSecond=&amp;yrop=eq&amp;r=2&amp;mx-pid=2644785">Link to MathSciNet entry about first paper along these lines.</a>
<h2 id="ivpforns">IVP for NS</h2>
NS initial value problem. This may be viewed as Newton’s laws for a fluid. Initial finite energy ($L^2$) data: how does it evolve? We can consider the spatial domain to be $R^3$ or $T^3$. (Real physical problems have boundaries.) The problem on $R^3$ with smooth boundary remains open.

Do solutions exist? Yes, in some sense.

If no singularities form, then yes. Solutions exists, they are unique and the theory is satisfactory.

If singularities form, then weak solutions exist but they aren’t known to be unique…

Leray weak solutions.
<ol>
	<li>$(u,p)$ solves the problem in the sense of distributions AND</li>
	<li>Integrability conditions and Sohr-vonWahl 1986 pressure condition.</li>
</ol>
Leray 1934.

I am studying every solution that satisfies these properties.

$L^s_t L^p_x$
<h3 id="singularsets">Singular sets</h3>
The singular set $S(u)$ is the set of space-time points at which $u(t,x)$ is not locally bounded. That is $(t_0, x_0) \notin S(u)$ if there is a neighborhood such that $u(t,x)$ is bounded on $Q$.

Serrin theory says this is good enough to define the singular set. We can upgrade to Holder contiuity.

These results have been improved along a sequence of steps culuminating in Escauriaza-Seregin-Sverak 2003.

Upper bounds on the singular set.

Singular times.

Leray said that singular times have zero 1/2 dimensional Hausdorff measure.

Caffarelli-Kohn-Nirenberg 1982.

The one dimensional parabolic Hausdorff measure of $S(u)$ is zero.

Restrict to a time slice.

CKN says that the 1d Hausdorff measure is zero.

How to define the Hausdorff dimension? Cover the singular set by balls and sum up over the radii to the power beta and then optimize over the cover.

<strong>Theorem 1.</strong>

If $T$ is a singular time for $u$ then $”dim” (WF(u)) \geq \frac{1}{2}$.

In each fiber it is at least half dimensional.
<h3 id="threeestimatesonlerayweaksolutions">Three estimates on Leray weak solutions</h3>
<ol>
	<li>Energy inequality (an axiom)</li>
	<li>Fois-Guilope-Temam 1981, Chemin 2004.
$$
\int \| u(\cdot, t) \|_{\infty} dt &lt; + \infty, ~ \forall ~T \in R^+.
$$</li>
	<li>Biryuk-Craig 2009. A (future) invariant set for NS flow….</li>
</ol>
Energy concentration set $S^{L^2}$. Suppose $T$ is a singular time when the $L^2$ norm drops down.

<strong>Theorem 2 (Arnold-Craig 2010):</strong> If $T$ is a singular time and is a time of energy discontinuity then the dimension of the WF is $\geq 1$.

Identify a geometry subset of $T^* (R^3)$.

Probe the solution with the Weyl calculus of pseduodifferential operators.

Identify the $L^2$ discontinuities with defect measures and $WF^{L^2} (u)$ with their support.

Define the “dimension” of the sets.

Argue by contradiction.
<h3 id="phasespacevolume:lowerboundsonthesizeofwavefrontsets">Phase space volume: lower bounds on the size of wave front sets</h3>
<h3 id="ideasofproof:microlocalanalysisanddefectmeasures">Ideas of proof: microlocal analysis and defect measures</h3>
&nbsp;