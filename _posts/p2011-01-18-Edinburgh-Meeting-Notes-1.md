---
layout: post
category : lessons
tags : [notes, Edinburgh, numerics]
---

<!--?xml version="1.0" encoding="ASCII"?-->

<!-- Processed by MultiMarkdown -->

These are notes from a meeting entitled <a href="http://www.nais.org.uk/NPDE2011/Speakers.php">Advanced Numerical Studies in Nonlinear PDEs</a> in Edinburgh, Scotland.
<h1 id="waltercraigmcmaster:waterwaveinteractions">Walter Craig (McMaster): Water Wave Interactions</h1>
I’m an analyst but I’m going to talk about numerics and experiments as well as analysis. We will discuss the problem of water waves and then I’ll talk about two specific settings in which the theory has led to good and quite elegant numerics and the numerics have started to answer some questions.

(joint work with P. Guyenne and <a href="http://www.math.toronto.edu/sulem">C. Sulem</a>)

<strong>Outline</strong>
<ul>
	<li>Free surface water waves</li>
	<li>Hamiltonian PDEs</li>
	<li>Periodic Traveling wave patterns</li>
	<li>Solitary wave Interactions</li>
	<li>The KdV scaling limit</li>
</ul>
<h2 id="freesurfacewaterwaves">Free surface water waves</h2>
Euler’s equations of hydrodynamics, incompressible and irrotational flow. This is therefore given as a potential flow. The irrotational assumption is really an oceanographers assumption. Of course, there is vorticity but we follow the models of oceanographers.

The fluid domain is $-h &lt; y &lt; \eta (x,t)$. So, the domain is changing. Free surface boundary conditions hold on $y = \eta (x,t)$.
<h3 id="zakharovshamiltonian">Zakharov’s Hamiltonian</h3>
<ul>
	<li>The energy functional</li>
</ul>
$$ H = K+P $$
$$
K = \int_x \int_{-h}^{\eta(x)} \frac{1}{2} |\nabla \phi|^2 dy dx.
$$
$$
P = \int_x \frac{g}{2} \eta^2 dx.
$$

This could also include surface tension effects.
<ul>
	<li>Zakharov’s choice of variables,
$$
z = ( \eta(x), \xi(x) = \phi(x, \eta(x))),
$$
for which we consider $\phi = \phi[\eta, \xi]  (x,y)$.</li>
	<li>Express the energy in terms of $\xi$ and $\eta$. This involves the Dirichlet-Neumann operator $G(\eta)$.</li>
</ul>
<h3 id="dirichlet-neumannoperator">Dirichlet-Neumann operator</h3>
<ul>
	<li>Laplace’s equation on the fluid domain: $\Delta \phi = 0$ subject to bottom Neumann boundary condition. Free surface boundary data $\phi (x, \eta(x)) = \xi(x)$, for which the D-N operator is given by
$$
\xi(x) \longmapsto \phi(x,y) \longmapsto N \cdot \nabla \phi (1+ |\nabla_x \eta|^2)^{1/2} := G(\eta) \xi(x).
$$</li>
	<li>In these coordinates, we can rewrite the boundary conditions in a new (and nicer) form. This reexpresses the water wave problem as a Hamiltonian system in Darboux coordinates.</li>
</ul>
<h2 id="hamiltonianpdes">Hamiltonian PDEs</h2>
<ul>
	<li>KdV is a Hamiltonian PDE with a different symplectic structure.</li>
	<li>Other Hamiltonian PDEs
<ul>
	<li>shallow water equations</li>
	<li>Boussinesq</li>
	<li>KP</li>
	<li>NLS</li>
	<li>Dysthe equation</li>
</ul>
</li>
</ul>
Many of these problems arise in scaling limits of the water wave problem.

