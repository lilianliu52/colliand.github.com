---
layout: post
category : lessons
tags : [Notes, USA, IAS]
comments: false
---
<!-- -->


<a href="http://www.math.ias.edu/">IAS School of Mathematics</a>

<a rel="attachment wp-att-985" href="http://blog.math.toronto.edu/colliand/2012/03/13/ias-workshop-on-symplectic-dynamics-2-tuesday/mathhall/"><img class="alignnone size-medium wp-image-985" src="http://blog.math.toronto.edu/colliand/files/2012/03/mathhall-214x300.jpg" alt="This image taken from IAS web site." width="214" height="300" /></a>

&nbsp;

<a href="http://www.math.ias.edu/wsd2">Workshop web page</a>
<h2 id="tuesday:2012-03-13">Tuesday: 2012-03-13</h2>
<ul>
	<li>9:00 - 10:00    Laszlo Szekelyhidi, University of Leipzig, “The h-principle for the Euler equations”  <a href="https://www.math.ias.edu/files/hofer/szekelyhidiab.pdf">abstract</a></li>
	<li>10:15 - 11:15  Camilo de Lellis, University of Zurich, “The h-principle for the Euler equations Part 2”  <a href="https://www.math.ias.edu/files/hofer/delellisab.pdf">abstract</a></li>
	<li>11:30 - 12:30  Vladimir Sverak, University of Minnesota, “On the long-time dynamics of some infinite-dimensional Hamiltonian systems”  <a href="https://www.math.ias.edu/files/hofer/sverakab.pdf">abstract</a></li>
	<li>2:30 - 3:30       Antoine Choffrut, University of Leipzig, “On the local structure of the set of stationary flows to the 2D incompressible Euler equations”  <a href="https://www.math.ias.edu/files/hofer/choffrutab.pdf">abstract</a></li>
	<li>4:30 - 5:30       Thomas Kappeler, University of Zurich, “Symplectic techniques for integrable PDEs”  <a href="https://www.math.ias.edu/files/hofer/kappelerab.pdf">abstract</a></li>
</ul>
<h1 id="laszloszekelyhidihttp:www.math.uni-leipzig.deszekelyhidiwelcome.html:theh-principlefortheeulerequations"><a href="http://www.math.uni-leipzig.de/~szekelyhidi/Welcome.html">Laszlo Szekelyhidi</a>: <em>The h-principle for the Euler equations</em></h1>
<img src="http://www.math.uni-leipzig.de/~szekelyhidi/Welcome_files/DSC_0175.jpg" alt="Lazlo Szekelyhidi" width="220" height="194" />

(chalk talk; joint work w. Camillo De Lellis)

“What I will speak about has nothing to do with symplectic and nothing to do with dynamics.” Hofer: very good.

Euler

$$\partial_t v + \nabla \cdot (v \otimes v) + \nabla p = 0; \nabla \cdot v = 0.$$

The spatial dimension $n=2,3$, certainly $&gt;1$. We will speak about weak solutions $v \in L^2_{loc} (T^n \times [0,T])$ and we throw all derivatives onto test functions.

Why look at weak solutions? The equations tell you conservation of mass and momentum. The derivation is done from a continuum analysis so this formulation is natural. For $n=3$, another reason is the relationship with turbulence (<strong>K41, O49</strong>). The story starts with <em>anomalous dissiipation</em>. The observation is that if you consider $NS_\nu$ with small $\nu$ then formally, the dissipation rate
$$
\nu \int |\nabla v|^2 dx &gt; \epsilon.
$$
This is observed in experiments as $\nu \rightarrow 0$. If you plot $\log k$ vs. $\log E(k)$ there are three different regimes: a low frequency regime related to the geometry of the domain, an inertial range with slope $-5/3$ and then a rapid dissipation at high frequencies. Bob Kohn once said that a log-log plot always looks linear. ….discussion with Peter and Camillo….”Bob Kohn is not here so let’s leave him alone.”  <strong>K41</strong> looked at ensemble averages and he derived the $-5/3$ scaling law. <strong>O49</strong> was thinking of a single solution. He said that if we beleive in this kind of log-log picture then in the intermediate regime we are far from dissipation so the nonlinear term is responsible for the $-5/3$ decay. Is it possible to see a single solution that displays this type of decay. If you translate this point of view into a regularity statement and look for $ v \in L^\infty_t C^\alpha_x$ then when $\alpha &gt; 1/3$ we have energy conservation and for $\alpha &lt; 1/3$ then you have anomalous dissipation possible. Klainerman: Is this $1/3$ easy to see? Discussion: Yes, it is just scaling, look at Fourier coefficients….

