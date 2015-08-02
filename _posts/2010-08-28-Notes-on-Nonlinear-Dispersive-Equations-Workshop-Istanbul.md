---
layout: post
category : lessons
tags : [notes, Istanbul]
comments: false
---


During last week's 
<a href="http://imbm.org.tr/NDE2010.htm">NDE meeting in Istanbul</a>, I experimented and took real-time notes in 
<a href="http://fletcherpenney.net/multimarkdown/">MultiMarkDown</a> during the talks. 
If any of the speakers wish, I can post links to their presentations provided they send me a copy of their slides.  --J. Colliander


<h1><a href="http://www.math.toronto.edu/colliand/">James Colliander</a> (<a href="http://www.math.toronto.edu">Toronto</a>)</h1>
<h3>Almost sure well-posedness of the cubic nonlinear Schrödinger equation  below $L^2({\mathbb{T}})$</h3>
I spoke about <a href="http://arxiv.org/abs/0904.2820">recent work</a> with <a href="http://www.math.toronto.edu/oh">Hiro Oh</a> . Here is a<a title="link" href="http://blog.math.toronto.edu/colliand/files/2010/08/2010_08_Colliander_Istanbul_Final.pdf"> link to my slides</a>.

Some conversations after my talk about Bourgain's high/low frequency truncation method and refined bilinear estimate are amplified in the <a href="http://blog.math.toronto.edu/colliand/files/2010/08/2009_06_15_Warwick_Colliander_Final.pdf">slides of my Warwick talk</a>.

<hr />

<h1 id="alberterkiphttp:people.sabanciuniv.edu.tralberterkipsabanciuniversityhttp:www.sabanciuniv.edutranasayfaanasayfa.phpsabanciu."><a title="Erkip" href="http://people.sabanciuniv.edu.tr/albert/">Albert Erkip</a> (<a title="Sabanci U." href="http://www.sabanciuniv.edu/tr/anasayfa/anasayfa.php">Sabanci University</a>)</h1>
<strong>A review of some results on a class of nonlocal nonlinear wave-type Cauchy problems</strong>

A lot of the work here is inspired by the thesis of Nilay Duruk.
<h2 id="overview">Overview</h2>
<ul>
	<li>Nonlocal Elasticity</li>
	<li>Examples</li>
	<li>Cauchy Problem</li>
	<li>Ongoing Studies</li>
</ul>
<h2 id="nonlocalnonlinearequation">Nonlocal nonlinear equation</h2>
$$u_{tt}=[\beta*(u+g(u))]_x$$

$$0≤{\hat{\beta}}(\xi)≤C(1+\xi^2)^{-r/2}$$
<h2 id="examples">Examples</h2>
Take $\beta=\delta,$ the Dirac measure. The equation becomes a more standard nonlinear equation.

Different choices of $\beta$ lead to different equations.
<h2 id="cauchyproblem">Cauchy Problem</h2>
The results identify conditions, usually involving smoothing assumptions on $\beta$, under which they obtain local well-posedenss results.

Global results are also obtained provided there is appropriate control in $L^\infty$.

How to get the $L^\infty$ control? If the integral of the nonlinearity is bounded from below by $-k u^2$ then we have a global solution.
<h2 id="ongoingstudies">Ongoing Studies</h2>
Obvious generalizations….2d case and efforts to generalize to equations which are <em>meaningful</em> in elasticity. We have also considered the <em>peridynamic</em> problem. This is a nonlocal generalization of the classical problems in elasticity which allows for tears and cracks.

Scattering? Small amplitude initial data? Travelling Waves?
<h2 id="postlude">Postlude</h2>
OK, so I discussed this further with H. Erbay. There are some issues with the linear problem. Let

$\Delta_\beta$ be the Fourier multiplier operator given by $-ξ^2 \beta(\xi )$. This collapses to the Laplacian when $\beta=1$. For the usual wave operator we have inhomogeneous smoothing of order 1 by the usual denominator games. However, for the wave operator corresponding to $\Delta_\beta$ we have smoothing by division by $\xi \beta(\xi)$. If $\beta(\xi)$ decays like $\xi^{-r}$ with $r&gt;2$ we lose the smoothing property and have new troubles.

