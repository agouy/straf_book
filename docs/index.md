--- 
title: "The STRAF Book"
author: "Alexandre Gouy and Martin Zieger"
date: "2024-12-03"
site: bookdown::bookdown_site
documentclass: book
output: bookdown::bs4_book
bibliography: references.bib  
link-citations: yes
description: "Online version of the STRAF Book."
---



# Preface {-}

<center><img src="img/cover.png" class="cover" alt="book_cover" width="300"/></center>

## What is this book? {-}

This is the online version of __The STRAF Book__, which is currently under
active development. It is dedicated to the STRAF software, a web application
for the analysis of genetic data in forensic practice.

## Forensic and population genetics, lost sisters {-}

Genetics has many faces, and population and forensic genetics are two of them. 
If we were to briefly summarise their respective scopes, we could say that the 
former aims at understanding genetic differences within and between populations 
and the latter is the application of those findings to legal matters.

Forensic genetics and population genetics have always been tightly linked
disciplines. This is likely because quite a number of questions they address
are similar. Even though problems in forensics and population genetics seem 
different, they often correspond to the same question, simply phrased differently.

In population genetics, a common goal is to characterise the genetic diversity of a set of populations, by looking at how related individuals are within and between populations. DNA profiling used in criminal investigations aims at matching different DNA samples. To be able to evaluate the probative strength of such a match, forensic geneticists need to know how much the members of the relevant population are genetically related to each other. The same applies to the calculation of probabilities for different hypotheses of kinship, e.g. in paternity tests. Both fields aim at __understanding__ and __quantifying__ the __relatedness__ of individuals based on their DNA.

Software and metrics developed in the population genetics for the study of the 
evolution of species are now used routinely in forensic genetics practice. 
But forensics is not just _applied population genetics_. The legal implications
and unique situations encountered in the forensics world also led to the 
development of relevant statistical tools and metrics with a more specific purpose.

## And then there was STRAF {-}

__STRAF__ was born from the encounter of two scientists: a forensic geneticist
and a  population geneticist, in 2017, in the beautiful city of Bern (Switzerland).
Martin came to visit a population genetics lab, where Alexandre was pursuing 
his Ph.D. thesis at that time. This led to a fruitful collaboration 
when they realised that some tools used in population genetics should be 
made more accessible to the forensics community.

The most striking example is the computation of forensics parameters, that describe
for example how good are our loci at discriminating samples. These 
parameters were typically computed using a spreadsheet that had been created by 
one of the suppliers of assays used to genotype samples. It is the mythical 
PowerStats v1.2 spreadsheet, allowing to compute forensic statistics and allele 
frequencies in Microsoft Excel. It has been since then removed from the Internet, 
and forensic geneticists started sharing this spreadsheet among each other, circulating 
almost secretly, "under the cloak" as French speakers would say.

As similar operations were done in routine in population genetics, we already had 
some scripts for the analysis of STR data. Then, after we applied them to an existing 
dataset, we decided to put everything into a web application so that the forensics 
community could benefit from it.

A few weeks later, STRAF was born [@ref_straf], and after four year, STRAF had become a 
widely used tool by the forensics community, but not only. 
It has been used as a support for teaching population genetics, and has 
been used in evolutionary biology studies. 
The positive reception of the software in the community motivated its 
development over the years until the release of STRAF 2.0 in 2021. 

## What will you learn? {-}

By reading this book, our hope is that you will:

* Get a brief overview of common __concepts__ in forensic and population genetics

* Learn how to use the __STRAF software__ for STR data analysis through __practical applications__

* Be able to __interpret__ common metrics and analyses used in forensics practice

## Outline {-}

The book is organised as follows:

* In __Chapter__ \@ref(introduction), we'll start by an __introduction__ to essential forensic and population genetics concepts.

* In __Chapter__ \@ref(importing-data), we will focus on data, from its generation to its preparation for
downstream analysis in STRAF.

* In __Chapter__ \@ref(forensic-parameters), we will review __forensic parameters__ that can be computed in STRAF,
and discuss their interpretation.

* In __Chapter__ \@ref(popgen-indices), we will review essential population genetics concepts and
describe __population genetics indices__ that can be computed in STRAF.

* In __Chapter__ \@ref(pca-mds), we will focus on __multivariate statistics__ and how they can provide 
insights into population structure, with a particular focus on Principal Component
Analysis (PCA) and Multidimensional Scaling (MDS), two widely used approaches in genetics.

* In __Chapter__ \@ref(ref-pop), we will explain how to compare samples of interest to
__reference populations__ by loading reference allele frequencies into the 
software and performing a Multidimensional Scaling analysis.

* In __Chapter__ \@ref(file-conversion), we gather recommendations around potential next analysis steps
by presenting STRAF's __file conversion__ capabilities and useful methods implemented in
__other software__.

* In __Chapter__ \@ref(snp-analysis), we discuss how to analyse Single Nucleotide Polymorphism (SNP)
data using the software.

* Finally, more details about the STRAF software are presented in the Appendix. 
