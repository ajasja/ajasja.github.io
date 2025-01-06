---
title: "Massively parallel measurement of protein–protein interactions by sequencing using MP3-seq"
order: 1 # Sorting order for featured pubs
collection: publications
date: 2024-08-27
venue: 'Nature chemical biology'
authors: 'A Baryshev*, A La Fleur*, B Groves, C Michel, D Baker, A Ljubetič✉, G Seelig✉'
paperurl: # Only if different than doi
doi: 10.1038/s41589-024-01718-x
type: 'Paper'
header:
  teaser: 'https://media.springernature.com/lw685/springer-static/image/art%3A10.1038%2Fs41589-024-01718-x/MediaObjects/41589_2024_1718_Figa_HTML.png?as=webp'
project: 
featured: true # Should the publication be shown under "Featured publications" at the top of page
readMore: true
---

Highlights:
* We measured more than 113,000 protein-protein interactions in a single tube!
* Found large orthogonal sets.
* Found new rules for protein design (at least two mismatches in the hydrogen bond network are required for orthogonality).
* Improved AlphaFold2 for predicting orthogonality of proteins (AF2 is not very sensitive on its own, but can be improved by physics- based Rosetta metrics).

 

Protein-protein interactions (PPIs) are key to biological functions and are used in applications ranging from drug development to synthetic cellular circuits. Designed coiled-coil proteins have been used in a variety of ways to build novel protein structures to regulate human cell function, including potential applications for therapeutics (Ljubetič et al. Nat.Biotech. 2017, Fink et al. Nat.Chem.Biol. 2019, Satler et al. JACS 2023).

However, to develop better protein binders, find larger orthogonal sets and train large AI models, we need more high-quality data.

Therefore, we have developed a yeast complementation system that allows us to measure thousands of protein-protein interactions in a single tube. We have carefully calibrated the system with known controls. To test the limits of the methods, we screened (in a single experiment) a set of 2+2 binders with more than 113,000 interactions! (337x337 asymmetric matrix).

We succeeded in obtaining high-quality data and new orthogonal sets. Next, we addressed a profound question of protein design: "How many hydrogen bond networks mismatches can be tolerated in a heterodimer?" We showed that at least two hydrogen bond mismatches are required for orthogonality and that the designs should be longer than 3.5 heptads. And finally, we wanted to investigate how good AlphaFold2 is at predicting orthogonality. It turned out that AF2 is not very sensitive because it always wants to pair the proteins with each other. However, using the physics-based Rosetta metrics, we could easily train good predictors for each protein family.

We anticipate that our assay will be useful to a wide range of biochemists and scientists involved in protein design.

The research was led by research assistant prof. dr. Ajasja Ljubetič at the Department of Synthetic Biology and Immunology at the National Institute of Chemistry and by prof. dr Georg Seelig at the University of Washington in Seattle.

The results were published in the journal Nature Chemical Biology.

Link to article: https://www.nature.com/articles/s41589-024-01718-x

Contact for further information: ajasja.ljubetic(at)ki.si

