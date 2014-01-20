
<!DOCTYPE html>
<!---MathJax-->
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_HTML">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
        }
    });
</script>
<!---EndMathJax-->
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title></title>
    
    <meta name="author" content="James Colliander">

    <!-- Le HTML5 shim, for IE6-8 support of HTML elements -->
    <!--[if lt IE 9]>
      <script src="http://html5shim.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->

    <!-- Le styles -->
    <link href="/assets/themes/twitter/bootstrap/css/bootstrap.min.css" rel="stylesheet">
    <link href="/assets/themes/twitter/css/style.css?body=1" rel="stylesheet" type="text/css" media="all">

    <!-- Le fav and touch icons -->
  <!-- Update these with your own images
    <link rel="shortcut icon" href="images/favicon.ico">
    <link rel="apple-touch-icon" href="images/apple-touch-icon.png">
    <link rel="apple-touch-icon" sizes="72x72" href="images/apple-touch-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="114x114" href="images/apple-touch-icon-114x114.png">
  -->
  </head>

  <body>

    <div class="navbar">
      <div class="navbar-inner">
        <div class="container">
          <a class="brand" href="/">James Colliander</a>
          <ul class="nav">
            
            
            


  
    
  
    
      
      	
      	<li><a href="/about.html">About</a></li>
      	
      
    
  
    
      
    
  
    
      
      	
      	<li><a href="/blog.html">Pages</a></li>
      	
      
    
  
    
      
      	
      	<li><a href="/courses.html">Courses</a></li>
      	
      
    
  
    
      
    
  
    
      
      	
      	<li><a href="/navigation.html">Navigation</a></li>
      	
      
    
  
    
      
      	
      	<li><a href="/research.html">Research</a></li>
      	
      
    
  
    
      
      	
      	<li><a href="/service.html">Service</a></li>
      	
      
    
  
    
      
    
  
    
      
      	
      	<li><a href="/tags.html">Tags</a></li>
      	
      
    
  
    
      
    
  



          </ul>
        </div>
      </div>
    </div>

    <div class="container">

      <div class="content">
        
<!---MathJax-->
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_HTML">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
        }
    });
</script>
<!---EndMathJax-->
<div class="page-header">
  <h1> <small>Supporting tagline</small></h1>
</div>

<div class="row">
  <div class="span8">
    &nbsp;

(Apologies for typos or misquotations...; please use comments to help me improve the post. --Jim Colliander)

&nbsp;

Princeton Math Colloquium 2012-03-14

Presenter: <a href="http://www.math.uchicago.edu/~cek/">Carlos Kenig</a>, University of Chicago

Title: A case study for critical non-linear dispersive equations: the energy critical wave equation

Abstract: We will discuss recent  work on the energy critical wave equation. The  issues studied are global  existence, scattering, finite time blow-up,  universal profiles at  blow-up and soliton resolution. This is viewed  not as an isolated series  of results, but as a way of approaching many  similar critical  non-linear dispersive equations.

<a rel="attachment wp-att-996" href="http://blog.math.toronto.edu/colliand/2012/03/14/princeton-math-colloquium-soliton-resolution-for-the-radial-energy-critical-focusing-nonlinear-wave-equation/news200713x-rd/"><img class="alignnone size-full wp-image-996" src="http://blog.math.toronto.edu/colliand/files/2012/03/news200713x-rd.png" alt="" width="275" height="223" /></a>
<!-- Processed by MultiMarkdown -->

<!--   Created by James Colliander on 2011-09-04.   Copyright (c) 2011 University of Toronto. All rights reserved.     -->

We hope this is a model case for how nonlinear dispersive wave equations should proceed. This is a model case. Techniques of harmonic analysis have been introduced into the subject. The focus of those studies concentrated on local well-posedness. In the last fifteen years, there has been a new concentration on global-in-time, blowup aspects.
<h2 id="linearwaveequation">Linear wave equation</h2>
We start with a review of the linear wave equation.

$$ (LW) \partial^2_t w - \Delta w = h, data (w_0, w_1).$$

We write the soluton as
$$
w(t) = S(t)(w_0, w_1) (t) + D(h)(t).
$$

Finite speed of propagation. Picture of a cone.

An important estimate in these studies is the Strichartz estimate.
<h2 id="criticalfocusingnlw">Critical focusing NLW</h2>
$$
\partial^2_t u - \Delta u = u^5, data (w_0, w_1).$$

