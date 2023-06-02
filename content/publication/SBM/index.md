---
title: "Reassessing the modularity of gene co-expression networks using the Stochastic Block Model"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:

- admin
- Luisa F. Pallares
- Julien F. Ayroles

date: "2023-05-31T00:00:00Z"
doi: "10.1101/2023.05.31.542906"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-05-31T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: bioRxiv

abstract: "Finding communities in gene co-expression networks is a common first step toward extracting biological insight from such complex datasets. Most community detection algorithms expect genes to be organized into assortative modules, that is, groups of genes that are more associated with each other than with genes in other groups. While it is reasonable to expect that these modules exist, using methods that assume they exist a priori is risky, as it guarantees that alternative organizations of gene interactions will be ignored. Here, we ask: can we find meaningful communities without imposing a modular organization on gene co-expression networks, and how modular are these communities? For this, we use of a recently developed community detection method, the weighted degree corrected stochastic block model (SBM), that does not assume that assortative modules exist. Instead, the SBM attempts to efficiently use all information contained in the co-expression graph to separate the genes into hierarchically organized blocks of genes. Using RNA-seq gene expression data measured in two tissues derived from an outbred population of _Drosophila melanogaster_, we show that (a) the SBM is able to find ten times as many groups as competing methods, that (b) several of those gene groups are not modular, and that (c) the functional enrichment for non-modular groups is as strong as for modular communities. These results show that the transcriptome is structured in more complex ways than traditionally thought and that we should revisit the long-standing assumption that modularity is the main driver of the structuring of gene co-expression networks."

tags: [drosophila, gene expression, SBM, modularity, gene co-expression]

# Display this page in the Featured widget?
featured: true

url_pdf: 'publication/SBM/SBM_2023-05-31.pdf'
url_code: 'https://github.com/ayroles-lab/SBM-tools'
url_dataset: 'https://drosophilaeqtl.org'
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

---