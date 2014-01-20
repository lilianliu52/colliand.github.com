---
layout: post
category : lessons
tags : [notes, Edinburgh, Energy Critical, NLS]
---


Last week, I had a chance to visit Edinburgh in part to serve as the external examiner on the PhD Thesis (<a href="http://arxiv.org/find/math/1/au:+Candy_T/0/1/0/all/0/1">papers</a>) of <a href="http://www.maths.ed.ac.uk/people/show?person=163">Tim Candy</a>. Tim is now Dr. Timothy Candy and has an exciting research program to develop as a postdoc at Imperial.

It turned out I had lucky timing since my visit overlapped with a visit by <a href="http://www.math.u-psud.fr/~pocovnicu/">Oana Pocovnicu</a>. I had a chance to hear her speak about her <a href="http://arxiv.org/abs/1112.1354">recent work on the Gross-Pitaevskii equation</a>. I took some notes during Oana’s talk and they appear below.

<img src="http://www.math.u-psud.fr/~pocovnicu/Poza_Aug_2011.jpg" alt="Oana Pocovnicu" />

(joint work with <a href="http://www.math.ucla.edu/~killip/">Rowan Killip</a>, <a href="https://web.math.princeton.edu/~hirooh/">Tadahiro Oh</a>, and <a href="http://www.math.ucla.edu/~visan/">Monica Visan</a>)

Edinburgh talk. 2012-05-21
<ul>
	<li>Dynamics becomes more interesting with a nonvanishing condition at infinity.</li>
	<li>This is the so-called energy critical case.</li>
</ul>
<strong>GP</strong>

$$
i \partial_t u + \Delta u = (|u|^2 - 1)u, u(0) = u_0
$$

The modulus will tend to 1 as $ |x| \rightarrow 1$.

<strong>Literature</strong>
<ul>
	<li>$R$
<ul>
	<li>Zhidkov 1987: introduced Zhidkov spaces.</li>
	<li>Gall 2004. gGWP in $X^1 (R)$</li>
</ul>
</li>
	<li>$R^2, R^3$
<ul>
	<li>Bethuel-Saut 1999 in $1+ H^1$.</li>
	<li>Gourbet 2007</li>
	<li>Gallo 2008</li>
	<li>Gerard 2006 in the energy space.</li>
</ul>
</li>
	<li>$R^4$
<ul>
	<li>Gerard 2006, small energy data such that $\nabla u \in L^2_t L^4_x.$</li>
</ul>
</li>
</ul>
Remark: energy critical in $R^4$.
<ul>
	<li>Gerard 2006 considered the energy space:</li>
</ul>
$$ E_{GP} = [ u = \alpha + v: |\alpha | =1, v \in \dot{H}^1, |v|^2 + 2 \Re (\overline{\alpha}v) \in L^2 (R^d)].
$$

Finite energy data do not have winding at spatial infinity. Therefore, to treat the finite energy case, it suffices to reduce the study to the setting where $u = 1 + v$ and $v$ satisfies…. She reduces the study to finite energy data so the set up excludes vortices right away.

<strong>Theorem (K-O-P-V):</strong>
GP is GWP in the energy space $E_{GP} (R^4)$.

Two ingredients:
<ul>
	<li>GWP of energy-critical defocusing NLS on $R^4$.</li>
	<li>Perturbation theory: We will treat the equation as a perturbation off the cubic NLS.</li>
</ul>
<strong>Scaling Invariance</strong>
<ul>
	<li>Dilation invariance of solutions for cubic NLS is described.</li>
	<li>Dependence of $\dot{H}^s$ in terms of the scaling parameter $\lambda$.</li>
	<li>critical, subcritical, supercritical.</li>
	<li>Cubic NLS on $R^4$ is critical in $\dot{H}^1$. Quintic NLS on $R^3$ is also critical in $\dot{H}^1$.</li>
</ul>
<strong>Strichartz Estimates</strong>
<ul>
	<li>Dispersive decay estimate</li>
	<li>Strichartz Norm; supremum over the admissible pairs.</li>
	<li>$N(I \times R^d)$ is the dual space of the Strichartz space $S(I\times R^d)$.</li>
	<li>Homogeneous Strichartz estimate</li>
	<li>Inhomogeneous Strichartz estimate</li>
	<li>Admissible pairs on $R^4: (\infty, 2), (2,4), (6, \frac{12}{5})$.</li>
	<li>By Sobolev embedding, we have some nice Strichartz containments.</li>
</ul>
<strong>Energy Critical NLS</strong>
<ul>
	<li>LWP. Cazenave-Weissler 1989</li>
	<li>GWP for small data. She then describes this by passing through Strichartz and identifies:
<ul>
	<li>If $\| \nabla e^{it \Delta } w_0 \|{L^6_t L^{12/5}_x}$ is small, we can close the argument.</li>
	<li>The smallness of this expression can be insured by shrinking $T$, but this depends upon the profile properties not just upon the norm of the data.</li>
	<li>GWP for small data follows.</li>
</ul>
</li>
	<li>Explains the blowup critereon showing that the spacetime $L^6$ norm controls the GWP+Scattering theory.</li>
</ul>
<strong>Main Results on defocusing energy-critical NLS</strong>
<ul>
	<li>Bourgain 1999: GWP + Scattering, quintic NLS on $R^3$ with radial data.
<ul>
	<li>induction on energy</li>
	<li>localized Morawetz estimate</li>
</ul>
</li>
	<li>Grillakis 2000: global regularity for quintic NLS on $R^3$ with radial data.</li>
	<li>CKSTT 2003: removed the radial assumption on $R^3$.</li>
	<li>Ryckman-Visan 2007: GWP and scattering for cubic NLS on $R^4$.</li>
	<li>Visan 2010: Simpler method for GWP+Scattering for cubic NLS on $R^4$, building on work of Dodson.</li>
	<li>Kenig-Merle 2006: <em>focusing</em> energy-critical NLS on $R^3, R^4, R^4, R^5$. GWP+ Scattering for radial data with energy and kinetic energy smaller than those of the stationary solution.</li>
</ul>
<strong>Goal: prove existence of a global solution with control on the spacetime $L^6$.</strong>
<ul>
	<li>Contradiction strategy.</li>
	<li>Minimal blowup solution must exist.</li>
	<li>Minimal blowup solutions mut be almost periodic. They are localized in physical and Fourier space.</li>
	<li>Frequency localized Morawetz inequality. (only true for the minimal blowup solution). This is obtained by localizing in frequency the interaction Morawetz estimate.</li>
	<li>This show that we have a smallness property on the spacetime $L^3$ norm on the high frequencies.</li>
	<li>With some interpolation, we can then prove that the spacetime $L^6$ is bounded, contradicting the hypothesis.</li>
</ul>
<strong>Cubic NLS on $R^4$ (Visan)</strong>

(Original proof due to Ryckman-Visan but Visan recently simplified that following some ideas of Dodson.)
<ul>
	<li>By contradiction and using concentration-compactness we have a minimal blowup solution.</li>
	<li>There are only two scenarios. Rapid frequency cascade scenario; quasi-soliton scenario.</li>
</ul>
These are excluded using the long-time Strichartz estimates in the spirit of Dodson. The quasisoliton case is excluded using Morawetz.

<strong>Perturbation theory</strong>

Recalls the perturbation lemma from CKSTT, adapted to this problem.

She nicely describes the reduction to proving a local result on a time interval controlled by the energy. Once we have this type of local theory, we essentially convert the critical problem into one that behaves like the subcritical problem so GWP will follow.

<strong>Remarks on Proof</strong>

Subcritical quadratic terms in the Duhamel-Strichartz analysis on local intervals have a time factor. If this time factor is small enough, these subcritical terms can be absorbed. Oh, now I understand! The point here is that GP can be viewed as the energy-critical NLS plus some quadratic terms which don’t destroy energy conservation. This perspective guides the KOPV analysis. They show that the GP equation can be treated as a perturbation off the dilation invariant energy critical case.

<strong>Cubic-Quintic NLS with non-vanishing BC on $R^3$</strong>

They write $u=1+v$ and observe that $v$ satisfies energy critical NLS with subcritical lower order terms. The Hamiltonian is not sign definite so does not provide coercive control over the kinetic energy term. This is compensated for by using a lower order term $M(v)$, the $L^2$ norm of the real part of $v$. This quantity is not conserved. They show that it satisfies a Gronwall type estimate and that turns out to suffice.

<strong>Scattering for the GP equation in the case of large data</strong>
<ul>
	<li>GP equation has traveling wave solutions that do NOT scatter.</li>
	<li>Formation of traveling waves require a minimal energy in $R^d, d \geq 3$. Bethuel-Gravejat-Saut 2009, de Laire 2009.</li>
	<li>Solutions with sufficiently small energy scatter. (Gustafson-Nakanish-Tsai 2006)</li>
	<li>Can one prove scattering up to the minimal energy of a traveling wave?</li>
</ul>
Our goal is to fill in the gap. But, this problem does not seem too easy to attack, so we tried to apply these ideas on a simpler problem.

<strong>Killip-Oh-Pocovnicu-Visan</strong>

For a Cubic-Quintic NLS with zero boundary conditions (which has conserved mass and energy and has soliton solutions) the are working to show that if $v_0 \in H^1 (R^3)$ then scattering holds true if the mass is smaller than the mass of any soliton OR if it has positive energy, smaller than the enrgy of any solution.

(Final statement is a work in progress.)
