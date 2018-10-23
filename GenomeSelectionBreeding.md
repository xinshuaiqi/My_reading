# 

[TOC]

# Genomic Breeding

### [Next generation breeding](https://www.sciencedirect.com/science/article/pii/S0168945215300169)

D Barabaschi, [A Tondelli](https://scholar.google.com/citations?user=5FXoH-cAAAAJ&hl=en&oi=sra), F Desiderio, A Volante… - **Plant** Science, 2016 - Elsevier

```markdown
* ref genome 
	* genome editing
* dense SNP:
	* haplotype blocks
	* genetic diversity 
	* GWAS + QTL mapping 
	* Genomics selection 
* New bottleneck: high-throughput phenotyping

# array-based genotyping assays with pre-defined SNP panels （old）
TaqMan™ (http://www.appliedbiosystems.com) and competitive allele-specific PCR (KASP™, http://www.lgcgenomics.com) are among the most popular techniques on the market. 

# direct sequencing of the populations of interest, genome wide, unbiased (New)
RAD seq and GBS

# Many valuable genes and alleles are stored in seed bank collections, hidden in cultivars, landraces, mutagenized populations and wild species. 
qxs: create a database of the gene, allele of these seed

Since a single reference genome is not enough to represent the diversity within a species [26], the re-sequencing of different cultivars, landraces and wild accessions assumes an important role to reveal domestication events [27], identify gene diversification and variations [28] and explain heterosis mechanisms


High throughput:
- Genotyping
- Phenotying
- data recording and computational analysis


Collect meta-data
- QIL 
- examples: 
 in rice [30] and wheat (http://wheat-urgi.versailles.inra.fr/Projects/Wheat-Initiative/Wheat-Information-System). 
 - reduce the information redundancy and highlight what is still missing


# GEBVs： genomic estimated breeding value
` MAS: 
use molecular markers that map near or within specific loci with known phenotypic effects

the selection of a relative small set of genes having major phenotypic effects
 
` GS
 exploit all available markers as predictors of breeding value

-- training pop
know geno, pheno, 
accuracy depends on:
 * marker density: inter marker coefficient, r2
 * LD

Basic models:
- linear regression
- blup
- bayesian 

# LD in major crops
Significant LD in outcrossed species extends for 0.1–1.5 kb in maize [63] and 15–20 kb for sorghum [86], while it extends for a considerably greater distances in self-crossed species like rice (from 75 kb in the indica background to 500 kb in temperate japonica), or barley where LD decays across 5–10 cM, representing approximately 20–40 Mb [87]. 


# Genome Editing
careful selected gRNA 

	# Genome editing relies on very accurate genome sequence information for the precise determination of the target site particularly if the target gene is part of a multigene family or if duplications or homeologus copies are present. 
	




# 8. The control of genetic recombination
In species such as barley, wheat or maize, the crossovers occur much more in the distal part of chromosome than in the pericentromeric regions

	# apomixis
	a process producing genetically identical offspring via seed without the intervention of a second parent 
```

![img](https://ars.els-cdn.com/content/image/1-s2.0-S0168945215300169-gr1.jpg)











### [Advances in Integrating Genomics and Bioinformatics in the Plant Breeding Pipeline](http://www.mdpi.com/2077-0472/8/6/75)

[H Hu](https://scholar.google.com/citations?user=8VQAL68AAAAJ&hl=en&oi=sra), [A Scheben](https://scholar.google.com/citations?user=21Fyv1AAAAAJ&hl=en&oi=sra), [D Edwards](https://scholar.google.com/citations?user=AxsOkqYAAAAJ&hl=en&oi=sra) - Agriculture, 2018 - mdpi.com

```markdown
# ref genome

# integrative crop database 
combining annotated genome sequences, gene functions, interaction networks and trait phenotypes

KnetMiner (Knowledge Network Miner) 
 (1) integrating diverse biological data into a knowledge graph, 
 (2) improving the knowledge graph with text-mining of the literature, 
 (3) identifying the link between genes and evidence nodes, 
 (4) applying the evidence-based gene ranking algorithm and visualising the integrated data.
 
# Trait Discovery
- meta analysis of QTL data
but QTL are
* low resolution 
* only the cross of these two parents

- GWAS 
- Forward and reverse genetics
- GS 
- Cis-regulatory elements



# ML in breeding
- phenotype
- genomics

# Genome Editing 
```

![Agriculture 08 00075 g002 550](https://www.mdpi.com/agriculture/agriculture-08-00075/article_deploy/html/images/agriculture-08-00075-g002-550.jpg)









# Genomic Selection

### [Genomic selection methods for crop improvement: Current status and  prospects](https://www.sciencedirect.com/science/article/pii/S2214514118300400) August 2018

https://www.sciencedirect.com/science/article/pii/S2214514118300400

```markdown
# challenges
# GS models usually face the problem that the number of markers is much higher than the number of phenotypic observations.
Degrees of freedom are insufficient to estimate all marker effects at the same time, a problem aggravated by multicollinearity
Solution: 
The GBLUP and Bayesian methods treat the effects of markers as random effects

# estimation of non-additive genetic effects
# combined analysis of multiple traits or multiple environments


With marker and phenotype information from observed populations, genomic selection (GS) can be used to establish associations between markers and phenotypes. It aims to use genome-wide markers to estimate the effects of all loci and thereby predict the genetic values of untested populations, so as to achieve more comprehensive and reliable selection and to accelerate genetic progress in crop breeding. 

marker ~ (QTL) ~ pheno

## METHODS 
# GBLUP and RR-BLUP
* all loci have common variance
* good for large number, small effect QTL 
* reduced dimentions 
* less iteration, more efficient
* accuracy of GBLUP and RR-BLUP often stays nearly constant regardless of the number of QTL

# Bayer
* allow different marker, different effect size, (better than GBLUP)
* capture large-effect QTL and yield better predictive abilities
* Studies have shown that the accuracy of Bayesian methods is slightly higher than that of GBLUP, especially for the scenario of distant relationships between training and testing sets [35,36].
* time-consuming
# LASSO
* a balance between selective shrinkage and computational efficiency

# nonparametric methods
Machine learning: RKHS and RBFNN 
SVM and RF are good at solving classification problems, whereas RKHS is suitable for regression problems.




# History
- selection one trait
- Selection index: multiple traits
- **BLUP** 1970
- 1990 **Marker assisted selection** (Molecular Breeding)。 
	BUT only suitable for traits controled by a small number of traits, NOT success for Quantitative traits
- GWS, upgraded MAS. 
	- GEBV: Genomic estimated breeding value

# Method
Training population: marker, phenotype 
Generate model
Predict unobserved individual: The average yield of the top 100 showed a 16% increase compared with the average yield of all potential hybrids.



# Additive effect only model 
estimate Breeding Value

**epistasis** are associated with specific genotypes and cannot be inherited consistently
**non additive effect** (dominance, epistasis) are often as Random ENV effects, as noise. 
heterosis

incorporating non-additive effects could be very beneficial in some populations 




# Additive + non-additive model 
In SOME population, this method is better
When non-additive effects are significant 



# Multiple traits + multiple ENV
multiple correlated trait: pleiotropy
G X E

# how to get more accurate results
**sample size** 
genetic relationship with model 

**marker density**

Su et al. [76] investigated genomic prediction using medium-density and high-density marker panels. **When marker density increased from 54 K to 777 K, prediction accuracy increased only 0.5–1.0%.** 

In short, with an increase in marker density, the accuracy of GS is not proportional to the cost.

**The length of haplotypes** may also affect accuracy  | **LD**
 If GS is applied for many generations, the effect of the markers does not change but the proportion of the genetic variance explained by them declines, and accuracy may decrease rapidly in subsequent generations after estimation owing to decay of genetic relationships 

genetic architecture of traits: heritability and distribution of causal genes

# genomic + transcriptomic + metabolomic 




```



![Fig. 1](https://ars.els-cdn.com/content/image/1-s2.0-S2214514118300400-gr1.jpg)

![Fig. 2](https://ars.els-cdn.com/content/image/1-s2.0-S2214514118300400-gr2.jpg)





### [Genomic selection in plant breeding: methods, models, and perspectives](https://www.sciencedirect.com/science/article/pii/S136013851730184X)

[J Crossa](https://scholar.google.com/citations?user=MsMBKCUAAAAJ&hl=en&oi=sra), [P Pérez-Rodríguez](https://scholar.google.com/citations?user=6FoMrm4AAAAJ&hl=en&oi=sra), J Cuevas… - Trends in plant …, 2017 - Elsevier



```markdown
The application of GS in plant breeding could be limited by two main factors: (i) genotyping costs; and (ii) unclear guidelines as to where GS can be efficiently applied in a breeding program.

GS focuses on predicting additive effects in early generations of a breeding program (F2:3) to achieve a rapid selection cycle with a short interval 

GP predicts the complete genetic values of individuals considering both additive and nonadditive (dominance and epistasis) effects, thereby estimating the performance (commercial value) of the cultivars. Genetic values of lines are predicted for some environments using an incomplete (sparse) multienvironment testing scheme.



# Accuracy depends on 

1. size and genetic diversity of Training pop
2. heritability of the traits
3. low LD, low accuracy 
4. Accuracy will plateau when increasing Marker #, pop size increase ... 
5. Add ENV into the model 

# When Number of markers (p) is larger than the population size (n):

Solutions to these problems include the use of: (i) penalized regression; (ii) variable selection; and (iii) dimensionality reduction (e.g., principal components)

Recent results for deep machine learning applied to GP can be found

# why plant is difficult than animal GS
In general, early statistical models developed for GP in animal breeding were based on single-environment assessments. However, in plant breeding, G × E interactions are of paramount importance. 

Multienvironment trials for assessing G × E interactions have an important role in plant breeding for selecting high-performing and stable lines across environments. 

qxs: when Env effect is negligible, GBLUP is better. 

```



![Figure 1](https://ars.els-cdn.com/content/image/1-s2.0-S136013851730184X-gr1.jpg)





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



### [High‐throughput phenotyping and **genomic** selection: The frontiers of **crop** breeding converge](http://onlinelibrary.wiley.com/doi/10.1111/j.1744-7909.2012.01116.x/full)

[L Cabrera‐Bosquet](https://scholar.google.com/citations?user=NDKX1Z4AAAAJ&hl=en&oi=sra), [J Crossa](https://scholar.google.com/citations?user=MsMBKCUAAAAJ&hl=en&oi=sra)… - Journal of integrative …, 2012 - Wiley Online Library



### [Genomic** selection for **crop** improvement](https://dl.sciencesocieties.org/publications/cs/abstracts/49/1/1)

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



### [Harvesting the promising fruits of **genomics**: applying **genome** sequencing technologies to **crop** breeding](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001883)

[RK Varshney](https://scholar.google.com/citations?user=Kdmxy8EAAAAJ&hl=en&oi=sra), R Terauchi, [SR McCouch](https://scholar.google.com/citations?user=GkvvVp8AAAAJ&hl=en&oi=sra) - PLoS Biology, 2014 - journals.plos.org



### [**Genomic** and metabolic **prediction** of complex heterotic traits in hybrid maize](https://www.nature.com/articles/ng.1033)

[C Riedelsheimer](https://scholar.google.com/citations?user=ufYZybgAAAAJ&hl=en&oi=sra), A Czedik-Eysenberg, C Grieder… - Nature …, 2012 - nature.com









### [**Genomic prediction** of breeding values when modeling genotype× environment interaction using pedigree and dense molecular markers](https://dl.sciencesocieties.org/publications/cs/abstracts/52/2/707)

[J Burgueño](https://scholar.google.com/citations?user=aUXx0mMAAAAJ&hl=en&oi=sra), [G de los Campos](https://scholar.google.com/citations?user=fRjGwkwAAAAJ&hl=en&oi=sra), K Weigel… - **Crop** …, 2012 - dl.sciencesocieties.org





### [Use of **crop** growth models with whole-**genome prediction**: application to a maize multienvironment trial](https://dl.sciencesocieties.org/publications/cs/abstracts/56/5/2141)

M Cooper, [F Technow](https://scholar.google.com/citations?user=X7wBWdoAAAAJ&hl=en&oi=sra), C Messina, C Gho… - **Crop** …, 2016 - dl.sciencesocieties.org



### [Plant breeding with **genomic** selection: gain per unit time and cost](https://dl.sciencesocieties.org/publications/cs/abstracts/50/5/1681)

[EL Heffner](https://scholar.google.com/citations?user=wzAvaU0AAAAJ&hl=en&oi=sra), [AJ Lorenz](https://scholar.google.com/citations?user=oWF6CUEAAAAJ&hl=en&oi=sra), [JL Jannink](https://scholar.google.com/citations?user=W2nZvQIAAAAJ&hl=en&oi=sra)… - **Crop** science, 2010 - dl.sciencesocieties.org







### [**Genomics**-based approaches to improve drought tolerance of **crops**](https://www.sciencedirect.com/science/article/pii/S1360138506001580)

[R Tuberosa](https://scholar.google.com/citations?user=8y1pwdYAAAAJ&hl=en&oi=sra), [S Salvi](https://scholar.google.com/citations?user=DtQehy8AAAAJ&hl=en&oi=sra) - Trends in plant science, 2006 - Elsevier









# Less useful

### [Plant **breeding** goes microbial](https://www.sciencedirect.com/science/article/pii/S1360138517301115)

Z Wei, [A Jousset](https://scholar.google.com/citations?user=esHy7AUAAAAJ&hl=en&oi=sra) - Trends in plant science, 2017 - Elsevier



### [Speed breeding is a powerful tool to accelerate crop research and breeding](https://www.nature.com/articles/s41477-017-0083-8)

A Watson, [S Ghosh](https://scholar.google.com/citations?user=oUBQGBQAAAAJ&hl=en&oi=sra), MJ Williams, [WS Cuddy](https://scholar.google.com/citations?user=6Y2MkgMAAAAJ&hl=en&oi=sra)… - Nature plants, 2018 - nature.com



### [Genomics-enabled **next**-**generation breeding** approaches for developing system-specific drought tolerant hybrids in maize](https://www.frontiersin.org/articles/10.3389/fpls.2018.00361/abstract)

T Nepolean, J Kaul, [G Mukri](https://scholar.google.com/citations?user=fL0KTdwAAAAJ&hl=en&oi=sra), S Mittal - Frontiers in plant science, 2018 - frontiersin.org



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































