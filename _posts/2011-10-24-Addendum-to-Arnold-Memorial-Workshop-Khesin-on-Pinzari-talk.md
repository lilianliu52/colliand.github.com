---
layout: post
author: James Colliander
published: true
tags : [Notes]
---

<!-- -->

&nbsp;

The following message is a guest post by <a href="http://www.math.toronto.edu/khesin/"> Boris Khesin</a>. Boris summarizes the wonderful talk given by Gabriella Pinzari at the workshop.  --Jim Colliander

<a href="http://en.wikipedia.org/wiki/File:Ecliptic_plane_3d_view.gif"><img class="alignleft size-full wp-image-529" src="http://blog.math.toronto.edu/colliand/files/2011/10/Ecliptic_plane_3d_view.gif" alt="" width="249" height="248" /></a>

Gabriella Pinzari (30min talk)  described her joint result with her advisor <a href="http://www.mat.uniroma3.it/users/chierchia/WWW/english_version.html">Luigi Chierchia</a> on a recently found fix for the famous KAM theorem, or rather for its application to the stability of the Solar system.

Namely, the original KAM theorem in<a href="http://iopscience.iop.org/0036-0279/18/6/R02"> Arnold's 1963 paper</a> claimed the persistence of the Liouville tori for perturbations of integrable systems under some nondegeneracy assumption - some determinant must be nonzero. This was a perfectly correct statement proved in the paper. But Arnold applied it to the Solar system without properly checking that for that system the determinant is indeed nonzero. (More precisely, Arnold checked the non-degeneracy condition for the first nontrivial case, the planar three-body problem, and claimed that this could extend to the general case: spatial, arbitrary $n$.) However, it turned out to be identically zero in the spatial case.

So later <a href="http://en.wikipedia.org/wiki/Michael_Herman_%28mathematician%29">M.Herman </a>developed a theory for how to deal with such a degeneracy in the KAM theory. Essentially  it shows how to use a slighter nondegeneracy "in the next term", which worked for the application to the Solar system. (It was published by J.Fejoz.)

But now Gabriella Pinzari explained that the source of the degeneracy in the application of the KAM theorem to the Solar system was the necessity to mod out rotations!! Once one mods out rotational symmetry in the Laplace plane, the system becomes nondegenerate (i.e. Arnold's determinant is nondegenerate) on the quotient! This is somewhat similar to the relation of Morse and Morse-Bott functions, as far as I understand.

Quoting Pinzari, "Arnold gave only some ideas on how to construct (by series) such a reduction, but did not develop these ideas.  What we have done was in essence to construct explicitly such a reduction. The miracle is that you can do it without singularities in the transformation (in a sense this is needed to control the convergence of the series that Arnold had in mind)."

[Note that since the determinant is identically zero, no higher order terms are nonzero. So M.Herman introduced a modification of the Hamiltonian which broke the rotation invariance of the modified system  and computed a modified torsion with nondegeneracy in higher orders and this worked for the application to the Solar system.  On the contrary, keeping the rotation invariance  allows one to stay in the nondegenerate setting on the quotient.]

I am really shocked that this unavoidable degeneracy  had such a simple explanation, which came unnoticed for 40 years. So all one needed  was to develop a rotation-invariant version of the KAM theory. (As far I as understand,  an equivariant KAM still does not exist beyond this rotation case.) And Arnold, who developed both KAM and group actions was in the best position to marry these two domains, but somehow it did not happen then!  --Boris Khesin

Here are some references from G.Pinzari:

&nbsp;
<ul>
	<li> <a href="http://www.mat.uniroma3.it/users/chierchia/TESI/PhD_Thesis_GPinzari.pdf">G. Pinzari's PhD thesis</a></li>
	<li> <a href="http://www.mat.uniroma3.it/users/chierchia/REPRINTS/Invent11.pdf">"An article where we put, in the above sense,  the planetary problem in Arnold's
setting and draw some (KAM) consequences on stability of motions."</a></li>
	<li><a href="http://www.mat.uniroma3.it/users/chierchia/REPRINTS/DCDS10.pdf">"Here we reprove Arnold's KAM theory for the planetary problem,
improving estimates of the Kolmogorov set-  trying to overcome
technicalities."</a></li>
	<li> <a href="http://www.mat.uniroma3.it/users/chierchia/REPRINTS/CMDA11.pdf">"Here we revisit Deprit's reduction in the form we need and give a
different proof of symplecticity."</a></li>
	<li> <a href="http://www.mat.uniroma3.it/users/chierchia/PREPRINTS/Chierchia_Pinzari_BNF_10.pdf">"Here we discuss symplectic relations between the two settings:
reduced and unreduced."</a></li>
</ul>
