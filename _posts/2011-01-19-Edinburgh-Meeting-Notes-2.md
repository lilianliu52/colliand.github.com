---
layout: post
category : lessons
tags : [notes, Edinburgh]
comments: false
---
<!-- Processed by MultiMarkdown -->

<!--#include virtual="${Base_URL}/templates/head.html" -->
<!--#include virtual="${Base_URL}/templates/header.html" -->
<h1 class="page-title"><a href="http://www.math.polytechnique.fr/~kuksin/">Sergei Kuksin (École Polytechnique)</a>: Nonlinear Schrödinger Equation</h1>
We consider Hamiltonian PDE. This is of course very interesting. In physics, there is a class of pdes which is also of interest:

Hamiltonian PDE = small damping + small forcing

Why is it so important?
<ol>
	<li>This class contains a very important equation: Navier-Stokes.
$$
\dot{u} + (u\cdot \nabla) u + \nabla p = \epsilon \Delta u + force; ~ \nabla \cdot u = 0.
$$
We are interested in cases $d = 2,3.$ For $d=3$, this problem seems impossible. So, let’s collapse to the 2d case.</li>
	<li>Nonlinear Schrödinger equation with some damping and forcing
$$
\dot{u} + i \Delta u - i |u|^2 u = \epsilon \Delta u + force.
$$
Similarly, we might want to study the PKdV equation
$$
\dot{u} + u_{xxx} + u u_x = \epsilon u_{xx} + force.
$$</li>
</ol>
We are interested in the small viscosity $\epsilon \ll 1$ and $t \rightarrow \infty$ extremes. At least we want to study $t \gtrsim \epsilon^{-1}$.

Two papers on my web page:
<ul>
	<li><a href="http://www.math.polytechnique.fr/~kuksin/rfpdef/kuk_pia.pdf">[SK, AP] 2008, JMPA</a></li>
	<li><a href="http://www.math.polytechnique.fr/~kuksin/rfpdef/eff_eq.pdf">[SK] 2010, GAFA</a></li>
</ul>
We introduce the slow time $\tau = \epsilon t$.
<h2 id="perturbationsoflinearhamiltonianpdes">Perturbations of linear Hamiltonian PDEs</h2>
$$
\frac{\partial u}{\partial \tau} + i \epsilon^{-1} (- \Delta u + V(x)u ) = \Delta u - \gamma_R |u|^{2p}u - i \gamma_I |u|^{2q} u + (random force).
$$
Both of the parameters $\gamma &gt; 0$ and satisfy $\gamma_R^2 + \gamma_I^2 =1$. The parameters $p,q$ are natural numbers, possibly 0. WE weill look at the case $d=1$ on $x \in [0,\pi]$ with Dirichlet boundary conditions.

Some more information about the random force,
$$
(random force) = \frac{d}{d\tau} \sum_{j=1}^\infty b_j \beta_j (\tau) e_j (x)
$$
Here the $\beta_j$  are complex valued standard, independent random variables.

We will work in the Sobolev space $H^2$.

<strong>Theorem 1:</strong> If $u_0 \in H^1$ then $\exists ~! ~ u^\epsilon (\tau, x)$ such that
$$
E ( \|u\|<em>1^2 + \int</em>0^\tau \| u(s)\|_2^2 ds) &lt; \infty.
$$

Let $u_0^\omega \in H^1$ be a random.
<ul>
	<li>Let $\mathcal{P}(u_0^\omega) = \mu$ denote the measure in H^1</li>
	<li>Calculate $u^\omega (\tau)$.</li>
</ul>
<strong>Definition:</strong> A measure $\mu$ is called a stationary measure if $\forall ~ \tau$ we have $\mathcal{P} (\mu_\tau ) = \mu.$

<strong>Bogolyubov-Krylov:</strong> A stationary measure <em>almost always</em> exists.

<strong>Theorem 2 (Hairer, Odasso, AS):</strong> If $b_j \neq 0 ~ \forall ~j$ then $\exists ~ !$ stationary measure $\mu^\epsilon.$ For any solution $u(\tau)$, we have
$$
\mbox{dist} (\mathcal{P}(u(\tau)), \mu^\epsilon) \rightarrow 0 ~\mbox{as}~ \tau \rightarrow 0.
$$

The measure $\mu_\epsilon$ depends upon the force but not on the data.
<h2 id="fouriertranform">Fourier Tranform</h2>
For the operator $A = - \Delta + V(x)$ consider the eignefunctions $\phi_1, \phi_2, \dots$ with associated eigenvalues $\lambda_1, \lambda_2, \dots$. Assume that
<ol>
	<li>$\lambda_1 &gt;0$</li>
	<li>$\lambda \cdot s \neq 0 ~ \forall s \in {\mathbb{Z}}^\infty, ~ 0 &lt;|s| &lt; \infty.$</li>
