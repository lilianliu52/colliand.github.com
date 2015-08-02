---
layout: post
category : lessons
tags : [Notes, USA, IAS]
comments: false
---
<!---->

<a href="http://www.math.ias.edu/">IAS School of Mathematics</a>

<img src="https://www.math.ias.edu/pictures/math/simonyi-blossoms.jpg" alt="Simonyi Hall" />

<a href="http://www.math.ias.edu/wsd2">Workshop web page</a>

Happy Einstein Birthday!

<img src="http://upload.wikimedia.org/wikipedia/commons/thumb/f/f5/Einstein_1921_portrait2.jpg/220px-Einstein_1921_portrait2.jpg" alt="Albert Einstein" />
<h2 id="wednesday:2012-03-13">Wednesday: 2012-03-13</h2>
<ul>
	<li>9:00 - 10:00    Wilfrid Gangbo, Georgia Institute of Technology, “Lifting absolutely continuous curves from P(Td) to P2(Rd)”  <a href="https://www.math.ias.edu/files/hofer/gangboab.pdf">abstract</a></li>
	<li>10:15 - 11:15  Jonatan Lenells, Baylor University, “Geometry of diffeomorphism groupos, complete integrability and optimal transport”  <a href="https://www.math.ias.edu/files/hofer/lenellsab.pdf">abstract</a></li>
	<li>11:30 - 12:30   David Ebin, SUNY, “Groups of diffeomorphisms and geodesics on them”  <a href="https://www.math.ias.edu/files/hofer/ebinab.pdf">abstract</a></li>
	<li>2:30 - 3:30       Susan Friedlander, University of Southern California, “Well / Ill-posedness results for the magneto-geostrophic equations: the importance of being even”.  <a href="https://www.math.ias.edu/files/hofer/friedlanderab.pdf">abstract</a></li>
</ul>
<h1 id="wilfridgangbohttp:people.math.gatech.edugangbo:liftingabsolutelycontinuouscurvesfromptdtop_2rd"><a href="http://people.math.gatech.edu/~gangbo/">Wilfrid Gangbo</a>: <em>Lifting absolutely continuous curves from $P(T^d)$ to $P_2(R^d)$</em></h1>
<img src="http://www.math.buffalo.edu/mad/PIX/gangbo_wilfrid.jpg" alt="Wilfrid Gangbo" />

(chalk talk; joint work with A. Tudorascu)

This work extends earlier work on the space of probability measures on the torus $P(T)$ to analogous results on $P(T^d)$. The earlier work used the embedding $P(T) \rightarrow L^2 (0,1)$ but we don’t have this embedding in the higher dimensional case.

Let $P_2 (R^d)$ be the set of Borel measures on $R^d$ with finite second moment $\int |x|^2 \mu (dx) &lt; \infty$. We say $\mu_0 \thicksim \mu_1$ if and only if $\int F d\mu_0 = \int F d \mu_1 ~ \forall F \in C(T^d), ~ \forall F \in C(R^d), ~ \forall F(x+z) = F(x), z \in Z^d$.

I define $P(T) = P(T^d)/\thicksim$.

Let $\gamma$ be a measure on $R^d \times R^d$ which satisfy $\pi_1$ # $  \gamma = \mu_0$ and $\pi_2$ # $ \gamma = \mu_1$.
More generally, we write
$$W^2_2 (\mu_0, \mu_1) = \inf_\gamma \int_{R^d \times R^d} |x-y|^2 \gamma (dx, dy).$$

<strong>Problem:</strong> Data: $v:(0,T) \times T^d \rightarrow R^d$ and $t \rightarrow \sigma_t \in P(T^d)$. Assume that $\partial_t \sigma_t + \nabla \cdot (\sigma v) = 0$ (in the sense of distributions). Can we find $t \rightarrow \hat{\sigma_t} \in P_2 (R^d)$ and $\hat{v}: (0,T) \times T^d \rightarrow R^d$ such that $\partial_t \hat{\sigma} + \nabla \cdot (\hat{\sigma} \hat{v}) = 0$ in the sense of distributions. Here $\hat{\sigma_t} \thicksim \sigma_t.$