<strong>Lemma (Properties of D-N operator):</strong>
<ol>
	<li>$G(\eta) \geq 0$ and $G(\eta) 1 = 0$.</li>
	<li>$G(\eta)^* = G(\eta)$ Hermitian Symmetric</li>
	<li>$G(\eta): H^1_\xi \rightarrow L^2_\xi$ is analytic in $\eta$ for $\eta \in C^1$. There is an operator valued power series expansion of $G(\eta)$ (using a theorem of <a href="http://www.ams.org/mathscinet/search/publdoc.html?arg3=&amp;co4=AND&amp;co5=AND&amp;co6=AND&amp;co7=AND&amp;dr=all&amp;pg4=AUCN&amp;pg5=AUCN&amp;pg6=PC&amp;pg7=ALLF&amp;pg8=ET&amp;r=1&amp;review_format=html&amp;s4=christ&amp;s5=journe&amp;s6=&amp;s7=&amp;s8=All&amp;vfpref=html&amp;yearRangeFirst=&amp;yearRangeSecond=&amp;yrop=eq">Christ-Journé 1987</a>).</li>
	<li>Some explicit calculations of the Taylor expansion (I couldn’t keep up….)</li>
	<li>Conservation Laws
<ul>
	<li>Mass: $M = \int \eta dx$ (He shows the calculation using properties of $G$.)</li>
	<li>Momentum: Similar calculation</li>
	<li>Energy: Easy since the commutator of $H$ with itself vanishes.</li>
</ul>
</li>
	<li>Taylor expansion of the Hamiltonian</li>
	<li>Linearized equations; comparison with the harmonic oscillator.</li>
</ol>
<h2 id="periodictravelingwavepatterns">Periodic Traveling wave patterns</h2>
<ul>
	<li>Can I find traveling wave solutions?
$$ \eta(x,t) = \eta ( x-tc); \xi(x,t) = \xi(x - tc) $$</li>
	<li>Spatially periodic, $\Gamma \subset {\mathbb{R}^{d-1}}$.
$$
\eta(x + \gamma, \cdot) = \eta(x, \cdot), \xi(x+\gamma, \cdot) = \xi(x, \cdot), ~ \forall \gamma \in \Gamma.
$$</li>
</ul>
On such domains, we can use the Fourier tranform.

<strong>Rk:</strong> Notice this is a mathematician imposing a period rather than the physics making that selection. More can be said in this direction, but let’s proceed this way.

<strong>Rk:</strong> These (time independent) traveling wave patterns can be imagined to emerge in transient interactions in seas. The nonlinear actions create large amplitudes and this might be related to the phenomena of <em>freak waves</em>.
<h3 id="equationsfortravelingwaves.">Equations for traveling waves.</h3>
Periodic traveling wave patterns are <em>critical points</em> of the Hamltonian on the variety $I = const$, with Lagrange multiplier $c \in {\mathbb{R}^{d-1}}.$

This leads to a bifurcation problem.

<strong>brief history (dimension $d=2$):</strong>
<ul>
	<li>Levi-Civita 1925; existence of traveling waves</li>
	<li>Struik 1926; traveling waves case</li>
	<li>Zeidler 1971</li>
	<li>Beale 1979</li>
	<li>Jones-Toland 1985</li>
</ul>
<strong>brief history (dimension $d=3$):</strong>
<ul>
	<li>Reeder Shinbrot 1981</li>
	<li>Sun 1986</li>
	<li>Craig-Nicholls 2000</li>
	<li>Iooss-Plotnikov-Toland 2000 (small divisor problem)</li>
</ul>
He shows a picture from the wave tank at Penn State. He then shows some numerics which are trying to model those observations and they look beautiful.

<strong>Kuksin Question:</strong> Stability of these patterns?
<blockquote><strong>Craig Answer:</strong> This is a very good question. I don’t know results like that. This is related to Benjamin-Feir. McLean showed instability for $d = 3$. Some further discussion….We need the Bloch theory of stability for these wave patterns. This appears to be difficult analytically so might need some numerical studies at first. There are instability zones….</blockquote>
<h2 id="solitarywaveinteractions">Solitary wave Interactions</h2>
Solitary waves in 2-dimensions (Friedreichs-Hyers 1954, Amick-Fraenkel-toland 1980s)
<ul>
	<li>Head-on collisions of solitons.</li>
