# Crop Genome Prediction 

[TOC]

### [**Genomic** selection for **crop** improvement](https://dl.sciencesocieties.org/publications/cs/abstracts/49/1/1)

[EL Heffner](https://scholar.google.com/citations?user=wzAvaU0AAAAJ&hl=en&oi=sra), ME Sorrells, [JL Jannink](https://scholar.google.com/citations?user=W2nZvQIAAAAJ&hl=en&oi=sra) - **Crop** Science, 2009 - dl.sciencesocieties.org

```markdown
# key points
- In simulations, the correlation between true breeding value and the genomic estimated breeding value has reached levels of 0.85 even for polygenic low heritability traits.
- Current MAS methods are better suited for manipulating a few major effect genes than many small-effect genes (Dekkers and Hospital, 2002)

# Two primary limitations to MAS are 
(i) the **biparental mapping populations** used in most QTL studies do not readily translate to breeding applications and 
(ii) **statistical methods** used to identify target loci and implement MAS have been inadequate for improving polygenic traits controlled by many loci of small effect.

**solution**: high density markers
? biparental mapping population vs breeding population

# LD based mapping:can be used for dissecting complex traits in breeding populations that already have extensive phenotypic data across locations and years
`avoids the need to develop special mapping populations
`mapping within breeding populations will allow for QTL identification and allelic value estimates that can be directly utilized by MAS without the need for extensive validation
`still have these problems: low heritability, small population sizes, few large-effect QTL, confounding population structure, and arbitrary significance thresholds

# Lande and Thompson (1990) proposed a visionary two-step approach: 
(i) select significant markers from large marker sets, and 
(ii) combine phenotypic information with significant markers in a selection index that would explain a significant proportion of additive genetic variance. 
 
# Genomic selection
a form of MAS that simultaneously estimates all locus, haplotype, or marker effects across the entire genome to calculate genomic estimated breeding values (GEBVs; Meuwissen et al., 2001). 

 
training population: 
	individuals having both phenotypic and genotypic data 
	estimate model parameters
calculate GEBVs for individuals having only genotypic data

# estimated breeding values (EBVs) 
- best linear unbiased prediction (BLUP): based only on phenotypic data of individuals and their realtives(Henderson, 1984)
- data on markers linked to known QTL can also be used for calculation of EBVs (Fernando and Grossman, 1989)

# Genomic selection differs from current MAS strategies
because instead of only using markers that have a predefined significant correlation with a trait, **all markers are used** to estimate breeding values for each genotype.

# LD decay 
- are affected by population characteristics such as evolutionary history, mating system, population size, admixture, recombination rate, and selection effects (Gaut and Long, 2003)
- highly variable among species, populations, and genomic regions
- can be used to determine target marker densities for GS

# qxs: accurate GEBV <- high quality dense markers <- high quality genome

# statistical models
- large number of markers, but limited number of phenotypes =>
- lack of degrees of freedom

# GEBV accuracy
the Pearson correlation between the GEBV and the true breeding value (TBV)

## three models: 
# stepwise regression, 
# ridge regression, and 
# Bayesian estimation.









```



### [**Genomic** selection: **genome**-wide **prediction** in plant improvement](https://www.sciencedirect.com/science/article/pii/S1360138514001411)

ZA Desta, [R Ortiz](https://scholar.google.com/citations?user=cxQ_518AAAAJ&hl=en&oi=sra) - Trends in plant science, 2014 - Elsevier

```markdown
# Table 1. Main features of genome-wide prediction models
parametric regressions
	penalized approaches
		` RR-blup
		` LASSO
		` EN
		` BRR
		` BL 
	Bayesian approach
		` Bayes A, B, C, ...
nonparametric regressions
` RKHS
` Random Forest

# Genomic selection versus other plant breeding methods
- easier than animal
	large pop size
	various mating design
	easy to get pure line hybrids
 
 MAS only uses markers significantly linked to target traits
 
 
 
 `GS techniques established in animal breeding are difficult to apply directly to plant breeding programs
 
 ` GS cannot stand lonely or replace conventional breeding approaches, but instead can be used in integrated breeding programs.
 ` Neither insertion-deletions (InDels) nor gene function are recognized when using GS
 
 
 `As selection cycles increase, the expected losses in diversity from GS are unavoidable [63]. the introduction of new parental lines containing favorable agro-morphological traits in the cycles of selection [54,55] may compensate this drawback of GS. 

` Most prediction accuracy in the validation set does not reflect the actual patterns of LD and population structure in the target species. 

` incorporation of G × E interactions into models
 
```



### [**Genome**-wide **prediction** of highly specific guide RNA spacers for CRISPR–Cas9-mediated **genome** editing in model plants and major **crops**](http://www.cell.com/molecular-plant/abstract/S1674-2052(14)60793-0)

K Xie, [J Zhang](https://scholar.google.com/citations?user=LbvoiHoAAAAJ&hl=en&oi=sra), [Y Yang](https://scholar.google.com/citations?user=Rgvd2Q8AAAAJ&hl=en&oi=sra) - Molecular plant, 2014 - cell.com



### [Integrating environmental covariates and **crop** modeling into the **genomic** selection framework to **predict** genotype by environment interactions](https://link.springer.com/article/10.1007/s00122-013-2231-5)

[N Heslot](https://scholar.google.com/citations?user=LqgWXYwAAAAJ&hl=en&oi=sra), [D Akdemir](https://scholar.google.com/citations?user=O_xha20AAAAJ&hl=en&oi=sra), ME Sorrells… - Theoretical and applied …, 2014 - Springer

```markdown
* a large number of correlated predictors each explaining a small amount of the total variance
* non-linear responses of genotypes to stresses are expected
* QTL G*E

Abbreviations
BLUP
Best linear unbiased predictor
GBLUP
Genomic estimated best linear unbiased predictor
GEBV
Genomic estimated breeding value
G*E
Genotype by environment interactions
GS
Genomic selection
MET
Multi-environment trials
QTL
Quantitative trait locus
Q*E
QTL by environment interaction
SGL
Sparse group lasso
SNP
Single nucleotide polymorphism
TPE
Target population of environments

收费

```





### [**Genomic** and metabolic **prediction** of complex heterotic traits in hybrid maize](https://www.nature.com/articles/ng.1033)

[C Riedelsheimer](https://scholar.google.com/citations?user=ufYZybgAAAAJ&hl=en&oi=sra), A Czedik-Eysenberg, C Grieder… - Nature …, 2012 - nature.com



### [High‐throughput phenotyping and **genomic** selection: The frontiers of **crop** breeding converge](http://onlinelibrary.wiley.com/doi/10.1111/j.1744-7909.2012.01116.x/full)

[L Cabrera‐Bosquet](https://scholar.google.com/citations?user=NDKX1Z4AAAAJ&hl=en&oi=sra), [J Crossa](https://scholar.google.com/citations?user=MsMBKCUAAAAJ&hl=en&oi=sra)… - Journal of integrative …, 2012 - Wiley Online Library



### [Harvesting the promising fruits of **genomics**: applying **genome** sequencing technologies to **crop** breeding](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001883)

[RK Varshney](https://scholar.google.com/citations?user=Kdmxy8EAAAAJ&hl=en&oi=sra), R Terauchi, [SR McCouch](https://scholar.google.com/citations?user=GkvvVp8AAAAJ&hl=en&oi=sra) - PLoS Biology, 2014 - journals.plos.org



### [**Genomic prediction** of breeding values when modeling genotype× environment interaction using pedigree and dense molecular markers](https://dl.sciencesocieties.org/publications/cs/abstracts/52/2/707)

[J Burgueño](https://scholar.google.com/citations?user=aUXx0mMAAAAJ&hl=en&oi=sra), [G de los Campos](https://scholar.google.com/citations?user=fRjGwkwAAAAJ&hl=en&oi=sra), K Weigel… - **Crop** …, 2012 - dl.sciencesocieties.org



### [**Genomics**-based approaches to improve drought tolerance of **crops**](https://www.sciencedirect.com/science/article/pii/S1360138506001580)

[R Tuberosa](https://scholar.google.com/citations?user=8y1pwdYAAAAJ&hl=en&oi=sra), [S Salvi](https://scholar.google.com/citations?user=DtQehy8AAAAJ&hl=en&oi=sra) - Trends in plant science, 2006 - Elsevier



### [Use of **crop** growth models with whole-**genome prediction**: application to a maize multienvironment trial](https://dl.sciencesocieties.org/publications/cs/abstracts/56/5/2141)

M Cooper, [F Technow](https://scholar.google.com/citations?user=X7wBWdoAAAAJ&hl=en&oi=sra), C Messina, C Gho… - **Crop** …, 2016 - dl.sciencesocieties.org



### [Plant breeding with **genomic** selection: gain per unit time and cost](https://dl.sciencesocieties.org/publications/cs/abstracts/50/5/1681)

[EL Heffner](https://scholar.google.com/citations?user=wzAvaU0AAAAJ&hl=en&oi=sra), [AJ Lorenz](https://scholar.google.com/citations?user=oWF6CUEAAAAJ&hl=en&oi=sra), [JL Jannink](https://scholar.google.com/citations?user=W2nZvQIAAAAJ&hl=en&oi=sra)… - **Crop** science, 2010 - dl.sciencesocieties.org



### [**Genomic** selection in plant breeding: a comparison of models](https://dl.sciencesocieties.org/publications/cs/abstracts/52/1/146)

[N Heslot](https://scholar.google.com/citations?user=LqgWXYwAAAAJ&hl=en&oi=sra), HP Yang, ME Sorrells, [JL Jannink](https://scholar.google.com/citations?user=W2nZvQIAAAAJ&hl=en&oi=sra) - **Crop** Science, 2012 - dl.sciencesocieties.org



### [Genomic Prediction Using Prior Quantitative Trait Loci Information Reveals a Large Reservoir of Underutilised Blackleg Resistance in Diverse Canola …](https://dl.sciencesocieties.org/publications/tpg/articles/0/0/170100)

[M Fikere](https://scholar.google.com/citations?user=1XXXhqMAAAAJ&hl=en&oi=sra), DM Barbulescu, MM Malmberg… - The Plant …, 2018 - dl.sciencesocieties.org

```markdown
**Genomic selection** uses a reference population that is genotyped and phenotyped to predict the genetic value for individuals that are only genotyped using genome-wide markers (Meuwissen et al., 2001)

Several studies argue that genomic selection provides better accuracies than might be achieved on the basis of pedigree information alone (Crossa et al., 2010; Jia and Jannink, 2012; Perez-Enciso et al., 2015; Tsai et al., 2015; Vela-Avitua et al., 2015).

# genomic prediction models:
Genomic Best Linear Unbiased Prediction (**GBLUP**) (Nejati-Javaremi et al., 1997; Habier et al., 2007; VanRaden, 2008), 
Ridge Regression Best Linear Unbiased Prediction (**RR-BLUP**), 
Bayes A and B (Meuwissen et al., 2001),
BayesR (Erbe et al., 2012).

# Method
Phenotyping:
 - weather data
 - randomized block design
 - Pheno: survival rate, infection values
 - BLUEs using ASReml
 	- Pheno = mean + fixed lines + random row + random column + residue
 	- result: H2 (broad-sense heritability), h2 (genomic heritability)
 	
 Genotyping
 - call SNP,filtering,samtools
 - imputation
 
 LD plink
 
 Heritability, Phenotypic and Genetic Correlations
 - Restricted Maximum Likelihood (REML) in ASReml 
 
 Manhattan plot of marker effects estimated for survival rate and average internal infection using BayesR (BR) and BayesRC (BRC).
 
 Cross Validation and Genomic Prediction Scenarios
 
```







