Defocusing has $- u^5$. Reviews scaling and explains criticality.
<h2 id="smalldatatheoryfornlw">Small data theory for NLW</h2>
Small (in $\dot{H}^1 \times L^2$) initial data evolves uniquely into a global-in-time solution which asymptotoically approaches (in same topology) into a linear solution as $ t \rightarrow \pm \infty$. Moreover, for any data, we have short time existence and a maximal time interval of existence.

This problem has an energy which is constant throughout the solution lifetime. Focusing vs. defocusing. There is competition, in the focusing case, between these two terms.

In the defocusing case, work of <strong>Struwe, Grillakis, Shatah-Struwe, Bahouri-Shatah</strong> proves that for any finite energy data, the solution exists globally and scatters. Another factor, Grillakis showed persistence of higher regularity.

In the focusing case, this fails. <strong>Levine 1974</strong> showed that if $E(u_0, u_1) \leq 0$ then the solution can not exist globally in time (in either direction). (This is done by obstruction.)  Recently, <strong>Kreiger-Schlag-Tataru 2009</strong> constructed solutions for which $T_+ &lt; \infty$ but for which the energy norm remains bounded. Also, in the focusing case, the elliptic equation admits a nonnegative solution $W$. This is a solution which is independent of time. This solution satisfies $\Delta u + u^5 = 0$. This solution is called the <em>ground state</em>. The reason for this terminology is that it arises as the optimizer in a Sobolev inequality and is charaterized variationally. This elliptic equation has been studied in connection with the Yanage problem in differential geometry. The formula for $W$ is explicit
$$ W(x) = \frac{1}{(1 + |x|^2/3)^{1/2}}.$$
$W$ is the unique nonnegative solution of the elliptic equation (<strong>Gidas-Ni-Nirenberg 1979</strong>) and the only $\dot{H}^1$ solution (<strong>Pohozaev 1965</strong>). It does not scatter to a linear solution. It is “non-dispersive.” <strong>Donninger-Krieger 2012</strong> have constructed global-ini-time solutions which are bounded in the energy class, are radial, and don’t scatter to either a linear solution or to $W$. There are other objects.
<h2 id="recallacollectionofrecentresults">Recall a collection of recent results</h2>
<strong>Theorem (Kenig-Merle 2008):</strong>
If $E(u) &lt; E(w)$ then:
1. If the gradient is smaller, we have global existence and scattering.
2. If the gradient is bigger, we have breakdown in (both directions of) finite time.
The case of equality is impossible under the hypothesis.

The proof of this result is an application of a general method. We call this a <strong>concentrated compactness rigidity method</strong>. Provides a brief summary of these ideas: small data, variational aspects, critical element extraction, rigidity.

<strong>Theorem (Duyckaerts-Merle 2008):</strong>
There exists $W_-, ~ W_+$ radial which have the same energy as $W$. Then, there are three statements which provide a characterization of the dynamics.

(original statement of DM had an extra hypothesis which is now removed with inputs from
<strong>Duyckaerts-Kenig-Merle 11, Krieger-Nakanishi-Schlag 11</strong>)

Now, we need to go beyond the energy threshold of $W$.
<h2 id="existenceoftypeiiblowupsolutions">Existence of Type II blowup solutions</h2>
These solutions exist for a finite time but their critical norm remains bounded.

<strong>Krieger-Schlag-Tataru 2009</strong>

Describes a singularity formation process along a rescaled $W$ profile plus a continuous remnant.

We next show this is a "universal" phenomena.

<strong>DKM 2009, 2010:</strong>

(Radial) Any Type II blowup (critical norm stays bounded) solution with just a little bit bigger size than $W$. Then the soution looks like a rescaled $W$ plus errors. All type II blowups look like rescaled $W$.

Corresponding nonradial result: Slightly larger (by $\eta_0$) in the $\sup$ sense as above. After a rotation and a translation, we find that the solution looks like a rescaled and translated $W_l$ plus a small error. The rescaling rate is understood. And we have
$$\lim_{t \uparrow 1} \frac{x(t)}{1-t} = l e^1 .$$

So, the possible profiles in the nonradial case are $W$ or its Lorentz transformations.

There also exist explicit solutions which blow up in finite time. These are built with ODE techniques and are independent of $x$. You can then chop them up with finite speed of propagation. These solutions have exploding critical norm. These are called Type I solutions. Conceivably, there are solutions which are Type I along one sequence of times and Type II along a different sequence of times.