In the discussion after the talk, E. Titi asked what they would do on a bounded domain. In this case, the convolution operator used to express the dynamics on the spatial side does not make sense near the boundary. Upon thinking about this a bit, it seems to me that a natural thing to do is to express the data in the basis of eigenfunctions of the Laplacian on the domain and then recast the dynamics as a multiplier operator in that basis. The issues of the domain are addressed then by the eigenfunctions and the nonlocal aspects near the boundary are resolved.

<hr />

<h1 id="sadeterbayhttp:math.isikun.edu.trserbaysadeterbyisikuniversity"><a title="Sadet Erby" href="http://math.isikun.edu.tr/serbay/">Sadet Erbay</a> (Isik University)</h1>
<strong>The Cauchy problem for a class of two-dimensional nonlocal nonlinear wave equations governing anti-plane shear motions in elastic materials</strong>

(joint work with H. Erbay and A. Erkip)
<ul>
	<li>Two dimensional nonlocal equations</li>
	<li>LWP</li>
	<li>Conservation of Energy and Global Existence</li>
	<li>Blowup</li>
</ul>
<h2 id="elasticitymotivatesstudyofnonlocalwaveequations">Elasticity Motivates Study of Nonlocal Wave Equations</h2>
Deformation fields in an elastic body might be influenced by distant points. Therefore, we encounter nonlocal elasticity.

$$ w_{tt}=(\beta *F_{w_x})_x + (\beta * F_{w_y})_y)$$

$$0 \leq \hat{\beta}(\xi) \leq (1 + |\xi|^2)^{-r/2}$$

Taylor expansion in $\beta$ leads to higher order powers in $\xi$, which produces higher order derivative correction terms.
<h2 id="cauchyproblem">Cauchy Problem</h2>
Convert IVP into a Banach space valued ODE. Sobolev embedding. Algebra property of $H^s \cap L^\infty$. Convenient assumptions allow them to control the nonlinearity. (All this is done pointwise in time and the regularity is quite high.)