</ol>
For any $u \in H^1$, we can expand $u$ w.r.t. the basis and denote the associated coefficients by $v_1, v_2, \dots$. The <em>Fourier transform</em> is the map $u \longmapsto v$ and the inverse goes the other way.

We can pass from $v_j$  to polar coordinates $I_j, \phi_j$. He recasts the dynamics w.r.t the polar coordinate variables and started speaking about averaging lemmas.
<h2 id="effectiveequations">Effective Equations</h2>
These objects are somehow analogs of the kinetic equations in the theory of weak turbulence….some notation….I want to understand this better….an average of the nonlinear potential energy term. This is a semilinear heat equation with a nonlocal heat equation. The term proportional to $\gamma_I$ does not influence the effective equation. This equation <em>really</em> takes complete control when $\epsilon$ is very small.

The advance obtained here uses randomness in the forcing. “I expect that the effective equation is relevant even without the randomness but I don’t know how to prove it.”

<hr />

<h1 id="j.collianderhttp:www.math.toronto.edu:numericalsimulationsofradialsupercriticaldefocusingwaves"><a href="http://www.math.toronto.edu/">J. Colliander</a>: Numerical Simulations of Radial Supercritical Defocusing Waves</h1>
<a href="http://www.math.toronto.edu/colliand/talks/2011_01_Colliander_Edinburgh_Final.pdf">My slides</a>

<hr />

<h1 id="f.bouchetens-lyonhttp:perso.ens-lyon.frfreddy.bouchet:invariantmeasures"><a href="http://perso.ens-lyon.fr/freddy.bouchet/">F. Bouchet (ENS-Lyon)</a>: Invariant measures</h1>
Collaborators:
<ul>
	<li>A. Venaille</li>
	<li>E. Simonnet</li>
	<li>H. Morita</li>
	<li>M. Corvellec</li>
</ul>
Physical phenomena. I am interested in self-organization in turbulent flows. Examples: stripes and spots on Jupiter. Ocean currents. Height differences in ocean surface. Stable jets.

I will mainly speak about the 2d Navier-Stokes equation with random forcing. This is not such a good model for these phenomena. There are others that are quite similar that might be better to describe the phenomena listed above like the quasigeostrophic and shallow water layer models.

Equilibrium will be related to 2D Euler. For 2D, we have the vorticity-stream formulation. Steady solutions to the Euler equation satisfying $\omega = f(\psi)$ or, equivalently, ${\bf{u}} \cdot \nabla \omega = 0,$ play a crucial role in describing the dynamics. Degeneracy: what is the selection mechanism leading to $f$? The main advance is that $f$ can be predicted using equilibrium statistical mechanics ideas.

Outline:
<ol>
	<li>Invariant measures of the 2D Euler equation
<ul>
	<li>Equilibrium stat mech</li>
	<li>applications of equilibrium stat mec</li>
	<li>invariant measures of the 2d euler equation</li>
</ul>
</li>
	<li>Irreversible relaxation of the 2D Euler equations
<ul>
	<li>irreversibility in fluid mechanics</li>
	<li>…..slide switched….ack</li>
</ul>
</li>
	<li>2D stochastic Navier-Stokes equation: non-equilibrium phase transitions</li>
</ol>
Statisitical mechanics for 2d and geopphysical flows.

Statistical equilibrium. very old idea. famous contributions
<ul>
	<li>Onsager 1949</li>
	<li>Joyce-Montgomery 1970</li>
	<li>Caglioti Marhioro plvirenti lions 1990</li>
	<li>Robert-Sommeria 1991</li>
	<li>Miller 1991</li>
	<li>Eyink-Spohn 1994</li>
</ul>
Robert-Sommeria-Miller (RSM) theory:

The most probable vorticity field. We want to measure the number of microscopic fields $\omega$ which correspond to a probabiility $\rho$. The number of such configuarations is quantified by the Boltzmann-Gibbs Entropy. This is the mixing entropy. Microcanonical RSM variational problem. Critical points are startionary flows of the QG model.

Microcanonical measures for Hamiltonian systems:
<ul>
	<li>Hamilton’s equations</li>
	<li>Liouville Theorem</li>
	<li>Define the microcanonical measures which are the natural invariant measures taking into account the constraints in the dynamics.</li>
</ul>
Detailed Liouvilles thEorem for 2D Euler:

Lee 1952, Kraichnan JFM 1975, Robert 2000

We want to take into account the casimirs and the constraints. He describes a limiting process based on galerkin approximations. Mean field behavior? Large deviations? Sanov theorem?

……lots of discussion…..ideas vs. proofs…..nontribvial…what’s going on? Audience is confusing me…speaker seems clear.

Young measures….entropy…

The claim is that the theory he and his collaborators hav developed explains the emergence and stabiltiy of coherent structures like the great spot on Jupiter. Similar statements about ocean structures.

Are microcanonical measures invariant measures for the 2D Euler dynamics? Is the setof invariant Young measures for the 2D Euler dynamics larger than the set of microcanonical measures?

Two conjectures:
<ul>
	<li>Weak perturbations of the 2D Euler equations close to steady states converge to invariant Young measures.</li>
	<li>The 2D Euler equations converge to invariant Young measures.</li>
</ul>
Wave breaking is an irreversible mechanism in fluids that does not require viscosity.

<hr />

<h1 id="sebastianreichhttp:users.math.uni-potsdam.desreich:dataassimilation"><a href="http://users.math.uni-potsdam.de/~sreich/">Sebastian Reich</a>: Data Assimilation</h1>
<h2 id="dataassimilation">Data Assimilation</h2>
Nature              Physical Laws

Measurements        Model
<pre><code>        Data

        Optimal prediction</code></pre>
He drew arrows between these frameworks of understanding and highlights the assembly of processing at the data assimilation level.

Sequential Data Assimilation in a nutshell.

Model + Observations $\longmapsto$ Prediction

Ingredients of Data Assimilation:
<ol>
	<li>Mathematical and numerical model. solutions and their undertainties caused by approximation errors as well as state and parameter undertainties.</li>
	<li>Data/observations with measurements as well as approximation (forward operators) errors –&gt; Inverse problems</li>
	<li>Numerical approximations to the data assimilation problem within a statistical (Bayesian) framework, assessment of the induced predictions and their uncertainties.</li>
</ol>
<h2 id="mathematicalproblemstatement">Mathematical problem statement</h2>
Consider an evolution problem for which the initial state is treated as a random variable with some given probability density function. For simplicity assume finite-d phase space. The uncertainty in the initial conditions will generally lead to unpredictability over long time intervals. Weather prediction is a nice example.

To counterbalance this increase in uncertainty, we collect observations at discrete times subject to some random measurement errors. We wish to find a trajectory that makes optimal use of the available information in terms of initial data, observations and model dynamics. The task of data assimilation is to combine the model, the measurements and then we want to make the optimal prediction.
<h2 id="theoreticalsolution">Theoretical solution</h2>
i) Model dynamics

Lift the dynamics to the level of the Liouville equation on the probability distribution function.

ii) Data assimilation

Assimilate data using Bayes’ theorem
$$\pi (x|y) \thicksim \pi(y|x) X \rho_{pr} (x).
$$

Here $\pi(x|y)$ is the know conditional PDF (likelihood) for observing $y$ given a state $x$. Given an actual measurement, we can correct and proceed.

Under Bayes’ theorem, we always reuce uncertainty.
<h2 id="ensembleprediction...">Ensemble Prediction…</h2>
ack….slides are changing fast.

<strong>Particle filter</strong>. We give better weight to points that are closer to the observed data. If we repeat this a few times, there will be very few particles contributing to the final answer.
<h2 id="assimilationasacontinuousdeformationofprobability:mckean-vlasov">Assimilation as a continuous deformation of probability: McKean-Vlasov</h2>
We can think of Bayes theorem as an optimal transportation problem.

Crisan-Xiong 2010 did something similar in the context of continuous time filter problem.

Otto 2001 for an application in gradient flow dynamics.

We started with an ODE, spoon fed the measurement data to update the dynamics, and encounter a more complicated dynamical description of the system. We encounter a McKean-Vlasov system, a modified Liouville equation, which is closed by an elliptic PDE.

Numerical filter implementations will now rely on appropriate approximations to the lliptic PDE. We use the ensemble of solutions to define an appropriate statistical model and then solve via numerics or by quadrature.

Obvious choices for the numerical version of $\rho$ include a Gaussian PDF parameterized by the ensemble mean and covariance matri (ensemble Kalmna filter) or Gaussian mxture modes.

<hr />

<h1 id="n.faou:2dsubmarines">N. Faou: 2d Submarines</h1>
2D Euler equation on 2-torus….I was a bit tired and did not type notes during this talk.

<hr />

<!--#include virtual="${Base_URL}/templates/footer.html" -->&nbsp;