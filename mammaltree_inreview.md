---
layout: default
title: Mammal Tree (In review)
weight: 5
incognito: true
---

## Inferring the mammal tree: species-level sets of phylogenies for questions in ecology, evolution, and conservation
#### Nathan S. Upham, Jacob A. Esselstyn, and Walter Jetz.
#### Submitted, _PLoS Biology_.

<br />

#### **Abstract**
Rates of speciation and extinction are fundamental to our understanding of evolutionary processes, but inferring these parameters requires reliable phylogenies. To establish a robust evolutionary timescale for all ~6000 species of mammals, we developed credible sets of trees that collectively contain all uncertainty in estimated topology, divergence times, and hence evolutionary rates. Our ‘backbone-and-patch’ approach to tree-building applies a newly assembled 31-gene supermatrix to two levels of analysis: (i) backbone relationships and ages among major lineages, using Bayesian fossil node- or tip-dating; and (ii) species-level phylogenies or ‘patch clades’ corresponding to each representative lineage in the backbone. Species unsampled for DNA are either excluded (‘DNA-only’ trees) or imputed within taxonomic constraints using branch lengths drawn from local birth-death models (‘completed’ trees). Joining rescaled patches to backbones results in species-level trees of extant Mammalia with all branches estimated under the same modeling framework, thereby facilitating rate comparisons among lineages as disparate as marsupials and placentals. We compare our phylogenetic trees to previous estimates of mammal-wide phylogeny and divergence times, finding that (i) node ages are broadly concordant among studies, and (ii) recent (tip-level) rates of speciation are estimated more accurately in our study than in previous ‘supertree’ approaches where branch lengths are collapsed and re-scaled due to polytomies. This study’s credible sets of mammalian phylogenetic history are now available for download at vertlife.org, enabling newly robust investigations of long-standing questions in comparative biology.

<br />

#### **Links to MCC consensus trees of the DNA-only distributions:**   
   **USAGE:** Consensus trees are only meaningful on our DNA-only distributions; completed trees are inappropriate for consensus since they contain taxonomically imputed species that vary in topological position within constraints (genus or family) across the credible set of trees.
      
   **Node-dated exponential (NDexp)** --- 4098 species; backbone estimated with 17 node calibrations 
   - [pdf file](https://www.dropbox.com/s/7kieolqutegm1ds/MamPhy_fullPosterior_BDvr_DNAonly_4098sp_topoFree_NDexp_MCC_v2_PLOTTED.pdf?dl=1){:target="_blank"} (150 inches long)

   **Fossilized birth-death (FBD)** --- 4098 species + 76 fossil tips; backbone topology as in Zhou et al. (2013)
   - [pdf file](https://www.dropbox.com/s/qy02tip03lenfsq/MamPhy_fullPosterior_BDvr_DNAonly_4098sp_topoFree_FBDasZhouEtAl_MCC_v2_PLOTTED.pdf?dl=1){:target="_blank"} (150 inches long)

<br />


#### **Movies of the credible sets of Mammalia trees (sample of 100 trees each of 10,000 total)**   
   **USAGE:** Shown is the phylogenetic uncertainty propagated into each credible set of trees, consisting of both age and topological variation. For the completed tree sets, the location of the 1813 imputed species are shown (i.e., those missing DNA sequences, of 5911 species total).

NDexp             |  FBD
:-------------------------:|:-------------------------:
<img src="http://vertlife.org/data/credibleSet_mamPhy_Completed-NDexp_100trees_all_higherNodeCols_tipLabel_v2_tipSeq.gif" width="300"/>  |  <img src="http://vertlife.org/data/credibleSet_mamPhy_Completed-FBDasZhouEtAl_100trees_all_higherNodeCols_tipLabel_v2_tipSeq.gif" width="300"/> 
:-------------------------:|:-------------------------:
<img src="http://vertlife.org/data/credibleSet_mamPhy_DNA-only-NDexp_100trees_all_higherNodeCols_tipLabel_v2_tipSeq.gif" width="300"/>  |  <img src="http://vertlife.org/data/credibleSet_mamPhy_DNA-only-FBDasZhouEtAl_100trees_all_higherNodeCols_tipLabel_v2_tipSeq.gif" width="300"/> 


<br />

[This subsetter tool](http://vertlife.org/phylosubsets/){:target="_blank"} will publish the full tree distributions, including the Completed trees of 5911 species, along with the article.