<strong>Eyink, Constantin-E-Titi</strong> solved the $\alpha &gt; 1/3$ part of Onsager’s conjecture. There is basically nothing known in the $\alpha &lt; 1/3$.

Spencer: Uniqueness in that range? Answer: No you need Lipschitz to see uniqueness so there remains a big gap.

Studying weak solutions puts us ina different framework than the study of smooth solutions, long time behavior for 2D,etc. This is a different world.

<strong>Theorem  (Scheffer-Shnirelman):</strong> There exists a nontrivial weak solution with compact support in time.

This solution can be thought of as having initial data zero, then it is not zero and after a while, it is zero again. (This solution is far from regularity $1/3$.)
<h2 id="h-principlegromov">h-principle (Gromov)</h2>
This theorem can be viewed as a statement of the form of the h-principle. This principle should be viewed as a different tpe of statement related to Hadamard ill-posedness.

<strong>Theorem (Nash-Kuiper):</strong> Any strictly short smooth embedding of (compact) $M^n \rightarrow R^{n+1}$ can be uniformly approximated by $c^1$ isometric embeddings.

For a geometer, this is viewed as a completely wrong theorem. It seemingly contradicts the classical rigidity of the 2-sphere. Any isometric embedding of the 2-sphere into $R^3$ is the standard embedding. However, that theorem requires curvature so needs $C^2$.

Berti: What is short? Answer: Distances in the image are shorter than distances in the domain. So, Lipschitz with constant less than 1.

Two conditions: A topological global condition, an embedding. A local condition, isometric.
<ul>
	<li>global: embedding</li>
	<li>local: isometric</li>
</ul>
General statement. If you can satisfy the global constraint, you can twist it satisfy the local statement. Another example is Gromov’s theorem
saying 2 forms can be converted into symplectic forms.

An idea of the proof of this statement (Nash): $M^n \rightarrow R^{n+2}$. This is basically about a single chart so let’s look instead at $\Omega \subset R^n$ and we consider the embedding $\Omega \rightarrow R^{n+2}$. We have
$$
\nabla u^T \nabla u = g
$$
and strictly short means $g - \nabla u^T \nabla u &gt;0$. We can make wrinkles. Wrinkling is written as a spiral
$$\tilde{u} (x) = u(x) + \frac{a(x)}{\lambda} (\sin (\lambda x \cdot \xi) \zeta (x) + \cos (\lambda x \cdot \xi) \eta (x)),$$
where $\zeta, \eta$ are unit normal to $u(\omega)$. This looks like a “telephone cord”. What happens in orthogonal directions? How does this affect the metric? This is something you can calculate:
$$
\nabla \tilde{u}^T \nabla \tilde{u} = \nabla u^T \nabla u + a^2 (x) \zeta \otimes \zeta + O(\frac{1}{\lambda}).
$$
This means I have a lot of freedom to change the metric in a fixed given direction. This allows me to write  $g - \nabla u^T \nabla u $ as a sum of terms $\sum a_j^2 (x) \xi^j \otimes \xi^j.$ It is important here that the $\xi$ does not depend upon $x$. This allows me to achieve a reduction in the difference

$$\| g - \nabla u^T \nabla u \|_0 = O(\frac{1}{\lambda}),$$

$$\| u - \tilde{u} \|_0 =  O(\frac{1}{\lambda}), $$

$$\| u - \tilde{u} \|<em>1 \thicksim \| a \|</em>0 \thicksim \| g - \nabla u^T \nabla u \|_0^{1/2}.$$
<h2 id="lipschitzisometries">Lipschitz isometries</h2>
$\Omega \rightarrow R^n$

<strong>Kirchlein</strong> Baire Category Method.

Consider the space $X = [ u \in Lip (\Omega): \nabla u^T \nabla u \leq Id]$ endowed with the supremum norm. The observation of Kirchlein is that $\nabla \cdot X \rightarrow L^1$ is Baire-1. Consider 1-Libschitz maps converging to the zero function. With this same argument, I can take any function and add corrugations.

Mather: What is Baire-1? Answer: It is a pointwise limit of continuous maps.

