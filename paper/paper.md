---
title: 'BGmisc: An R Package for Behavior Genetics Analysis'
output:
  rmarkdown::html_vignette:
    keep_md: TRUE
tags:
  - R
  - pedigrees
  - behavior genetics
authors:
  - name: S. Mason Garrison
    orcid: 0000-0000-0000-0000
    affiliation: 1
  - name: Michael D. Hunter
    orcid: 0000-0002-3651-6709
    affiliation: 2
  - name: Xuanyu Lyu
    orcid: 0000-0000-0000-0000
    affiliation: 1
  - name: Jonathan D. Trattner
    orcid: 0000-0000-0000-0000
    affiliation: 3  
  - name: S. Alexandra Burt
    orcid: 0000-0000-0000-0000
    affiliation: 4
affiliations:
 - name: University, Place, USA
   index: 1
 - name: University, Place, USA
   index: 2
 - name: University, Place, USA
   index: 3
 - name: University, Place, USA
   index: 4
date: "21 August, 2023"
bibliography: paper.bib
vignette: >
  %\VignetteEncoding{UTF-8}
  %\VignetteIndexEntry{BGmisc: An R Package for Behavior Genetics Analysis}
  %\VignetteEngine{knitr::rmarkdown}
---
<!--Guidance 
JOSS welcomes submissions from broadly diverse research areas. For this reason, we require that authors include in the paper some sentences that explain the software functionality and domain of use to a non-specialist reader. We also require that authors explain the research applications of the software. The paper should be between 250-1000 words. Authors submitting papers significantly longer than 1000 words may be asked to reduce the length of their paper.
Your paper should include:

A list of the authors of the software and their affiliations, using the correct format (see the example below).
A summary describing the high-level functionality and purpose of the software for a diverse, non-specialist audience.
A Statement of need section that clearly illustrates the research purpose of the software and places it in the context of related work.
A list of key references, including to other software addressing related needs. Note that the references should include full names of venues, e.g., journals and conferences, not abbreviations only understood in the context of a specific discipline.
Mention (if applicable) a representative set of past or ongoing research projects using the software and recent scholarly publications enabled by it.
Acknowledgment of any financial support.
-->
# Summary
<!-- > A summary describing the high-level functionality and purpose of the software for a diverse, non-specialist audience. -->

The field of behavior genetics seeks to understand the genetic and environmental influences on individual differences in behavior. As research in this domain has expanded beyond classical twin studies, so has the need for specialized tools to facilitate complex analyses and equally-complex data structures. The BGmisc package addresses this need by offering a suite of functions tailored for modeling pedigrees and complex data structures. 

( need to be more speccific )


# Statement of need
<!-- A Statement of need section that clearly illustrates the research purpose of the software and places it in the context of related work. -->

`BGmisc` is an R package specifically designed for extended family data, such as pedigrees. Unlike tools that focus solely on classic twin studies, BGmisc accommodates the intricate relationships found in extended family structures. It contains a variety of behavior genetic functions and is intended for use by behavior geneticists and others working with large pedigree data. The package models genetic relationships, infers relatedness, simulates pedigrees, and converts pedigrees into various relatedness matrices. [Describe the dependencies and compatibilities here.]

At present, behavior genetic tools exclusively focus on model fitting for standard family structures (e.g., example, example).  ( paragraph on contextualizing the current field )
<!-- A list of key references, including to other software addressing related needs. Note that the references should include full names of venues, e.g., journals and conferences, not abbreviations only understood in the context of a specific discipline.-->

The study of complex family structures, beyond classic twins, necessitates specialized tools. BGmisc meets this need by offering a comprehensive suite of functions designed for these intricate analyses:

- Relatedness Coefficient Calculation: Using path tracing rules first described in [@Wright1922], BGmisc calculates the relatedness coefficient between all pairs of individuals based on mother and father ids.

- Relatedness Inference: The package infers the relatedness between two groups based on the observed total correlation, given  additive genetic  and shared environmental parameters

- Model Identification: BGmisc determines if a variance components model is identified and fits the estimated variance components of a model to covariance data. The technical aspects related to model identification have been described in Hunter et al. [@hunter_analytic_2021].

- Pedigree Conversion: The package converts pedigrees into various relatedness matrices, including additive genetics, mitochondrial, common nuclear, and extended environmental relatedness matrices.

- Pedigree Simulation: BGmisc simulates pedigrees based on parameters like the number of children per couple, generations, sex ratio, and birth rate, allowing for the modeling of intricate family dynamics beyond classic twins.


<!-- Mention (if applicable) a representative set of past or ongoing research projects using the software and recent scholarly publications enabled by it.-->
These features collectively enable researchers and practitioners to conduct more nuanced analyses of genetic relationships, facilitating the exploration of the multifaceted genetic relationships that shape human behavior. It was developed as part of a grant and has been used in several projects (e.g., [provide examples]) and theses (cite Xuanyu).



# Availability

The BGmisc package is open-source and available on both GitHub at https://github.com/R-Computing-Lab/BGmisc and the Comprehensive R Archive Network (CRAN)  at https://cran.r-project.org/package=BGmisc. It is licensed under the GNU General Public License


# Acknowledgements

The current research is supported by the National Institute on Aging (NIA), RF1-AG073189. We would like to acknowledge assistance from Carlos Santos.


# References