</ul>
The numerics reveal some inelasticity in the collision. We’d like to understand those. If we make the amplitude of the solitons bigger, the dispersive ripples are more visible.
<h2 id="thekdvscalinglimit">The KdV scaling limit</h2>
<strong>Titi’s Question:</strong> Can we reduce to the surface equations including rotation?
<blockquote><strong>Craig’s Answer:</strong> Yes and No. You can make a rotation depending purely on y and impose that. Then it is reducible. But this is rather artificial. There is stuff that happens in the middle which is not a surface effect. Therefore, this problem requires a more complete analysis of the Euler equation and will not collapse to a system on the surface.</blockquote>

<hr />

<h1 id="sergeynazarenkowarwick:assumptionstechniquescahllengesinwaveturbulence">Sergey Nazarenko (Warwick): Assumptions, Techniques, Cahllenges in Wave Turbulence</h1>
This is not so much about new result. Instead, this is an attempt by a physicist trying to explain wave turbulence ideas being explored by physicists to mathematicians. My view is that there is a lot of interesting work to be done. Lots of open problems….
<h2 id="whatiswaveturublence">What is wave turublence?</h2>
He shows a picture of a relatively calm seashore from Nice. He emphasizes there is a wide range fo scales in these problems. <strong>WT is a statistical system of nonlinear waves</strong>.

Examples:
<ul>
	<li>Water waves</li>
	<li>Waves in rotating and stratified fluids (internal and inertial waves, Rossby waves)</li>
	<li>Plasma waves</li>
	<li>Waves in Bose-Einstein condensates</li>
	<li>Kelvin waves on quantized vortex filnments</li>
	<li>MHD turbulence in interstellar turbulence and solar wind</li>
	<li>Nonlinear optics</li>
	<li>Solids: phonons, spin waves. Kinetics of phonons in weakly anharmonic crystals is a first example of study in tis direction (1920s). I didn’t catch the name….</li>
</ul>
He shows a picutre of a wave take of Lukaschuk.

Waves in fusion plasmas. Shows a picture of a Tokamak. Drift wave turbulence causes anomalous heat and particle loss - major problem for fusion. The devices have grown larger and larger basically to carry out the confinement for a longer period of time.

MHD turbulence in astrophysics. He shows some data from the <a href="http://swoops.lanl.gov/">Ulysses/Swoops (los alamos) solar wind studies</a>.

Bose Einstein Condensates <a href="http://www.warwick.ac.uk/~masbu/BEC_physca_D_06.pdf">Nazarenko-Onorato 2006</a>:
<ul>
	<li>Inverse cascade - condensation</li>
	<li>Condensate strongly affects WT</li>
</ul>
Quantum Turbulence (see Lvov et. al. 2007) (Superfluid turbulence)
<ul>
	<li>Kelvin waves on quantized vortex filaments</li>
	<li>Interaction with hydro eddies (vortex bundles) is important</li>
	<li><a href="http://www.springerlink.com/content/50681u4055x504x6/fulltext.pdf">Kelvin Wave Turbulence</a></li>
</ul>
Optical Turbulence
<ul>
	<li><a href="http://www.opticsinfobase.org/view_article.cfm?gotourl=http://www.opticsinfobase.org/DirectPDFAccess/F8C107B3-00CC-CFB9-2FA6C8440558385A_188671.pdf%3Fda%3D1%26id%3D188671%26seq%3D0%26mobile%3Dno&amp;org=Univ%20of%20Edinburgh%20">Bortolozzo et. al 2008</a></li>
	<li>This project studies nonlinear corrections (coming from the optical physics) which are included beyond the 1d NLS model.</li>
</ul>
<strong>Kuksin Question:</strong> Which corrections? Can you write them down?
<blockquote><strong>Nazareknko:</strong> Something like a DNLS correction…not so clear.</blockquote>
<h2 id="ingredientsintheapproach">Ingredients in the approach</h2>
He writes $NLS_3^\pm (T^d)$ and comments that this is a physically reasonable model but we are really interested in the study in infinite space with finite energy density.

He reexpresses the NLS equation in Fourier language.

Set of wave modes: amplitudes and phases.

N-mode joint probability density function. Some notation….probability…sectors in the wave modes setting.
<h3 id="randomphaserpandrandomphaseamplituderpasystems">Random Phase (RP) and Random Phase Amplitude (RPA) systems</h3>
RP:

All phases are independent random variables such that uniformly distributed on $S^1$.

RPA:
<ol>
	<li>All amplitudes and all phases are independent random variables.</li>
	<li>All phases are uniformly distributed on $S^1$.</li>
</ol>
Note: RPA does not mean Gaussian. Nevertheless, we have obtained successful closures without assuming the Gaussian statistics.

Frog Jumps!
<ul>
	<li>expanding in small nonlinearity</li>
	<li>Assuming RP at $t=0$.</li>
	<li>Taking limit of a large box followed by the limit of small nonlinearity.</li>
</ul>
(The order of these steps is important.)

Evolution of joint PDF? We can derive the evolution equation under these assumptions. The derivation is rather systematic, in fact it is perhaps rigorous.

Mathematical Challenges:
<ul>
	<li>WT is formally derived for $t=0$.</li>
	<li>Does it work at the long time of nonlinear evolution?</li>
	<li>Does RPA survive over this time?</li>
	<li>Adding forcing and dissipation: will WT describe the steady state?</li>
</ul>
<blockquote>Hmmmm….This RPA condition at $t=0$ reminds me a bit of the assumption of product wave function in the QMB theory. The dynamics in the Hartree derivation might drive the multiparticle wave function away from the product case. Here we have a dynamic that might drive us away from the RPA condition.</blockquote>
Evolution of 1-mode PDF.

Kinetic equation (Hasselmann 1962).

Kolmogorov-Zakharov state.
<ul>
	<li>Explained a steady state spectrum corresponding to energy cascade.</li>
	<li>Exact solution of the asymptotic closure.</li>
</ul>
Numerics and Analysis of KE.
<ul>
	<li>What is the role of KZ solutions with respect to the thermodynamic Rayleigh-Jeans state?</li>
	<li>Similar issues for the classical Boltzmann equation.</li>
</ul>
Zakharov was awarded the 2003 Dirac Medal for “putting the theory of wave turbulence on a firm mathematical ground”! What is it that we want to do?

<hr />

<h1 id="gregortannernottingham:awavechaosapproachtowardsdescribingthevibro-acousticresponseofengineeringstructures">Gregor Tanner (Nottingham): A wave chaos approach towards describing the  vibro-acoustic response of engineering structures</h1>
(Joint work with D. Chappel, Stefano Gianai, Hanya Ben Hamdin, Dmitrii Maksimov)

This talk is more directed toward engineering applications. inuTech is an industrial collaborator.

Overview:
<ul>
	<li>Introduction - the need for numerical short wavelenght methods in vibroacoustics</li>
	<li>From wave equations to the Liouville equation</li>
	<li>Solving the Liouville equation - a boundary integral approach (Dynamical Energy Analysis - DEA)</li>
	<li>Tackling the Midfrequency problem - hybrid methods</li>
	<li>Numerical results</li>
</ul>
Aim: predicting wave intensity distributions for the vibro-acoustical response of mechanical structures. Think of a car. Companies like Bombardier and Airbus use these methods. It is a difficult problem. You want these structures to be quite and with no noise in the interior.

Where is the problem?

Techniques:
<ul>
	<li>Low frequencies - wavelength around the size of the object</li>
	<li>Finite Element method</li>
	<li>Boundary elemtn method</li>
	<li>plane wave methods</li>
</ul>
High Frequencies:
<ul>
	<li>Ray tracing</li>
	<li>Statistical energy analysis</li>
	<li>…</li>
</ul>
Midfrequency problems:
<ul>
	<li>Structures with large variations in the local wavelength. (Large variations in the stiffness of components, ie body frame and side panels.)</li>
	<li>Hybrid methods. Try to connect exact numerical methods with the statistical methods.</li>
</ul>
<h2 id="shortwavelengthapproximations-fromwavechaostostatisticalmethods">Short wavelength approximations - from wave chaos to statistical methods</h2>
<ul>
	<li>Wave chaos -short wavelength asymptotics
<ul>
	<li>Keller</li>
	<li>Gutzwiller</li>
	<li>Berry</li>
	<li>Bogolmolny</li>
	<li>Smilansky</li>
</ul>
</li>
	<li>Nonlinear dynamics - thermodynamic formalism
