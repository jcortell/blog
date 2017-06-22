---
id: 8138
title: 'Spare time fun: protein structure analysis of mutations causing inheritable diseases'
date: 2016-12-01T08:44:09+00:00
author: Jorge Cortell
layout: post
guid: http://blog.cortell.net/?p=8138
permalink: /blog/2016/12/01/spare-time-fun-protein-structure-analysis-of-mutations-causing-inheritable-diseases/
categories:
  - Geek Fun
  - General
  - Hacking
  - "Life's pleasures"
  - Personal
  - Science
  - Technology
  - Why not? Utopia?
---
Most people I know would not consider _protein structure analysis of mutations causing inheritable diseases_ &#8220;spare time fun&#8221;. Then again, most people I know don&#8217;t think I am like most people they know.

This week I&#8217;m a &#8220;single-dad&#8221;, since my wife is traveling. So my spare time right now is almost non existent. Nevertheless, the thought of mutating a Proline into a Glycine at position 22 intrigued me, so I spent a few minutes simulating it. Here is what I found out:<section> 

### Method

The 3D-structure of my protein of interest was obtained from the UniProt database using Reprof. The structural information was obtained from the analysis of PDB: [3NIR](http://pdb.rcsb.org/pdb/explore/explore.do?structureId=3NIR). Annotations were obtained from UniProt entry [CRAM_CRAAB](http://www.uniprot.org/uniprot/CRAM_CRAAB).</section> <section> 

### Amino Acids

I was interested in the mutation of a Proline into a Glycine at position 22.

The figure below shows the schematic structures of the original (left) and the mutant (right) amino acid. The backbone, which is the same for each amino acid, is colored red. The side chain, unique for each amino acid, is colored black.

![](http://www.cmbi.ru.nl/hope/static/images/aa/pro.jpg) mutates into ![](http://www.cmbi.ru.nl/hope/static/images/aa/gly.jpg)

Each amino acid has its own specific size, charge, and hydrophobicity-value. The original wild-type residue and newly introduced mutant residue differ in these properties: the mutant residue is smaller than the wild-type residue, while the wild-type residue is more hydrophobic than the mutant residue.</section> <section> 

### Variants

A mutation to &#8220;S&#8221; was found at this position, which differs from the mutation I was simulating. The effect of this variant is annotated as: In isoform SI.</section> <section> 

### Conservation

The wild-type residue is not conserved at this position. Another residue type was observed more often at this position in other homologous sequences. This means that other homologous proteins exist with that other residue type than with the wild-type residue in my protein sequence, but the other residue type is not similar to my mutant residue. Therefore, the mutation is possibly damaging.</section> <section> 

### Domains

This residue is part of an interpro domain named: Thionin [IPR001010](http://www.ebi.ac.uk/interpro/entry/IPR001010)

The mutated residue is located on the surface of a domain with unknown function. The residue was not found to be in contact with other domains of which the function is known within the used structure. However, contact with other molecules or domains is still possible and might be affected by this mutation.</section> <section> 

### Amino Acid Properties

The wild-type and mutant amino acids differ in size. The mutant residue is smaller than the wild-type residue. This will cause a possible loss of external interactions.

The hydrophobicity of the wild-type and mutant residue differs. The mutation might cause loss of hydrophobic interactions with other molecules on the surface of the protein.</section> <section> 

### Images

![](http://www.cmbi.ru.nl/hope/yasara/0fc26700-bbb3-4a1c-85a9-b6a3b0f5e997/22GLY_overview.png/)Overview of the protein in ribbon-presentation. The protein is coloured by element; α-helix=blue, β-strand = red, turn=green, and random coil=cyan.

![](http://www.cmbi.ru.nl/hope/yasara/0fc26700-bbb3-4a1c-85a9-b6a3b0f5e997/22GLY_overview_grey.png/)

Overview of the protein in ribbon-presentation. The protein is coloured grey, the side chain of the mutated residue is coloured magenta and shown as small balls.

![](http://www.cmbi.ru.nl/hope/yasara/0fc26700-bbb3-4a1c-85a9-b6a3b0f5e997/22GLY_zoom.png/)

Close-up of the mutation. The protein is coloured grey, the side chains of both the wild-type and the mutant residue are shown and coloured green and red respectively.

![](http://www.cmbi.ru.nl/hope/yasara/0fc26700-bbb3-4a1c-85a9-b6a3b0f5e997/22GLY_zoom2.png/)

Close-up of the mutation (seen from a slightly different angle). The protein is coloured grey, the side chains of both the wild-type and the mutant residue are shown and coloured green and red (not show from this angle) respectively.

![](http://www.cmbi.ru.nl/hope/yasara/0fc26700-bbb3-4a1c-85a9-b6a3b0f5e997/22GLY_zoom3.png/)

Close-up of the mutation (seen from a slightly different angle). The protein is coloured grey, the side chains of both the wild-type and the mutant residue are shown and coloured green and red respectively.</section> <section> 

### Movies

![](http://www.cmbi.ru.nl/hope/yasara/6c11cb58-f112-43f9-9f7a-4d907c84c268/22GLY_turning.gif/)Close-up of the mutation. Both the wild-type and mutant side chain are shown in green and red respectively. The rest of the protein is show in grey.

![](http://www.cmbi.ru.nl/hope/yasara/6c11cb58-f112-43f9-9f7a-4d907c84c268/22GLY_morphing.gif/)

Close-up of the mutation, same colours as animation 1. The animation shows alternating the wild-type side chain and the mutant side chain.</section> <section> 

### Citation

Protein structure analysis of mutations causing inheritable diseases. DOI: [10.1186/1471-2105-11-548.](http://dx.doi.org/10.1186/1471-2105-11-548) PubMed: [21059217](http://www.ncbi.nlm.nih.gov/pubmed/21059217)<a href="http://www.cmbi.ru.nl/hope/report/583f164001ca360009798abb/" target="_blank">.</a></section>