<strong>DKM 2011:</strong> $W_+$ turns out to be Type I.
<h2 id="solitonresolutionforradialsolutionsofnlw">Soliton resolution for radial solutions of NLW</h2>
For a long time, there has been a widespread belief in the math physics community that large, global in tie, solutions of dispersive equations, asymptotically in time, they decouple into a sum of finitely many modulated solitons, a free radiation term and a term that goes to zero at infinity. This is a kind of philosophy that guides the research. So far, this has only been proved for the integrable KdV equations. <strong>Eckhaus-Schurr</strong> carried this out using the completely integrable structure. Corresponding results for mKdV can be obtained via the Miura transform. Heuristic arguements for this conjecture, in the case of cubic NLS in 1D, were given by <strong>Ablowitz-Segur 1976</strong> and <strong>Zakharov-Shabat 1971</strong>. These are all subcrticial equations, for which one expects that these decompositions are stable, unlike in critical equations.

For more general equatiosn, so far, results have been found for data close to the soliton, in subcritical nonlinearities due to several authors. <strong>Buslaev-Perelman 1992</strong> NLS, <strong>Soffer-Weisntein 1990, Marterl-Merle 2001</strong> for gKdV) For corresponding results with blowup there are works by <strong>Merle-Raphael, Martel-Merle</strong>. There have also been large solution results for critical equivariant wave maps onto the sphere due to <strong>Christodoulou-Tahvildar-Zadeh, Shatah-T-Z, Struwe</strong>. They sow convergence along some sequence of times converging to the blwup time locally in space to a soliton (harmonic map).

In the finite time blowup case, for the 1d nonlinear wave equation, <strong>Merle-Zaag</strong> have obtained reusults of this kind using a Lyapunov functional tool.

In critical elliptic problems, such as the ones mentioned earlier, in domains excluding a small ball, considering radial solutions, there have been obtained results on decompositions inot "towering bubbles" (the analog of a finite sum of modulated solitons), as the size of the ball goes to zero. <strong>Musso-Pistoia 2006</strong>

The first general results for radial solutions of NLW were for type II solutions and held only for a sequence of times. We now have the full soliton resolution for radial solutions of NLW.

<strong>Theorem:</strong> Let $u$ be radial solution of NLW. Then, one of the following holds true:
<ol>
	<li>Type I blowup.</li>
	<li>Type II blowup with a full decomposition as a finite sum rescaled $W$, with ordered scaling speeds.</li>
	<li>Radiation plus a sum of modulated solitons.</li>
</ol>
Consequence: Any solution which exists globally in time is bounded.

Remark 1: When the existence time is finite, the limit of the norm exists. It is either divergent or it is bounded. There are no mixed asymptotics. We do not yet have solutions which require more than one bump but we expect that they exist. For 1d NLW similar constructions were made by <strong>Cote-Zaag 2011</strong>. See also <strong>Musso-Pistoia 2006</strong>.

Remark 2: Quantifications. Each bump absorbs some energy.

Discussion....no claim of stability. This is not generic.
<h2 id="ideasoftheproofglobalcase">Ideas of the proof (global case)</h2>
The fundamental new ingredient of the proof is the following dispersive property that all radial solutions to NLW (other than 0 and $\pm W$ ) must have: $ \exists ~ R &gt;0,, ~ \eta &gt; 0$ such that for all $ t \geq 0$ or all $ t \leq 0$
$$
\int_{|x| &gt; R + |t|}  |\nabla_{x,t} u (x,t)|^2 dx \geq \eta.
$$

&nbsp;
    <hr>
    <div class="pagination">
      <ul>
      
        <li class="prev disabled"><a>&larr; Previous</a></li>
      
        <li><a href="">Archive</a></li>
      
        <li class="next disabled"><a>Next &rarr;</a>
      
      </ul>
    </div>
    <hr>
    
  </div>
  
  <div class="span4">
    <h4>Published</h4>
    <div class="date"><span>Liquid error: undefined method `strftime' for nil:NilClass</span></div>

  
    <h4>Tags</h4>
    <ul class="tag_box">
    
    


  
     
    	<li><a href="/tags.html#Notes-ref">Notes <span>6</span></a></li>
     
    	<li><a href="/tags.html#USA-ref">USA <span>5</span></a></li>
     
    	<li><a href="/tags.html#Princeton-ref">Princeton <span></span></a></li>
    
  



    </ul>
    
  </div>
</div>


      </div>

<a href="http://www.math.toronto.edu"><img style="position: absolute; top: 0; left: 0; border: 0;" src="http://www.math.toronto.edu/colliand/images/twitterlogo.png" width="120" alt="Department of Mathematics Avatar" /></a> 

      <footer>
        <p>&copy; 2012 James Colliander, <a href="Department of Mathematics">Department of Mathematics</a>, <a href="University of Toronto">University of Toronto</a>. 
        </p>
      </footer>

    </div> <!-- /container -->

    
  </body>
</html>