<ul>
	<li>Ruelle</li>
	<li>Arnold</li>
	<li>Sinai</li>
	<li>Eckmann</li>
	<li>Cvitanovic - chaosbook.org</li>
</ul>
</li>
	<li>Wave transport - statistical methods in vibro-acoustics
<ul>
	<li>Lyon - SEA (1967 paper)</li>
	<li>Langley - WIA</li>
	<li>Heron</li>
	<li>Weaver - diffusion equation</li>
	<li>Le Bot - radiative transformation</li>
</ul>
</li>
</ul>
Linear wave equation. WKB ansatz. Hamiltoninan equations for the amplitude and phase. Characteristics of JH; nonlinear ODE; Liouville equation (linear).

Linear wave –&gt; WKB –&gt; HJ equation –&gt; Liouville Equation
<h2 id="thinkofpolygonalbilliardsnotnecessarilyconvex.">Think of polygonal billiards, not necessarily convex.</h2>
We want to understand the influence of a source (transfmitting at frequency $\omega$) at one location on the wave amplitude at another point. He writes this as a green’s function $G(r, r_0, \omega)$.

Small wavelength limit, so low frequency waves.

Write things as sums over all paths.

Perron-Frobenius operator…

<img src="http://www.redorbit.com/modules/imglib/download.php?Url=/modules/news/upload/9058010d5358bdaf0e4e98600432eee8.jpg" alt="Tandem Satellite images of coastline of Madagascar" />

I started wondering about connections between these ideas and quantum ergodicity…

<img src="http://www.aimath.org/news/que/typicalstadium.gif" alt="Typical Wave Function in a stadium Billiard" />

<img src="http://www.aimath.org/news/que/stadium_scarring.jpeg" alt="Bouncing Ball Modes" />

<strong>Postlude:</strong>

I had a nice conversation with Gregor after the break. I learned from him about <a href="http://www.sciencedaily.com/releases/2010/12/101213151415.htm">microlasers</a>. The idea is to build a circular region out of a lasing material. We energize the material somehow with hopes to excite the whispering gallery mode. The laser light propagates near the boundary but can be arranged to exit the medium by raising the curvature at a specific location. These appear to be rather hard to control to create a unidirectional beam. Since the losses take place all along the boundary, there is very little power in the output beam. Some web searching revealed an <a href="http://www.seas.harvard.edu/news-events/news-archive/2010/harvard-scientists-demonstrate-highly-unidirectional-201cwhispering-gallery201d-microlasers">advance made</a> by the Capasso group at Harvard.
<img src="http://www.seas.harvard.edu/news-events/images/Figure-1.jpg" alt="Elliptic Notched Microlaser Cavity Drawing" />
<img src="http://www.seas.harvard.edu/news-events/images/Figure-2.jpg" alt="Elliptic notched microlaser cavity SEM photograph" />.
<img src="http://www.physorg.com/news/2010-12-highly-unidirectional-gallery-microlasers.html#" alt="Microlaser Cavity (Artistic Rendition)" />
<img src="http://www.seas.harvard.edu/news-events/images/Figure-3.jpg" alt="Schematic Image" />
<img src="http://www.seas.harvard.edu/news-events/images/Figure-4.jpg" alt="Artistic Rendering" />

<hr />

<h1 id="daviddritschelst.andrews:clamthecombinedlagrangianadvectionmethodhttp:www.sciencedirect.comscience_obmimg_imagekeyb6why-4yt6df3-1-28_cdi6863_user809099_piis0021999110001671_originsearch_coverdate072f202f2010_sk997709985viewcwchpdglzvzz-zskwbmd596705cc5acc103e36f154c4de6cec75eiesdarticle.pdf">David Dritschel (St. Andrews): CLAM, The <a href="http://www.sciencedirect.com/science?_ob=MImg&amp;_imagekey=B6WHY-4YT6DF3-1-28&amp;_cdi=6863&amp;_user=809099&amp;_pii=S0021999110001671&amp;_origin=search&amp;_coverDate=07%2F20%2F2010&amp;_sk=997709985&amp;view=c&amp;wchp=dGLzVzz-zSkWb&amp;md5=96705cc5acc103e36f154c4de6cec75e&amp;ie=/sdarticle.pdf">Combined Lagrangian Advection Method</a></h1>
(Many many collaborators)