(My impression is that ideas from <span class="externalcitation"> (<a id="Kenig:1991p67" href="http://www.iumj.indiana.edu/IUMJ/FULLTEXT/1991/40/40003">Kenig-Ponce-Vega, Indiana Math Journal, </a></span><a id="Kenig:1991p67" href="http://www.iumj.indiana.edu/IUMJ/FULLTEXT/1991/40/40003">1991 vol. 40 (1) pp. 33-69</a><span class="externalcitation">)</span> could be used to prove Strichartz-type estimates adapted to this family of problems, under more precise assumptions on the decay of $\hat{\beta}$.

Blowup Alternative expressed in terms of $\| Dw \|_{L^\infty}$.
<h2 id="conservationofenergyandglobalexistence">Conservation of Energy and Global Existence</h2>
The energy involves a Fourier multiplier replacing the usual appearance of $\nabla$ in the kinetic energy. Under certain lower bound conditions on the potential energy, they can prove that a certain norm is bounded for all time which in turn controls the blowup alternative norm $\|Dw\|_{\infty}$.

.

<hr />

<h1 id="nilayduruksabanciuniversity">Nilay Duruk (Sabanci University)</h1>
<strong>Blow-up and global existence for a general class of nonlocal nonlinear coupled wave equations</strong>

(joint work with H. Erbay and A. Erkip, this is part of her thesis)
<ul>
	<li>Nonlocal Cauchy problem</li>
	<li>Local</li>
	<li>Global</li>
	<li>Blowup</li>
</ul>
<h2 id="nonlocalcauchyproblem">Nonlocal Cauchy Problem</h2>
Nonlocal coupled system of two fields each of the flavor flavor

$$u_{tt}=[\beta*(u+g(u))]_x$$

with assumptions that
$$0≤\hat{\beta}(\xi)≤C(1+\xi^2)^{-r/2}.$$

Examples include certain coupled improved Boussinesq Equations. Such systems have been studied by Godefroy 1998 and Wang, Li (2009). The system models interaction of transverse waves in an elastic medium.

GWP and Blowup for a coupled system with $\beta = e^{-|x|}$ is open.
<h2 id="lwp">LWP</h2>
Local Lipschitz continuity of the right hand side of the system using pointwise in time estimates coming from Sobolev control of $L^\infty$.
<h2 id="gwp">GWP</h2>
Define an operator $P$ which plays the role of $\nabla$ in the energy depending upon $\beta$.

The nonlinearity for the system is assumed to arise from a Lagrangian/Hamiltonian formulation. Thus, we have a conserved energy. We then prove some Sobolev style bounds adapted to $Pu$ generalizing the case of $\nabla u$. With lower bounds on the potential energy, she obtains globalizing control.

Gronwall is used to show that the energy density stays bounded….
<h2 id="blowup">Blowup</h2>
Adaptation of the virial identity (following Godefroy 1998) shows that negative energy solutions explode.

(This strikes me as something that could be explored further from the generalized virial identity point of view.)
<h2 id="postlude">Postlude</h2>
I suggested that they look at the <a href="http://www.iumj.indiana.edu/IUMJ/FULLTEXT/1991/40/40003">KPV paper</a> and to try to imitate Morawetz-type calculations using the generalized virial identity.

<hr />

<h1 id="g.m.musluistanbultechnicaluniversity">G. M. Muslu (Istanbul Technical University)</h1>
<strong>The Cauchy problem for the one-dimensional nonlinear peridynamic model</strong>

(joint work with H. Erbay, A. Erkip, G. Muslu)
<ul>
	<li>Motivation</li>
	<li>Peridynamic Model</li>
	<li>LWP</li>
	<li>GWP</li>
	<li>Blowup</li>
</ul>
<h2 id="needforanewtheoryofsolidmechanics">Need for a new theory of solid mechanics</h2>
For example, across a crack we have discontinuities across. We need a theory which replaces PDEs with integral equations. The peridynamic model was first proposed by Silling in 2000.
<h2 id="peridynamicmodel">Peridynamic Model</h2>
Classical elasticity

$$\rho_0 u_tt = (f(u_x))_x$$

Peridynamic theory

$$\rho_0 u_tt = \int f(u(y,t) - u(x,t), y-x)dy$$

Newton’s third law demands that $f(η,ξ)=-f(-η,ξ)$. There are many studies on the modelling but there is relatively little mathematical analysis. Our aim is to study the nonlinear problem.
<h2 id="lwp">LWP</h2>
For convenience, we study $f(η,ξ)=β(ξ)g(η)$ where $\beta$ is even and $g$ is odd and $g(0)=0.$

Analysis in an appropriate space (pointwise in time tricks) leads to a LWP result. The treat the continuous and bounded case and the $C^1$ and bounded case. They also treat the $H^s \cap L^\infty$ case for all polynomial nonlinearities.
<h2 id="energyidentity">Energy Identity</h2>
$$E=\|u_t|^2+ \int \int \beta(y-x) w(u(y,t)-u(x,t)) dydx$$

Nice symmetrization tricks based on even/odd leading to energy identity.
<h2 id="blowup">Blowup</h2>
Concavity result. Negative energy solutions blowup.

<hr />

<h1 id="goncaakihttp:www.mat.univie.ac.atwkaki.htmgoncaakiweierstrassinstituteberlin"><a title="Gonca Aki" href="http://www.mat.univie.ac.at/~wk/Aki.htm">Gonca Aki</a> (Weierstrass Institute, Berlin)</h1>
<strong>Thermal effects in gravitational Hartree systems</strong>

(part of Ph.D thesis, joint w. Jean Dolbeaut and Christof Sparber)

Intersted in self-gravitating quantum particles. We represent this by density matrix operator. We are given a total mass of the system which is the integration of the occupation numbers over all occupation sites.

Energy is the kinetic energy of each state plus an interaction term described using the occupation number operators.

Variational problem corresponding to $H^1$ expressed in terms of the density matrices $\rho$.

The free energy is lower bounded by the kinetic energy using the Hardy-Littlewood-Sobolev inequality.

ack....the talk is dense and  fast for me to keep up this way, maybe even without trying to type but I like this stuff!.

Defines a notion of maximal temperature, which could perhaps be infinity. Minimizers satisfy an EL equation so we know more about them.

Compensated compactness leads to proof of existence of minimizers. Obital stability follows. Positivity of critical temperature for all $M&gt;0$. This extends a theorem of Lieb who showed the minimizer was a pure state when $T=0$ to the setting of $T \in [0, T_c]$. They have also found an explicit expression of the value of
$T_c$

Remarks for finite maximal temperature: For $\beta (s)=s^p$ with $p∈(1,7/5)$ , the maximal termperautre is finite.

<hr />

<h1 id="louisjeanjeanuniversitdefranche-comtbesanconfrance"><a href="http://www-math.univ-fcomte.fr/pp_Annu/LJEANJEAN/">Louis Jeanjean</a> (Université de Franche-Comté, Besancon, France)</h1>
<strong>Stability and instability results for standing waves of quasi-linear Schrödinger equations</strong>

(joint with M. Colin and M. Squassina)

<a href="http://profs.sci.univr.it/~squassina/papers/lavori/CJS-I.pdf">Nonlinearity 23 (2010), 1353-1385</a>

Many other issues can be studied. Lots of open problems.

$$i\phi_t+ \Delta \phi + \phi \Delta |\phi|_2+f(|\phi|_2)\phi=0$$
<h2 id="cauchyproblem">Cauchy Problem</h2>
We will first address the Cauchy problem. Next, we will study the traveling waves and their stability.

Poppenberg, JDE 172 (2001) proved LWP in $H^\infty$.

New energy term: $\int|\phi|^2 |\nabla|\phi|^2 dx$

Cauchy problem is based on work of M. Colin, CPDE 27 (2002), 325-354. This is based on energy methods to overcome the loss of derivatives induced by the quasi-linear term, gauge transforms, ….

OPEN: Solve the local Cauchy problem under more general conditions on the nonlinearity and on the data. Look for global existence results.
<h2 id="standingwaves">Standing Waves</h2>
Ansatz:
$$\phi_\omega= u_\omega (x) e^{-i\omega t}.$$

A calculation shows that

$$-\Delta u - u \Delta(|u|^2) + \omega u = |u|^{p-1}.$$

$$&lt;m_\omega = \inf\{ E_\omega (u): u is a nontrivial weak solution of the elliptic problem.\}$$

The results identified a new critical threshold. We have $1+ \frac{4}{N}$ as usual but this problem also involves $3 + \frac{4}{N}$.

<hr />

<h1 id="henrikkalischhttp:folk.uib.nohka002kalischu.bergennorway"><a title="Kalisch" href="http://folk.uib.no/hka002/">Henrik Kalisch</a> (U. Bergen, Norway)</h1>
<strong>Conservation equations for long wave models and applications to undular bores</strong>

This is basically a modeling problem. There will not be a single proof in this.
(joint work with Al Fati Ali and Magnar Bjorkavag)

<strong>Surface Waves</strong>

Assume the fluid is incompressible, inviscid, two dimensional, irrotational, assumption that the wave does not overturn.

Euler equations, some boundary conditions at surface and at bottom. The LWP problem has been solved in just the last 10 years or so. Numerically, this is a difficult problem. The problem is often simplified by putting long wavelength or small amplitude assumptions.

Long wavelength gives the shallow water wave equations. Shallow water waves equation looks like a coupled system of Burger’s equations. There are an infinite number of conserved quantities in the shallow water wave equations.

Small amplitude case is known as the Airy theory. Rewrite Euler in terms of the velocity potential but you still have the boundary conditions. The pressure is removed. Linearize the Bernoulli equation on the boundary and calculate the dispersion formula by putting in plane waves. It emerges that $\omega^2=g k \tanh(h_0 k)$.

One can compare the dispersion relation for the KdV, BBM and water wave formulae. KdV is a bad model for water waves since