Such a lift becomes important if I want to associate the rotation number. I want to write
$$
\frac{d}{dt} \int_{T^d} x d \sigma_t = \int_{T^d} v_t d \sigma_t$.
$$

<strong>Weak KAM:</strong> (A small fraction of what is known) $M= T^d$. Let $h: T^* M \rightarrow R$. Let $w(z_0, z_1) = z_0 (J z_1)$ where $J$ is the usual matrix satisfying $J^2 = - Id$.  Let $X_h$ denote the associated Hamiltonian vector field:
$$
\dot{\phi} = X_h (\phi), \phi_0 = (x_0, p_0).
$$
The associated flow is denoted $\phi_t = (x_t, p_t).$

<strong>Existence of weak Lagrangian Tori:</strong> $\overline{h}: R^d \rightarrow R$ is the effective Hamiltonian, $ c \in R^d$.
<ol>
	<li>$\exists ~ u \in C(t^d)$ with $h(x, c+ \nabla u) = \overline{h} (c)$ (viscosity)</li>
	<li>$u_c (x) = c \cdot x + u(t).$ ($\partial u_c$ is invariant under $\phi$.)</li>
	<li>$\forall ~ x_0 \in T^d ~ \exists v_0 $ such that if $(x_t, p_t) = \phi_t$ then $\forall ~ T$
$$
u(x_T) - u(x_0) = \int_0^T [l(x,\dot{x}) + c \cdot \dot{x} + \overline{h} (c)] dt$$
$$
\lim_{t \rightarrow \infty} \frac{\hat{x_t}}{t} = - \nabla \overline{h} (c).
$$</li>
</ol>
<strong>General Fact:</strong> $M \rightarrow $ compact.

<strong>Specific to finite $d$:</strong>

Given $x \in W^{1,2} (0,T, T^d)$ and take two lifts $\hat{x}, \hat{y} \in W^{1,2, R^d}$. We then find that
$$
\hat{x_t} - \hat{y_t} = n \in Z^d
$$
because we have
$$
\lim_{t \rightarrow \infty} \frac{\hat{x_t}}{t} = \lim_{t \rightarrow \infty} \frac{\hat{y_t}}{t}
$$

<strong>Obstacle in infinite dimensions:</strong>

Let $M_0 = P(T^d)$ and in the sense of distributions we have
$$\partial_t \sigma + \nabla \cdot (\sigma v) = 0.$$

If $\nabla \cdot (\sigma w) = 0$ then $v+w$ is another velocity.

(wash board…)

Let $\mu \in P_2 (R^d)$ and define the tangent space $T_\mu P_2 (R^d)$ and also the space $T_\mu P(T^d)$. These are defined with $L^2$ closures.

<strong>Pseudo symplectic form:</strong> ….going faster and I’m not keeping up with the typing.

<strong>Theorem (Gangbo-Kun-Pacuni 2011):</strong>
<ol>
	<li>$\Omega$ is a closed skew symmetric nondegenerate 2-form.</li>
	<li>$\exists ~ X_H$ such that $ -dH = \Omega (X_H, \cdot)$.</li>
	<li>$\dot{f} = X_H (f) \iff \partial_t f + \nabla_x (vf) = \nabla_v (f (\nabla V + \nabla W * \rho)).$</li>
</ol>
This is a nonlinear Vlasov equation.

I want to state the analog of the weak KAM theorem in our context.

<strong>Theorem</strong> Let $\overline{H}$ be the effective Hamiltonian of $H$ restricted to $R^d$ and let $c \in R^d$.
<ol>
	<li>$\exists ~ U: P(T^d) \rightarrow R$ such that (in viscosity sense)