A corollary of Baire Category theorem. The points of continuity is dense. Despite the troubles with the corrugation possibility, most maps in this space are points of continuity. The only places where you can’t improve is where the gradient is already maximizing. As a consequence, most maps in this space are isometric.

This is an argument which can be generalized quite a bit and can be applied to the Euler equations.

<strong>Example.</strong> The original system (O). (Tartar-DiPerna ideas)

$$\sum_{i=1}^n A_i \partial_i z = 0, ~in D’$$
$$ z(x) \in K, ~a.e. ~x$$

and we want to move to same relaxed condition (R) but with $z(x) \in K^{\Lambda}$, which he refers to as the convex hull of $K$. The principle is that most (in the sense of Baire Category) solutions of the relaxed setting R are solutions of the original problem O.

Question: What is the set $K^\Lambda$? This is the “wave cone”. Let $z: R^n \rightarrow R^d$ here. $\Lambda = [ \hat{z}: \exists \xi \in S^{n-1} ~s.t.~ \sum_i A_i \xi_i \hat{z} = 0]$. So, these are the directions in which we can oscillate while maintaining the conservation law and keeping the constitutive relations intact. So, that is $\Lambda$ and then the $\Lambda$-convex hull is like this. $z \notin K^\Lambda$ if $\exists ~ f ~ \Lambda$-convex so that $f(z) &gt; 0, f|_K \leq 0$. You can separate. This general point of view was developed by <strong>Tartar, DiPerna</strong>.

Klainerman: what is the “h”? Answer: In this setting “h” stands for homotopy but that is not so present in this discussion. My view of the weak version of the h-principle is that there are a lot of solutions which have less regularity. De Lellis: Gromov woud say that you can take your short map and homotopize it while maintaining that it is an isometry, except at the endpoint.
<h2 id="applicationtoeuler">Application to Euler</h2>
Now, you can write the Euler equations in this form by renaming the nonlinearity as a new variable. He shows how to do this by renaming some variables, interprets the associated $K$ and $K^\Lambda$.

<strong>Theorem (DL-Sz):</strong> Let $\overline{e}$ be a given function on $T^n \times [0,T]$ and let $(\overline{v}, \overline{u}, \overline{q})$ be smooth strict subsolution. Then $\exists ~ v_k \in L^\infty$, a sequence of weak solutions of Euler such that $v_k \rightharpoonup \overline{v}$ in $L^\infty$ and $\frac{|v_k|^2}{2} = \overline{e}$ a.e. $(x,t)$.

This is the “local part” of the h-principle. Given one subsolution, I can construct a solution by adding these waves. More or less, what Scheffer-Shnirelman have done is to take 0 as the subsolution.

….I am very much running out of time….so just to state one more theorem which touches the initial data.

Admissibility. Those weak solutions for which the $L^2$ norm is nonincreasing. Under this type of assumption, you have the weak-strong uniqueness. Any such strong solution is unique within the larger class of weak solutions emerging from the same initial data.

<strong>Theorem:</strong> Let $n=2$. Let $v_0(x)$ be the shear flow (he indicates this graphically wiht an interface and an arrow to the right above and an arrow to left below). $\exists~$ infinitely many admissible weak solutions.

He draws the interface with a thickened interface of some growing-with-time size outside of which we have the share flow.

Among all the selection criteria you might be considering for restoring uniqueness among the weak solutions, you could ask for maximally dissipating, you could choose the shear flow itself. Or you could ask for the one which has the fastest interface thickening. It is not yet clear which is the physically relevant selection critereon.

Questions:

Sverak: If you take a sequence of smooth solutions onverging to your data, is there any relation to your solution? Answer: It depends how it converges. Sverak: The best you can with continuous. Answer: I’m not sure.
<h1 id="camilodelellishttp:user.math.uzh.chdelellis:theh-principlefortheeulerequationspart2"><a href="http://user.math.uzh.ch/delellis/">Camilo de Lellis</a>: <em>The h-principle for the Euler equations Part 2</em></h1>
(continuation of previous talk; chalk talk)

I’ll start by mentioning some related results in the literature.