<img src="http://www.nationalgalleries.org/media_collection/6/NG%202233.jpg" alt="Courbet's &quot;The Wave&quot;" />

I’ll be speaking a bit about a numerical method. I’ll focus mostly on the results we’ve obtained to understand the large scale atmospheres, like Jupiter and perhaps also the ocean.

The numerical method (CLAM) emerges from a Lagrangian method from the 50s for studying fluid dynamics. Zabusky then built from these developments to develop new methods in plasmas. We’ve been extending these ideas to treat certain geophysical fluid flows.

The atmosphere and the oceans are extremely complex, turbulent flows. Accurate computer simulation is immensely difficult to achieve. However, much of this difficulty is inherent in the computational methods employed:
<ul>
	<li>None take direct advantage of the natural inherent Lagrangian advection of dynamical, chemical and biological tracers. (Exploit Lagrangian Descriptions.)</li>
	<li>None seek to separate slow vortical (eddying) and fast wave-like motions and use appropriate, optimal numerical methods for each. (Slow <a href="http://en.wikipedia.org/wiki/Rossby_wave">Rossby waves</a> interacting with fast waves <a href="http://en.wikipedia.org/wiki/Inertial_wave">inertial-gravity waves</a>.)</li>
</ul>
We can build the mathematical theory of the separation into the numerical methods and this will lead to better predictions.

Contour Advection (CASL) Dritschel &amp; Ambaum 1997

geostropic and hydrostatic balances are basic features for describing atmospheric wave dynamics.

This talk reminds me somehow of Bourgain’s high/low method for proving low regularity GWP.

The idea is to use the advection of the vorticity to resolve some (especially relevant) sub-grid scales.

<hr />

<h1 id="dugaldduncanhttp:www.ma.hw.ac.ukdugald:ideequation"><a href="http://www.ma.hw.ac.uk/~dugald/">Dugald Duncan</a>: IDE equation</h1>
Overview:
<ul>
	<li>full IDE equation and how it looks like, where it arises</li>
	<li>Linear part of the IDEbehaviour and approximation</li>
	<li>the full problem - behanviour and approximation</li>
	<li>examples</li>
</ul>
$$
u_t = \sigma \int_\Omega J(x-y) [u(y,t) - u(x,t)]dy + f(u) dx ~ \forall x \in \Omega, t&gt;0.
$$
Typically, $f(u) = u - u^3$. This should be contrasted with the Allen-Cahn equation

$$
u_t = \sigma \Delta u + f(u) dx ~ \forall x \in \Omega, t&gt;0.
$$

There are no spatial derivatives. Therefore, there are now boundary conditions. Instead, this is some kind of integral dynamical equation. It is similar to the <a href="http://en.wikipedia.org/wiki/John_W._Cahn">Cahn</a>-Allen equation.

This equation is also related to sandpiles, neurons, phase transitions.

Other variations recently: Rossi, Perez-Llanos, Andreu, Mazon, Toledo et. al. They study a nonlocal version of the $p$-laplacian.

Linear IDE:
<ul>
	<li>Ignore the nonlinear reaction term for now and take $\sigma \geq 0$ and $\Omega \subset {\mathbb{R}}$:
$$  u_t = Lu.$$</li>
	<li>L is a linear operator - partly a convolution:
$$
Lu = \int_\Omega J(x-y) [u(y,t) - u(x,t)]dy = J * u
$$
…ack slide changed….</li>
</ul>
Discontinuities don’t move. The solution collapses to the average value. Ther eis acomparison principle.

Snapshots of linear behavior.

He does a Fourier analysis of the behavior of plane waves. Instead of having an $\omega^2$, we have $$\hat{J} (\omega) - \hat{J} (0) \thicksim \frac{\omega^2}{2} \frac{d^2}{d \omega^2} {\widehat{J}} (\omega).$$

Peter Bates and Paul Fife did some of the earliest analysis on this equation.

<!--#include virtual="${Base_URL}/templates/footer.html" -->