$$ H(\mu, c + \nabla_w H) = \overline{H} (c). $$</li>
	<li>Given $\sigma_0 \in P(T^d) ~ \exists ~ v_0: T^d \rightarrow R^d$ such that if $f_0 = \sigma_0 \delta_{{v0}}$ then
$$
f_t = \sigma_t \delta_{{vt}},
$$
$$
U(\sigma_t) - U(\sigma_0) = \int_0^T [ L(\sigma_t, v_t) + \int_{R^d} v_t \cdot c d\sigma_t + \overline{H} (c)] dt.
$$</li>
	<li>We also have
$$
| \frac{1}{T} \int_0^T  dt \int_{R^d} v_t d\sigma_t +\nabla \overline{H} (c) | \leq \frac{const}{\sqrt{T}}.
$$</li>
</ol>
<strong>Corollary:</strong> If $(\hat{\sigma}, \hat{v_t})$ is an appropriate lift then
$$\lim_{T \rightarrow \infty} \frac{1}{T} \int_0^T ( \int_{R^d} x d\sigma_t) dt = - \nabla \overline{H} (c).$$

<strong>Questions:</strong>

Mather: This has connections with fluids?

Answer: Kinetic theory. Consider the system $ \partial_t^2 x = \frac{1}{N} \sum_{j=1}^N W(x_i - x_j) - \nabla V(x_i)$. When we consider the $N \rightarrow \infty$ limit, we can move the weak KAM theory from this $N$ particle system to the infinite particle case by moving to the setting of measures. This framework lets us prove convergence of discrete models to the PDE case.
<h1 id="jonatanlenellshttp:www.baylor.edumathindex.phpid75442:geometryofdiffeomorphismgrouposcompleteintegrabilityandoptimaltransport"><a href="http://www.baylor.edu/math/index.php?id=75442">Jonatan Lenells</a>: <em>Geometry of diffeomorphism groups, complete integrability and optimal transport</em></h1>
<img src="http://www.baylor.edu/content/imglib/118978.jpg" alt="Jonatan Lennells" />

(pdf slides; Happy $\Pi$ day!; Einstein’s birthday)

(joint work with B. Khesin, G. Misiolek, S. Preston)
<h2 id="outline">Outline</h2>
<ul>
	<li>A new equation</li>
	<li>Geometry of $Diff(M)$</li>
	<li>A sphere</li>
	<li>Optimal Transport</li>
	<li>Geometric Statistics</li>
</ul>
<h2 id="anewequation">A new equation</h2>
$$ \rho_t + u \cdot \nabla \rho + \frac{1}{2} \rho^2 = \frac{- \int_M \rho^2 d \mu}{2 \mu(M)}.
$$
<ul>
	<li>$M$ is a compact Riemannian manifold.</li>
	<li>$\mu(M)$ is the volume of $M$.</li>
	<li>This is an exciting equation because it is completely integrable for any $M$.</li>
	<li>This is a geodesic equation on $Diff(M)/Diff_\mu (M)$.</li>
	<li>Describes $\dot{H}^1$-optimal transport</li>
	<li>reduces to the Hunter-Saxton equation for $M=S^1$. (derived in the context of liquid crystals in the early 90s.)</li>
</ul>
Euler-Arnold Equations. Summary of those ideas.

abc-metric. You can add some other terms to the original $L^2$ inner product involving $L^2$ inner products involvling codifferentials and the musical isomorphism. A lot of different equations arise as you take different values of the parameters. Writing down the associated abc Euler-Arnold equation generates a big equation which can be specialized into various equations. To obtain the $\dot{H}^1$ metric, we cancel away the terms associated with factors a and c. We simplify by setting $a=0, b= \frac{1}{4}, c = 0$.