Survey article: <strong>D-Sz</strong> posted on web in 2011 contains all this literature.
<ul>
	<li><strong>Wiedeman:</strong> Global existence of weak solutions for any $L^2$ initial data in $R^3$. This would have been a fantastic theorem if it had not been too many solutions. This is the global analog of what was outlined before. Kappeler: ARe they adminssible? Answer: No. We are not anywhere near the blowup problem.</li>
	<li><strong>Sz-Wiedemann:</strong> You can approximate any measure-valued solutions (a la DiPerna-Majda) with exact solutions.</li>
	<li><strong>Sz-Wiedemann:</strong> The set of “bad” initial data is $L^2$-dense.</li>
</ul>
These techniques can also be applied to other equations.
<ul>
	<li>Incompressible porous medium equations. Some class of active scalar equations. <strong>Caddoba-Faoco-Grancedo</strong>, <strong>Shydkoy</strong>, <strong>Sz</strong>.</li>
	<li>Compressible Euler. <strong>D-Sz</strong>, <strong>Chiararoli</strong>, <strong>Chiadaroli-D</strong>. (Higher dimensional conservation laws have a striking nonuniqueness, contrast with the entropy conditions in 1d)</li>
</ul>
The fact that there exist $C^1$ isometric embeddings uniformly approximating any short smooth embedding was surprising.

<strong>Theorem (D-Sz 2011):</strong> For any given $e: [0,1] \rightarrow R^+$ smooth. Then there exists a $C^0$ solution of incompressible Euler in $T^3 \times [0,1]$ such that
$$
e(t) = \frac{1}{2} \int \frac{|v|^2}{2} (x,t) dx.
$$

We are moving towards the lower part of the conjecture of Onsager. I can’t claim this is saying anything about turbulence, but it does speak to the issues of dynamics of solutions viewed on Fourier coefficients.

Remark: It seems we can reach some Holder regularity, something explicit like $\frac{1}{500}$.

Shnirelman: Can you say something about modulus of regularity about this solution? Answer: You can work out something. It would be painful to work out. Finding a Holder exponent is achieved through an iteration process.

The process uses smoothness properties of $e(\cdot)$.

….change gears.

<strong>Borisov ‘50:</strong> If $v \in C^{1,\frac{2}{3} + \epsilon}$ is an isometric embedding of a positively curved connected 2d surface in $R^3$ then the image is convex.

This gives you rigidity. This is a local theorem. The global theorem would say that the sphere has an isometric rigidity. Borisov also had an announcement…..never published his proof.

<strong>Borisov (1965—&gt;2004):</strong> h-principle for 2d analytic surfaces in $R^3$ if $u \in C^{0, \frac{1}{13} - \epsilon}$.

<strong>Conti; D-Sz:</strong> Rigidity and h-principle in general dimension (with better exponenets). For 2d the exponent is $\frac{1}{7}$.

He describes a double iteration scheme. He emphasizes that the parameter $\xi_0$ appearing inside the $\sin$ and $\cos$ is independent of $x$.

There are always successive one dimensional layers in any convex integration, in any h-principle appliation. To improve these constructions and obtain the $C^0$ statement we need to replace these constructions by higher dimensional generalizations. This is a direction suggested also by Gromov in his book.

…slowing down on typing….I’m just going to watch this.
<h1 id="vladimirsverakhttp:math.umn.edusverak:onthelong-timedynamicsofsomeinfinite-dimensionalhamiltoniansystems"><a href="http://math.umn.edu/~sverak/">Vladimir Sverak</a>: <em>On the long-time dynamics of some infinite-dimensional Hamiltonian systems</em></h1>
<img src="http://www.math.umn.edu/pacim/faculty%20photo/sverak2.jpg" alt="Vladimir Sverak" />
<h2 id="mainexamples">2 main examples</h2>
<ol>
	<li>$w_t + u \nabla w =0, ~ w = \curl u, \nabla \cdot u = 0, x \in T^2</li>
	<li>$NLS_3 (T^2)$</li>
</ol>
Thanks to Shnirelman, Kuksin, Choffrut, Keel, Polacik (slide changed fast might be incomplete).

Speculative picutre in Fourier space.

There is an interesting possibilty that on the macroscopc scale the dynamics might be simpler than in finite dimensional cases. Why? If you look at the dynamics on the Fourier space, at time $t=0$, we impose some nice initial data and as tiem evolves, some part of the solution moves toward infinite frequency. Everything in this direction is very hard to establish. There are some obstructions to this behavior. For example, KAM and complete integrability block this phenomena. We consider here “generic solutions”. Even though the initial data might be very complicated, we might end up with complexity moving into the high Fourier modes and what remains will be dictated by the conservation laws. This should be contrasted with finite-d systems. If one truncates the PDE in a naive way, we will initially see the same type of picture (motion toward infinite frequencies) and then we will hit the frequency cutoff and there will eventually be a thermalization. The “complexity” has “nowhere to go”.

