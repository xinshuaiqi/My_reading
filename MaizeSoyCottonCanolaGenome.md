[TOC]



# Maize Genome 

https://www.panzea.org/

https://www.maizegdb.org/

https://www.maizegdb.org/genome/assemblies_overview



## B73 Maize Genome V4

Improved maize reference genome with single-molecule technologies

nature 2017

<https://www.nature.com/articles/nature22971?sf88114573=1>

```markdown
52 times better than the previous one: contig length
better  intergenic spaces and centromeres
additional 130 k TEs
110 k transcript from pacbio

# New B73 
65X pacbio 

- 2958 contigs
- N50: 1.2 Mb
- optical      map => 625 scaffolds
- gap      filling  pseudomolecules: + BAC and genetic map => 2.1Gb; 
- - 2522       gaps
- mean       gap length: 27kbp
- optical genome maps using the Irys system

Assembly:

- Celera      Assembler
- Falcon

Polish:

- Quiver  

RefAligner
```

- [LPUQ00000000.1](https://www.ncbi.nlm.nih.gov/genome?LinkName=nuccore_genome&from_uid=1135493037)
- [LPUQ01.5](https://www.ncbi.nlm.nih.gov/Traces/wgs/?val=LPUQ01#contigs) (144 scaffolds)
- [Gramene Zea mays AGPv4]http://ensembl.gramene.org/Zea_mays/Info/Index
- http://ensembl.gramene.org/Zea_mays/Info/Annotation/#assembly

LPUQ01 maize v4 data:

- 1.1 1058 seqs
- 1.4 640 seqs
- 1.5 144 seqs



## MO17 genome

<https://www.maizegdb.org/genome/genome_assembly/Zm-Mo17-REFERENCE-NRGENE-1.0>

Project PI  

Jinsheng Lai

Sequencing method: Illumina

Assembly methods: NRgene(DenovoMagic)



## Maize cultivar BH207 genome

<http://www.plantcell.org/content/28/11/2700>

```markdown
- Stiff Stalk germplasm pool      germplasm pool:B73
- Iodent      germplasm pool :  PH207

2500 genes difference


GDE difference
TE difference

# comparative genome hybridization revealed pervasive copy number variation (CNV) and presence/absence variation (PAV) between two heterotic inbred lines (B73 and Mo17), including an ∼2.6-Mb region on chromosome 6 that was present in B73 and absent in Mo17 (Springer et al., 2009; Beló et al., 2010).

```



## picture of B73 and Mo17

http://www.plantcell.org/content/15/10/2236.short



Maize genome duplication vs Sorghum



## [Close split of sorghum and maize genome progenitors](http://genome.cshlp.org/content/14/10a/1916.short)

Z Swigoňová, J Lai, [J Ma](https://scholar.google.com/citations?user=hGFwT5sAAAAJ&hl=en&oi=sra), [W Ramakrishna](https://scholar.google.com/citations?user=vlg9obIAAAAJ&hl=en&oi=sra)… - Genome …, 2004 - genome.cshlp.org

```sh
# probably the first paper confirmed the duplication event
maize - sorghum divergence :11.9 Ma
maize duplication: >4.8 Ma

The Sorghum bicolor genome and the diversification of grasses
https://www.nature.com/articles/nature07723
```



## Network of maize inbred line

https://genomebiology.biomedcentral.com/articles/10.1186/gb-2013-14-6-r55

https://media.springernature.com/full/springer-static/image/art%3A10.1186%2Fgb-2013-14-6-r55/MediaObjects/13059_2013_3103_Fig6_HTML.jpg



# Pan genome

### [High-resolution genetic mapping of maize pan-genome sequence anchors](https://www.nature.com/articles/ncomms7914)

[F Lu](https://scholar.google.com/citations?user=RbNQWbUAAAAJ&hl=en&oi=sra), [MC Romay](https://scholar.google.com/citations?user=YNokV_4AAAAJ&hl=en&oi=sra), JC Glaubitz, PJ Bradbury… - Nature …, 2015 - nature.com

```markdown
- presence/absence variation (PAV), an extreme form of CNV
- inversion
- translocation

# Between any two maize varieties, about half of the genome is not shared because of the high level of TE activity during maize evolution17,18

# CML247
high disease resistance 





```









# Pan transcriptome

[Maize pan-transcriptome provides novel insights into genome complexity and quantitative trait variation](https://www.biorxiv.org/content/early/2015/07/12/022384)

Minliang Jin, Haijun Liu, Cheng He, Junjie Fu, Yingjie Xiao, Yuebin Wang, Weibo Xie, Guoying Wang, **Jianbing Yan**

bioRxiv 022384; doi: https://doi.org/10.1101/022384



### [A brief review of software tools for pangenomics](https://www.sciencedirect.com/science/article/pii/S167202291500008X)

[J Xiao](https://scholar.google.com/citations?user=TwM2dD8AAAAJ&hl=en&oi=sra), [Z Zhang](https://scholar.google.com/citations?user=-ubyQtsAAAAJ&hl=en&oi=sra), [J Wu](https://scholar.google.com/citations?user=vpzs5O0AAAAJ&hl=en&oi=sra), [J Yu](https://scholar.google.com/citations?user=jkgpS0kAAAAJ&hl=en&oi=sra) - Genomics, proteomics & bioinformatics, 2015 - Elsevier

```markdown
# two most popular tools
- Panseq 
	 Panseq, another online pangenomic tool, is able to determine core and accessory regions of genome assemblies based on MUMmer and BLASTn, as well as to identify SNPs among the core genomic regions. In addition, Panseq also has a locus selector module that selects the most discriminatory loci among the accessory loci or core gene SNPs [17]. Panseq, however, is not able to provide pangenomic profile and functional enrichment analysis that is important for the biologists to filter out functional relevance of the pangenomic elements.
	 
- PGAP: pan genome analysis pipeline
	PGAP is a stand-alone program developed by Zhao et al. in 2012, which contains five functional models [22]. Based on functional gene clustering and analysis, PGAP presents pangenomic profile (partitions of pangenomic elements or gene categories), genetic variation, species evolution, and function enrichment of different strains and isolates of a given pangenome.

# major Functions:

- categorizing orthologous genes, 
- calculating pangenomic profiles, 
- integrating gene annotations, and 
- constructing phylogenies 

# The concept of pangenome 
first proposed in 2005 by Tettelin et al. [1,2], which is defined as the entire genomic repertoire of a given species or phylogenetic clade when multiple species are defined by systematics.  

# 3 groups of gene profile
- core (shared by all genomes), 
- dispensable, and 
- strain- (or isolate-) specific genes

# take home
-  the performance of pangenomic analysis strongly depends on the accuracy of genome assembly and annotation
- orthologous gene identification is a key step in pangenomic analysis
- sampling

```



### [Inside the pan-genome-methods and software overview](http://www.ingentaconnect.com/content/ben/cg/2015/00000016/00000004/art00006)

L Carlos Guimaraes, L Benevides de Jesus… - Current …, 2015 - ingentaconnect.com



### [Insights into the maize pan-genome and pan-transcriptome](http://www.plantcell.org/content/26/1/121.short)

[CN Hirsch](https://scholar.google.com/citations?user=8VTLS9cAAAAJ&hl=en&oi=sra), [JM Foerster](https://scholar.google.com/citations?user=fI2VKB8AAAAJ&hl=en&oi=sra), [JM Johnson](https://scholar.google.com/citations?user=NKLGLsoAAAAJ&hl=en&oi=sra), [RS Sekhon](https://scholar.google.com/citations?user=dZCATBkAAAAJ&hl=en&oi=sra)… - The **Plant** …, 2014 - Am Soc **Plant** Biol

Illumina sequencing



### [Genome diversity in maize](https://www.hindawi.com/journals/jb/2011/104172/abs/)

V Llaca, MA Campbell, S Deschamps - Journal of Botany, 2011 - hindawi.com



### [Whole-genome sequencing of multiple *Arabidopsis thaliana* populations](https://www.nature.com/articles/ng.911)

[J Cao](https://scholar.google.com/citations?user=Rvk1TF4AAAAJ&hl=en&oi=sra), [K Schneeberger](https://scholar.google.com/citations?user=aESuL1AAAAAJ&hl=en&oi=sra), [S Ossowski](https://scholar.google.com/citations?user=imRxrJ4AAAAJ&hl=en&oi=sra), [T Günther](https://scholar.google.com/citations?user=holW0eEAAAAJ&hl=en&oi=sra)… - Nature …, 2011 - nature.com

```markdown
# 80 strains, 8 populations
200-bp insert libraries and generated 10- to 20-fold coverage (average 17) with 42- to 64-bp paired-end reads on the Illumina Genome Analyzer platform

map to reference genome (119Mbp)

# accuracy
1. single-nucleotide polymorphisms (SNPs) and 1- to 20-bp insertions and deletions (hereafter called small indels) in unique regions on the basis of single-read alignments against the 119.2-Mb reference genome
	For 67.3% of reference positions, we had information from at least 75 strains, and for 43.6% we had complete information.
	**94% SNP ** to validate 325 predicted SNPs, We could PCR-amplify 304 sequence variants; dideoxy sequencing revealed that all carried the predicted mutation (Supplementary Table 2). 

2.   **97.5% SV** 40 randomly chosen SV deletions with a predicted size of 22 bp to 14.3 kb, we obtained PCR products for 39, all of which were validated.

3. SNP/SV = 7.2: 1 
	2,684,863 SNPs and 370,258 small indels
4. Number of SV
	at least 174,789, of which 49% were detected in more than one strain

figure2 上面那一段 继续


```



# Soy

### [**Genome** sequence of the palaeopolyploid soybean](https://www.nature.com/articles/nature08670)

[J Schmutz](https://scholar.google.com/citations?user=v4hqKg8AAAAJ&hl=en&oi=sra), [SB Cannon](https://scholar.google.com/citations?user=AH9CA8sAAAAJ&hl=en&oi=sra), [J Schlueter](https://scholar.google.com/citations?user=EjqqFLQAAAAJ&hl=en&oi=sra), [J Ma](https://scholar.google.com/citations?user=hGFwT5sAAAAJ&hl=en&oi=sra), [T Mitros](https://scholar.google.com/citations?user=7naxhDMAAAAJ&hl=en&oi=sra)… - nature, 2010 - nature.com





# Cotton

### [**Genome** sequence of cultivated Upland cotton (*Gossypium* *hirsutum* TM-1) provides insights into **genome evolution**](https://www.nature.com/nbt/journal/v33/n5/abs/nbt.3208.html)

F Li, G Fan, [C Lu](https://scholar.google.com/citations?user=S3MeNKgAAAAJ&hl=en&oi=sra), G Xiao, C Zou, RJ Kohel, Z Ma… - Nature …, 2015 - nature.com



# Canola

### Genome-wide selection footprints and deleterious variations in young Asian allotetraploid rapeseed

NY7

Qiu Jie

https://www.biorxiv.org/content/biorxiv/early/2018/09/09/412551.full.pdf

```markdown
Ningyou7, Aisan rapeseed

Historical introgression 
first historical introgression of B. rapa dramatically broadened the
allelic pool of Asian B. napus, but decreased their deleterious variations

The secondary historical introgression of European rapeseed (canola-quality) has reshaped Asian rapeseed into two groups, accompanied by an increase in genetic load

Intro开始写的模糊，没有清晰的主题


In China,
the local B. rapa oilseed crop had been cultivated for more than a thousand years (Li,
2001), but from the 1950s this crop was extensively replaced by B. napus
“Shengliyoucai” (SL) types, which included a series of cultivars and derived lines that
had been developed following selective breeding (Liu, 2000). Many distinct cultivars
were further derived based on SL with introgression of B. rapa, an approach
frequently adopted to broaden the genetic diversity and improve the local adaptation
of B. napus in Asia (Zhang et al., 2014)

In the 1970s, Asian
rapeseed was further significantly improved by the introgression of European ‘double
low’ alleles which had been discovered in Canada and then re-introduced to European
rapeseed lines, providing low seed glucosinolate and erucic acid. 

# Tapidor 

# Darmor

# ZS11 


```

### [Assembly and comparison of two closely related *Brassica napus* genomes](https://onlinelibrary.wiley.com/doi/abs/10.1111/pbi.12742)

[PE Bayer](https://scholar.google.co.in/citations?user=GOL15xQAAAAJ&hl=en&oi=sra), [B Hurgobin](https://scholar.google.co.in/citations?user=5xBWe1gAAAAJ&hl=en&oi=sra), [AA Golicz](https://scholar.google.co.in/citations?user=KR_W0jIAAAAJ&hl=en&oi=sra)… - Plant biotechnology …, 2017 - Wiley Online Library

Tapidor 

<http://appliedbioinformatics.com.au/index.php/Darmor_Tapidor>



### [The high‐quality genome of *Brassica napus* cultivar 'ZS11' reveals the introgression history in semi‐winter morphotype](https://onlinelibrary.wiley.com/doi/abs/10.1111/tpj.13669)

F Sun, G Fan, Q Hu, Y Zhou, M Guan, C Tong… - The Plant …, 2017 - Wiley Online Library

zs11

#####  xawz3download

http://ocri-genomics.org/Brassia_napus_genome_ZS11/





# Lettuce

http://lgr.genomecenter.ucdavis.edu/

account:xinshuaiqi; monsanto email, pass: regular-

 [Reyes Chin Wo et al. (2017)](https://www.nature.com/articles/ncomms14953) 