The equation induced by these choices has some degeneracy issues. These can be resolved by quotienting out part of the phase space. The function $u$ is not uniquely determined but its coset is uniquely determined. (Similar issues arise in Hunter-Saxton.) The equation we are considering here is a geodesic equation on a (quotiented) Diffeomorphism group.

Jacobian determinant.
<h2 id="asphere">A sphere</h2>
<strong>Theorem (Khesin-Misiolek-Lennels-Preston):</strong> The map which takes the coset $[\eta]$ to its associated Jacoobian $\sqrt{Jac_\mu \eta}$ is an isometry onto a subset of the sphere.

This isometry lets them transport all the questions about the geodesic equation on this complicated Diff phase space into corresponding questions about geodesics on the sphere. Since we understand the sphere well, we can conjugate results there using the mapping to obtain explicit solution formulae for the geodesic equation. Magical integrability!

Preceding works.

<strong>Khesin-Misiolek 2003:</strong> Showed Hunter-Saxton may be viewed within the Euler-Arnold framework.

<strong>Lennels 2006:</strong> Recognized the image of the map as a portion of the sphere.
<h2 id="optimaltransport">Optimal Transport</h2>
Optimal Transport. Wasserstein distance between two probability measures.

<strong>Moser 1965</strong>, <strong>Ebin-Marsden 1970</strong>, <strong>Otto 2001</strong>, also <strong>Benamou-Brenier</strong>.

The $\dot{H}^1$ optimal distance induces what they call the spherical Hellinger distance since it resembles the Hellinger distance used in probability theory
<h2 id="geometricstatistics">Geometric Statistics</h2>
Statistical model.

Fisher-Rao information metric.

<strong>Theorem (KMLP):</strong> The  $\dot{H}^1$ metric coincides with the Fisher-Rao metric when restricted to any k-dimensional submanifold of the (quotiented) $Diff$.

This is another reason why we think this metric is important. It arises from many different points of view.
<h2 id="summary">Summary</h2>
<ul>
	<li>We found a new integrable PDE.</li>
	<li>The PDE is a geodesic equation on a quotieted diff with  $\dot{H}^1$ metric.</li>
	<li>A sphere</li>
	<li>One can understand what is going on using the optimal transportation point of view using the $\dot{H}^1$ metric.</li>
	<li>This metric coincides with a basic metric arising in geometric statistics.</li>
</ul>
<h2 id="openproblems">Open problems</h2>
<ul>
	<li>Global weak solutions of the PDE? All solutions break in finite time because you hi the boundary of the diffeomorphism coset. However, there is no problem when you view the dynamics on the sphere. The motion along the great circle may be continued. This type of development has taken place already in the context of the Hunter-Saxton equation. The process appears to be more complicated in this more general context since the Jacobian can vanish.</li>
	<li>Transfer results from geometric statistics into this diffeomorphism quotient. Then reinterpret these objects in the setting of PDE.
<strong>Amari-Nagaoka 2000</strong> alpha-connections, dual connections.</li>
	<li>Develop an optimal transport theory based on the $\dot{H}^1$ theory.</li>
	<li>Find a Lax pair.</li>
	<li>Find a bi-Hamiltonian structure.</li>
	<li>Analyze the associated two-component equation (c.f. <strong>Lennels-Zhao 2011</strong>). There is a 2-component Hunter-Saxton so that object suggests we might find a corresponding generalization. This has been observed by LZ.</li>
</ul>
<h1 id="davidebinhttp:www.math.sunysb.eduebin:groupsofdiffeomorphismsandgeodesicsonthem"><a href="http://www.math.sunysb.edu/~ebin/">David Ebin</a>: <em>Groups of diffeomorphisms and geodesics on them</em></h1>
<img src="http://www.math.sunysb.edu/~ebin/ebin-face.jpg" alt="David Ebin" />

(joint work with <a href="http://math.colorado.edu/~prestos/">Stephen Preston</a>)