Let’s look at defocusing $NLS_3$. We have, for this equation, three basic conserved quantities:
<ul>
	<li>Energy</li>
	<li>Momentum</li>
	<li>Mass</li>
</ul>
Variational principal. We can think of the equation as a variatonal principal: minimize E subject to the mass=m and momentum=p constraints. We can compare this situation to 2D Euler. (In 3D there is the possibility that everything goes to infinity.) The $L^2$ norm and momentum provide constraints and the minimization principle gives you some nontrivial solutions even in the linear case.

The most optimisitic scenario for the transfer to high frequencies is that for a generic solution over a long period of time, the solution will spend most of its time (in some weak topology) near this manifold of minimizers of $E$ subject to the constraints given by parameters $p,m$. The natural “phase space” for solutions is $H^1$ and we view the manifold $M(p,m) subset H^1$. Ergodicity.

The variationa principle may be viewed from the statistical mechanics point of view. Consider a finite-d truncation via Dirichlet prjection. If we believe in stat mech in this scenario, we can use the microcanonical ensemble and look at the set of all points in our phase space where our energy lies between $E$ and $E + \delta$. We have a natural volume measure on this space. We can similarly $\delta$-thicken around the momentum and mass level sets. We can then hope that the solution will concentrate onto a measure living on these subspaces. This is provably rigorous in the linear case. In the limit as the truncation parameter goes to infinity, the energy $E$ is “forgotten” while the mass and momentum constraints are “remembered”. Another way to look at it is to follow the rule-of-thumb that the energy is equidistributed across possible states. Our initial energy is finite and we are equidistributing it across more and more states. Therefore, the temperature (energy per state) and the whole solution will weakly converge to zero. So, as $N \rightarrow \infty$, we concentrate on low frequencies consistent with the constraints and the rest of the solution goes to zero temperature.

Comparison with Gibbs measure. (<strong>Lebowitz, Bourgain,…</strong>) In this construction, one exponentiates the Hamiltonian and interprets this as a density with respect to the Wiener measure. For the Gibbs measure, $\langle E \rangle = + \infty$ and $\beta &gt; 0$. These functions live on function spaces with infinite energy. The measure is concentrated on functions with low regularity and infinite energy. Remarkably, the dynamics is still well-defined by the PDE (<strong>Bourgain</strong>).

A rigorous result. NLS defines a dynamical system on the space $(X, w)$, where $X = [ \psi \in H^1, \| \psi \|_{H^1}\leq C]$. Here “w” denotes the weak topology. This is OK because Bourgain has shown well-posedness on $H^s, s&lt;1$ (<strong>Bourgain</strong>).

<strong>Theorem:</strong> The $\Omega$-limit set (wrt the weak topology) contains solutions for which no movement to high frequencies goes to infinity. These are precompact in $H^1$.

These are the “end states” which solutions approach in the weak topology.

<strong>Question:</strong> Does every $\psi \in \Omega_+ (\psi_0)$ have this property?

Heuristics: If $\psi \in \Omega_+ (\psi_0)$ then the high frequency part has already separated.

Interpretation:

The solutions do not quite approach $M(p,m)$. there is probably some escape….ack slide changed.
<h2 id="dincompressibleeuler">2D incompressible Euler</h2>
the situation is quite similar. The difference between 2D Euler and NLS is that, in some sense, 2D Euler is a Poisson system instead of a Hamiltonian system. The system is a Hamiltonian system on symplectic leaves. Formally, 2D Euler should be viewed as a family of Hamiltonian systems and the orbit takes place on the leaf.

Fourier representation. Stream function. Energy. Conserved quantities associated with vorticity transport.

Natural “phase space”…. $L^\infty (T^2)$ with a weak * topology. <strong>Yudovich</strong> has shown the evolution is well-posed in $L^\infty (T^2)$. We have the necessary well-posedness pieces in place. Importantly for us, in this context of developing fine structures in teh flow, we have the stability result: If the data converges weak start then the same is true at later times. this follows from the proof of Yudovich.

