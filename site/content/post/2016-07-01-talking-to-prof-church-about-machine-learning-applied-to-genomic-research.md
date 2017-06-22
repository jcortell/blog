---
id: 7964
title: Talking to Prof. Church about machine learning applied to genomic research
date: 2016-07-01T12:44:02+00:00
author: Jorge Cortell
layout: post
guid: http://blog.cortell.net/?p=7964
permalink: /blog/2016/07/01/talking-to-prof-church-about-machine-learning-applied-to-genomic-research/
categories:
  - Geek Fun
  - General
  - "Life's pleasures"
  - News
  - Personal
  - Science
  - Technology
  - Technolust
  - Why not? Utopia?
---
During my flight to Boston I read “[Regenesis](http://www.regenesisthebook.com/)”, the interesting genomic science book by Professor George Church, which was a gift from my friend Dr. Raminderpal Singh.

<img class="aligncenter" src="https://c3.staticflickr.com/8/7288/27881551722_868f869297.jpg" alt="George, Raminder and Jorge 2016 Boston" width="500" height="375" />

On Wednesday evening I had a very interesting conversation in Boston with both of them. Neither of them needs an introduction in the genomics world, but for those of you outside the field:

  * Raminder is Vice-president at Eagle Genomics and Advisor at Kanteron Systems. He was previously Genomic Medicine Strategy Lead at IBM, where he was responsible for the Watson Genomics project.
  * George is a bestselling author, Professor of Genetics at Harvard Medical School and Professor of Health Sciences and Technology at Harvard and MIT. His PhD led to the first genome sequence and contributed to nearly all &#8220;next generation&#8221; DNA sequencing methods.

Since George’s lab work revolves around chip-DNA-synthesis, gene editing, stem cell engineering, super-resolution, molecular computing, dark matter and similar subjects, and since he has PhD students from Harvard, MIT, Boston U., and Cambridge, during the conversation I could not resist the opportunity and I asked him about de novo computational discovery of motifs.

It is an idea I had a few weeks ago while sailing from Saint Petersburg to Helsinki: what if we apply machine learning/intelligence (whether Random Forests or Hierarchical Temporal Memory) algorithms, or even better quantum computing, to look for sequence motifs (nucleotide or amino-acid sequence pattern) to help us predict and engineer structural motifs (chain-like biological molecules)? We could begin with those related to binding and folding, which could lead to an exponential advance in the field of information storage and synthetic biology. But that would be only the beginning. The possibilities and implications could be really far fetching. It would overflow the SFLD 😉

In a nutshell (graphical silly example), it would make it much easier to go from this:
  
<img class="aligncenter" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5c/G-quadruplex.svg/400px-G-quadruplex.svg.png" width="400" height="240" />to this:

<img class="aligncenter" src="https://upload.wikimedia.org/wikipedia/commons/a/aa/Telomer-structure.gif" width="400" height="348" />

And not only describe it, but also understand it and facilitate its application in de-novo engineering.

There are already over 100 software programs which try to do this programmatically (MEME, EXTREME, AlignAce, Amadeus, CisModule, FIRE, Gibbs Motif Sampler, PhyloGibbs, SeSiMCMC, ChIPMunk, Weeder, SCOPE, MotifVoter, MProfiler…). Weirauch et al. evaluated many in a 2013 benchmark. But what I am proposing is a lot more powerful, versatile, and quick than anything done before (as far as I know).

He mentioned some of the research work his wife (Harvard Professor Ting Wu, whom I also met in Boston) is currently involved in around Super-resolution imaging for chromatin folding, and evolutionary conservation, and told me “**your idea is really interesting**”.

> Honestly, I usually can care less about what others think of my ideas (I’m a scientist, I value evidence and data, not “beliefs” or “judgements”) but I personally admire and respect his work, and agree with his views, specially on sharing knowledge and human genome editing, so his comment made my day and encouraged me to further pursue that hypothesis… someday. Right now in my spare time I am redesigning a multi-sensors data stream interface for NASA (pro-bono, unrequested&#8230; but that&#8217;s my idea of fun!).