Maps from a manifold to itself. Discussion of various topologies of such maps.
<ul>
	<li>Volume preserving maps. Diffeomorphisms (Volumorphisms)</li>
	<li>Even dimensional manifolds with a symplectic form. We can consider the maps which preserve the symplectic form. (Symplectomorphisms)</li>
	<li>For odd dimensional manifolds, we can consider maps which preserve the contact form. (Contactomorphisms)</li>
</ul>
In all these cases, we can discuss the geodesics…..ack low battery.

Boothby-Wang fibration.
<h1 id="susanfriedlanderhttp:cams.usc.edususanfri:wellill-posednessresultsforthemagneto-geostrophicequations:theimportanceofbeingeven"><a href="http://cams.usc.edu/~susanfri/">Susan Friedlander</a>: <em>Well / Ill-posedness results for the magneto-geostrophic equations: the importance of being even</em></h1>
<img src="http://uscnews.usc.edu/assets_c/2010/08/Friedlander-thumb-167xauto-17935.jpg" alt="Susan Friedlander" />

(joint work with Vlad Vicol, Walter Rusin, Francisco Gancedo, Weiran Sun)

Homage to Oscar Wilde…

Amain theme is that there is a difference in behavior of solutions in Active Scalar Equations when the associated Fourier multiplier is even versus odd.
<h2 id="activescalarequationsincompressiblefluids">Active Scalar Equations; Incompressible Fluids</h2>
$$\theta_t + u \cdot \nabla \theta =0. $$
$$ \nabla \cdot u = 0. $$

$$ u = O [\theta], ~ PDO $$

$R^d$ or $T^d$. Even or odd Fourier multiplier symbol. The results I’ll describe are not influenced by the presence of a physical boundary. The emphasis will be on examining the influence of the operator O on the properties of the PDE.

Consider $u_j = \partial_i T_{ij} \theta, ~ \nabla \cdot u = $. Here $T_{ij}$ is a $d \times d$ Calderon-Zygmund operators.
<ul>
	<li>ODD Symbol: Locally well-posed in Sobolev spaces. Commutator in energy estimates. **Chae et. al, Friedlander-Vicol.</li>
	<li>EVEN Symbol: Lipschitz ill-posed in Sobolev spaces. <strong>Friedlander-Vicol</strong>; Nonuniqueness for $L^\infty$-weak solutions. Techniques from convext integration. <strong>Shuydkoy</strong>.</li>
</ul>
Recent reviews of results for certain active scalar equations. <a href="http://www.math.wisc.edu/~kiselev/mmnparc.pdf">“Regularity and blowup for active scalars”</a> <strong>Kiselev 2010</strong>.

<strong>SQG Equation</strong>: $u = R^\perp \theta$, symbol $\frac{i (k_2, -k_1)}{|k|}$.

<strong>Constantin-Majda-Tabak 1994, Resnick 1995 (Chicago thesis; unpublished), Wu, Cordoba, Chae, Iyer, Ju, Fefferman</strong>

The SQG equation had been known in the geophysics community before its introduction to the mathematical community by Constantin et.al.

Local existence for smooth initial data BUT global existence of smooth solutions is OPEN (just as it is open for 3D Euler). Cordoba and Fefferman have ruled out the existence of certain solution scenarios.
<h2 id="modifiedsqgequationokhitani">“Modified” SQG Equation (Okhitani)</h2>
Insert a power of $(-\Delta)^{1/2} = \Lambda$ in the map $\theta \rightarrow u$ so that
$$
u = \nabla^\perp \Lambda^{\beta-2} \theta
$$
where $1 &lt; \beta \leq 2. <strong>Chae, Constantin, Cordoba, Ganceda, Wu 2011</strong>. Local existence of smooth solutions in $H^s$, global existence of weak solutions.

Note: result holds more generally when the symbol is ODD and order $\leq 1$.
<h2 id="ipmequation:singularintegraloperatorwithevensymbol">IPM equation: singular integral operator with EVEN symbol</h2>
Darcy’s law.