Analogy with NLS. He draws a table.
<ul>
	<li>Phase space: $H^1$ ….  $L^\infty$</li>
	<li>Weakly continuous: Momentum, mass …. $ E = \int -\frac{1}{2} \omega.$</li>
	<li>Lower semicontinues: Energy…..  ack slide changed.</li>
</ul>
Fourier picture. Variational principle, related to the notion of “mixing” introduced by <strong>A. Shnirelman</strong>). We minimize the energy subject to the constraints associated to the weakly continuous quantities. This produces a steady state solution (whih depends on $f_0$).

More geometric picture. We know that a good topology is the weak * topology on $L^\infty$. We can therefore study the weak * closure of the orbit.

Example: Data that looks like $\omega_0 = \chi_A - \chi_B.$ Here $B = T^2 \backslash A, ~ |A| = |B|$.

<strong>Onsager 1947</strong>, <strong>Montgomery-Johce, 1970s</strong>, <strong>Miller, Robert 1990s</strong>, <strong>Turkington 1990s</strong>, closely related to <strong>Shnirelman’s</strong> notion of “mixing”.

Looks similar to Ising model, except that the interaction is long-range. “Most-probable” configuration for a given energy $E$? But we specify here the number of configuration cells that have sign +1, and how many have -1. We can then do the usual statistical mechanics calculations.

He draws another analogy diagram.
<ul>
	<li>NLS …. 2D Euler</li>
	<li>$C^N$…..Ising config</li>
	<li>Classical Maxwell Boltzmann microcannical ensemble picture……fermions (generalized) with long range interaction.</li>
</ul>
Full ergodicity seems….ack.

A more geometric picture for Euler (a sketch).

Geometric finite-d approximations inside the $SDiff (T^2)$ viewpoint. Remarkable fact learned from <strong>Khesin</strong> book showing that we have finite-d geometric approximations using $SU(N)$.

Determining the “end states” for Euler.

Calcuating the “entropy” etc., one gets different answers depending upon how one counts.

In Euler on the torus, the temperature is not zero but is instead negative as was observed by Onsager. All these predictions suggest that hte “end states” consist of shear flows.

An example where transfer to high frequencies was proved: Landau damping.

The only situation where this was rigorously proved wiath the Vlasov-Poisson system.
<ul>
	<li>Landau 1946</li>
	<li>Caglioti-Maffei</li>
	<li>Hwang-Velazquez 2008</li>
	<li>Mouhot-Villani 2009</li>
</ul>
Is there an analog of Landau dampoing possible for 2D Euler?
<ol>
	<li>Linear Landau damping: Yes (<strong>Sverak</strong>)</li>
	<li>Nonlinear case: probably yes, but seems more difficult than the Vlasov-Poisson case.</li>
</ol>
Is there an analog for this in the 2d NLS case? This seems more difficult in the NLS case. Transfer to high frequencies for dispersive equations:
<ul>
	<li>2d NLS: “I-team”</li>
	<li>Various model situations: Bourgain,…</li>
</ul>
Questions:
1. Can you formulate a stability statement related to your question about the “end states” in the Schrodinger setting? Answer: I expect there should be stability statements around the energy minimizers subject to mass and momentum constraints.
2. Do you expect corresponding statements for the focusing problem (when you don’t expect blowup)? Yes, but there will be a weak convergence to soliton instead of the “breather” energy minimizers.

In discussion after the talk, Sverak suggested that these minimizers are not localized onto single Fourier modes and instead appear to be some kind of “breather” solution. These objects should have variational stability properties resembling corresponding statements about solitons and built along the motif of Arnold Stability results as appearing in the book by <strong>Khesin</strong>.

T. Oh reported to me that some studies like those suggested in this talk appear in work of <a href="http://arxiv.org/abs/1009.5737">Chatterjee-Kirkpatrick</a>.
<h1 id="antoinechoffruthttp:www.math.uni-bonn.depeoplechoffrut:onthelocalstructureofthesetofstationaryflowstothe2dincompressibleeulerequations"><a href="http://www.math.uni-bonn.de/people/choffrut/">Antoine Choffrut</a>: <em>On the local structure of the set of stationary flows to the 2D incompressible Euler equations</em></h1>
<img src="http://www.mat.uniroma1.it/people/garroni/Choffrut.jpg" alt="Antoine Choffrut" width="326" height="326" />

<a href="http://arxiv.org/abs/1012.2736">arXiv</a>

(chalk talk)

The Euler flow evolves on symplectic leaves. If you start on one of these leaves, then the Euler flow stays on the leaf. The result I want to prevent is the following. Suppose you have a stationary solution on one leaf, then the other stationary solutions are located on a curve that passes through the leaves. There is a 1-1 correspondence between the stationary solutions and the leaves.

This talk will be a bit more elementary than the other talks. Some aspects were forecasted by Preston and Sverak in earlier talks in this workshop.

Consider a (potato shaped) domain $\Omega$. The Euler equation $ \partial_t u + (u \cdot \nabla) u _ \nabla p =0, \nabla \cdot u =0, u \cdot N =0 (\partial \Omega).$

In 2D, we introduce $u = (u^1, u^2)$ and the vorticity $w =\partial_x u^2 - \partial_y u^1$ and we can derive the vorticity equation
$$ \partial_t w + u \cdot \nabla w = 0.$$

How do you recover $u$ from $w$? and vice versa? Introduce, in 2D, the stream function $u = \nabla^\perp \psi$.

$\psi|_{\partial \Omega} =$ locally constant. We have $\Delta \psi = w$.

Kelvin: A curve $c_0$ at time $t =0$ evolves along the flow to a curve $c_t$ at a later time. We obtain that $\int_{\Gamma_i} \frac{\partial \psi}{\partial N} = \gamma_i$. $\Delta \psi = w$ and some  boundary conditions….

I can rewrite the vorticity equation as $\partial_t w + {\psi, w } = 0$ where the bracket is defined as the area of the parelellogram determined by $\nabla w$ and $\nabla \psi$.

Transport interpretation.

Coadjoint orbit.

<strong>Theorem (Choffrut-Sverak; GAFA 2012):</strong> Let $\overline{w}$ be a “non-degenerate” steady state. Then there exists a $C^\infty$-nhbhd $W$ of $\overline{w}$ such that any coadjoint orbit intersecting $W$ contains exactly one steady state in $W$.

The proof is by an inverse function theorem. I need to say how I am going to implement this function theorem. How do I describe my orbits? How do I describe my steady states? I want to show these are in one-to-one correspondence.

….lots of discussion…..smooth dependence….lots of chatter…..speaker needs to be able to describe more.

Characterization of steady states. The transport equation tells me that there is no dependence of $w$ on $t$ so that $w (\eta_t (x)) = w(x)$, $w = F(\psi)$ provided $\nabla \psi \neq 0$. I impose that $\nabla \psi \neq 0$ in $\Omega$ and I assume that $\Omega$ is an annular domain (with exactly one hole). Steady states are exactly parametrized by $F$.

Characterization of coadjoint orbits.

Transport $\implies A(0) = | [x \cdot w (x) &lt; c ]| = |[x: w \circ \zeta (x) &lt; c]|$

Correspondence.
<ul>
	<li>Steady states ………  F</li>
	<li>Orbits …………. A</li>
</ul>
Steady states can be characterized as conditional critical points of
$$
E(w) = \frac{1}{2} \int_\Omega | \nabla \psi |^2
$$ (restricted to an orbit.)

Recall $\Delta \phi = w$.
Calculating the first variation leads us to $\delta E = \int \nabla \psi \cdot \nabla \phi = - \int \psi { \alpha, w} = 0 $ (using a permutation property.) Since this is true for all $\alpha$, we find that ${\psi, w} = 0$. Similar ideas come up in the Arnold stability theorem.

Euler as a geodesic configuration space. Lagrangian least action principle. <strong>Marchioro-Pulvarenti</strong>, <strong>Chemin</strong>.

Clairaut, Noether, Lie group with (left) invariant metric.

That was the Lagrangian formulation on the tangent space. The real action takes place in the cotangent bundle where we have a Hamiltonian formalism.
<h1 id="thomaskappelerhttp:www.math.uzh.chindex.phpprofessurkey1113:symplectictechniquesforintegrablepdes"><a href="http://www.math.uzh.ch/index.php?professur&amp;key1=113">Thomas Kappeler</a>: <em>Symplectic techniques for integrable PDEs</em></h1>
<img src="http://www.math.uzh.ch/fileadmin/math/user/tk/bilder/tk.jpg" alt="Thomas Kappeler" />

(pdf slides)

Aim: Survey of recent results on integraple PDEs obtained by symplectic techniques. The model equation is the $NLS_3^{\pm}(T)$.