$$ u = R^\perp R_1 \theta. $$

<strong>Cordoba-Gancedo-Orive 2007</strong>

Regular initial data, local existence, weak solutions, SQG and IPM present different behaviours. Global existence of smooth solutions is OPEN.

Even symbol:
$$( \frac{k_1 k_2}{|k|^2}, \frac{-k_1^2}{|k|^2}).$$

There is very different behaviors among these equations for rough data. “Patch type initial data”
<h2 id="sipmequationsevenunbounded">SIPM equations (even, unbounded)</h2>
$$ u = R^\perp R_1 \Lambda^\beta \theta$$

<strong>Friedlander-Gancedo-Sun-Vicol (2012)</strong>
<ul>
	<li>Locally Lipschitz ill-posed in $H^s, ~ s&gt;2$. Proved for $0 &lt; \beta \leq 2$ in $T^d \times [0,\infty]$</li>
	<li>Locally well-posed for some “patch-type” weak solutions. Proved for $0&lt;\beta &lt;1 $ in $R^2$.</li>
</ul>
(Discussion: the notions of “wellposedness” changes between the previous two bullet points.)

Symbol: $k_1 k^\perp |k|^{\beta -2}$
<h2 id="magnetogeostrophicmgequations">Magnetogeostrophic (MG) equations</h2>
<strong>Friedlander-Vicol 2011</strong>

Long symbol $M$, even, unbounded, 3D. $ u = M\theta$. Here $M$ is a vector operator that defines a 3-vector $u$.

Cauchy problem is ill-posed in Hadamard sense in Sobolev spaces. There is no Lipschitz solution map.
<h2 id="ill-posedness:singularevensymbol">Ill-posedness: singular, even, symbol</h2>
Active scalar equation. Special direction with index $d$, often associated with gravity. A list of many conditions on the $d$th component $S_d$ of the Fourier multiplier operator….allowing them to build eigenfunctions to show Lipschitz failure.

<strong>Definition:</strong> Locally Lipschitz $(X,Y)$ well-posed.

$$\| \theta_1 (\cdot, t) - \theta_1 (\cdot, t)\|<em>X \leq K \| \theta</em>1 (\cdot, 0) -\theta_2 (\cdot, 0) \|_Y.
$$

The spaces $X,Y$ are often chosen to be $(H^r, H^S)$.

<strong>Theorem:</strong> Under the many assumptions on $S_d$, the active scalar equation is Lipschitz $(H^r, H^s)$-illposed for any $r &gt; R, s \geq r+1$.
<h2 id="linearproblem">Linear problem</h2>
Linearize around $\theta_0 = \sin m x_d $. Write out a Fourier series. Crank out a recurrence relation.

Continued fractions, characteristic equation. These ideas where used by Michalkin and Sinai to show unstable eigenvalues for the shear flow for Navier-Stokes equations.
<h2 id="ill-posednessofthenonlinearproblem">Ill-posedness of the nonlinear problem</h2>
Follows a proof by contradiction.
<h2 id="effectsofdissipation:mg">Effects of dissipation: MG</h2>
Dissipation: $ \nu (-Delta)^{1/2}$

Using De Giorgi techniques, Caffarelli-Vasseur proved critical SQG. What can we say about the MG equation?
<ul>
	<li>Case $1/2 M \gamma &lt; 1$: LWP in $H^s$, for $ s&gt; \frac{5}{2} + (1 - 2\gamma)$. Well-prepared initial data.</li>
	<li>Case $ 0 &lt; \gamma &lt; 1/2$: Diffusion is too weak to overcome the continued fraction construction.</li>
	<li>Case $\gamma = 1/2$: Unique global solution when the initial data and source are small in a suitable sense, then there exists a unique golbal solution. However, if the data are large in this respect then we can run the ill-posedness construction. This reveals a very precise dichotomy.</li>
</ul>
&nbsp;