Topics:
<ul>
	<li>Phase portrait/ space of orbits; construction of normal coordinates</li>
	<li>Asymptotic properties of solutions</li>
	<li>KAM theorem</li>
</ul>
NLS as a Hamiltonian system.

Phase space: $L^2_C$. Pairs of functions. More generally, a function space.

There is a canonical Poisson bracket

$$ {F,G}(\phi) = -i \int_0^1 \partial_1 F \partial_2 G - \partial_2 F \partial_1 G) \phi dx. $$

Defocusing NLS. Focusing NLS.

Defocusing NLS as an integrable PDE on T. <strong>Grebert-Kappeler-Poschel</strong> “The defocusing NLS equation and its normal form” to appear in EMS.

Focusing NLS as integrable PDE: only few results.
<h2 id="part1.reviewofnffordefocusingnls.">Part 1. Review of NF for defocusing NLS.</h2>
<strong>Theorem (GKP):</strong> There exists a canonical map (closely related to the Fourier transform) which reveals that defocusing NLS may be viewed as a system of infintely many coupled oscillators.

Steps of proof:

Local part. We have to construct these coordinates $x_n (\phi)$ and $y_n (\phi)$. How to build these coordinates?

Global part. We have a global chart.
<h3 id="zakharov-shabatoperatorzs">Zakharov-Shabat operator (ZS)</h3>
<ul>
	<li>Lax pair for NLS</li>
	<li>Periodic spectrum of $L(\phi)$ on [0,2].</li>
</ul>
<strong>Counting Lemma:</strong> He describes the spectrum with a picture on the board. Floquet theory.
<ul>
	<li>characteristic function</li>
	<li>two-sheeted spectral curve</li>
</ul>
<strong>von Neumann-Wigner 1929</strong>

The eigenvalues come in pairs. Asymptotically, they are like $n\pi + l_n^2$.
<h3 id="constructionofactionsangles">Construction of actions/angles</h3>
<ul>
	<li>Choose cycles $a_n$</li>
	<li>Cycles induce (i) actions and (ii) 1-forms.</li>
	<li>1-forms induce angles.</li>
</ul>
<h3 id="birkhoffcoordinates">Birkhoff coordinates</h3>
Euclidean versions of these action angle coordinates.

Important features of construction
<ul>
	<li>same cycles $a_n$ were used to define $I_n$ and the 1-forms $\beta_n$.</li>
	<li>Cycles/1-forms are defined on the spectral curve and not on phase space.</li>
</ul>
<h2 id="part2.normalformforfnls">Part 2. Normal Form for fNLS</h2>
<ul>
	<li>There do not exist global Birkhoff coordinates.</li>
	<li>The associated Zakharov-Shabat operator $L$ is not necessarily self-adjoint.</li>
	<li>Symmetries of $spec_p (L(\phi))$.</li>
	<li>$spec_p (L(\phi))$ can be described.</li>
</ul>
We believe that one can characterize the (local) existence of Birkhoff coordinates near $\phi \iff$ spectral properties of the Zakharov-Shabat operator.
<h3 id="standardpotentials">Standard Potentials</h3>
Describes how to carry out the construction. The focusing case requires local constructions.

The discussion here is very precise and I don’t think I can convey more than is available on the slides.

…
<h2 id="part4.kamfordefocusingnls">Part 4. KAM for defocusing NLS</h2>
<ul>
	<li>Defocusing NLS is integrable on all of $L^2$.</li>
	<li>Question: KAM on $L^2$, not only near equilibrium point 0?</li>
	<li>Defocusing NLS frequencies can be expressed using the Birkhoff coordinates.</li>
</ul>
<strong>Proposition:</strong>
Can check the Kolmogorov and Melnikov conditions and then conclude by analyticity.
<h3 id="nearresonances">Near resonances</h3>
<ul>
	<li>$\omega_j - \omega_{-j} = O(1)$ for $ j \rightarrow \pm \infty$ jeopardizes measure estimate of standard KAM theorem for integrable PDE.</li>
	<li>Ways to overcome difficulties:</li>
	<li><strong>Craig-Wayne-Bourgain</strong> method. <strong>Bourgain, IMRN 95</strong></li>
	<li><strong>Kuksin-Poschel</strong>, <strong>Berti</strong></li>
	<li>Restrict the perturbations <strong>Geng-You CMP 06, JDE 05</strong></li>
</ul>
<strong>Kappeler-Liang JDE 12</strong>

&nbsp;