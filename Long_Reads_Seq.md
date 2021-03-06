# Table of Content

[TOC]



# Long Reads Sequencing

### [The impact of third generation genomic technologies on plant genome ...](https://www.sciencedirect.com/science/article/pii/S1369526616301315)

https://www.sciencedirect.com/science/article/pii/S1369526616301315

```markdown
# nice review of bionano, Hi-C and 10Xgenome

```





### [Single-molecule DNA sequencing technologies for future genomics research](https://www.sciencedirect.com/science/article/pii/S0167779908002047)

PK Gupta - Trends in biotechnology, 2008 - Elsevier

### [PacBio Sequencing and Its Applications - ScienceDirect](https://www.sciencedirect.com/science/article/pii/S1672022915001345)

https://www.sciencedirect.com/science/article/pii/S1672022915001345

by A Rhoads - ‎2015 - ‎[Cited by 338](https://scholar.google.com/scholar?newwindow=1&safe=active&rlz=1C1GCEB_enUS796US796&biw=1536&bih=746&um=1&ie=UTF-8&lr&cites=11702491833015593169) - ‎[Related articles](https://scholar.google.com/scholar?newwindow=1&safe=active&rlz=1C1GCEB_enUS796US796&biw=1536&bih=746&um=1&ie=UTF-8&lr&q=related:0ejN1VGaZ6IrBM:scholar.google.com/)

```markdown
# no high throughput
`Pacbio RS II:
35,000-70,000 of the 150,000 ZMW wells 

`Illumina HiSeq 2500 
produces up to 8 billion paired-end 125 bp reads (1 trillion bases) per two flow cells over a 6-day run, resulting in a daily throughput of ∼167 billion bases (using High Output Run Mode)

# error rate
11-15%

# NGS and PacBio sequencing are complementary
using the high-throughput and high-accuracy short read data to correct errors in the long reads

PacBio long reads can provide reliable alignments, scaffolds, and rough detections of genomic variants, while short reads refine the alignments/assemblies/detections to single-nucleotide resolution. 

# Iso-Seq 
up to 10 kbp 

```

### [Evaluation of hybrid and non-hybrid methods for *de novo* assembly of nanopore reads](https://academic.oup.com/bioinformatics/article-abstract/32/17/2582/2450734)

[I Sović](https://scholar.google.com/citations?user=MMnxhpgAAAAJ&hl=en&oi=sra), [K Križanović](https://scholar.google.com/citations?user=y8VMyaIAAAAJ&hl=en&oi=sra), [K Skala](https://scholar.google.com/citations?user=-QRZmOcAAAAJ&hl=en&oi=sra), [M Šikić](https://scholar.google.com/citations?user=EK7apmcAAAAJ&hl=en&oi=sra) - Bioinformatics, 2016 - academic.oup.com

```markdown
# All non-hybrid methods correctly assemble the E. coli genome when coverage is above 40x

# hybrid methods are highly dependent on the quality of NGS data, but much less on the quality and coverage of nanopore data and perform relatively well on lower nanopore coverages.

# ALLPATHS-LG showed overall the best results.
it requires a rather specific set of Illumina paired-end
;and mate-pair short read libraries to perform the assembly

# In case only paired-end reads are available, SPAdes might be a good choice.

`intro`
* de Bruijn graph (DBG)
* Overlap-Layout-Consensus (OLC)
* Celera assembler
	* HGAP, one of the early one, using BLASR
    * PBcR
    * LQS
* Daligner

`result`
# suggest 40X 
```



Scaffolding







# Latest progress

[SALSA 2](https://www.biorxiv.org/content/early/2018/02/07/261149)

```markdown
# Contigs: 
Unambiguous reconstructions of the sequence 
# Scaffolding：
utilizes long-range linking information such as BAC or fosmid clones, optical maps, linked reads,or chromosomal conformation capture to order and orient unitigs. 

# Hi-C
measuring the contact frequency between all pairs of loci in the genome
* provide linkage information
* spanning tens of megabases

# limitations of previous methods
* require chr number
* sensitive to input assembly contiguity and Hi-C library variations
* Inversions are common
* ...

# SALSA2
the first method to leverage assembly graph
information for scaffolding Hi-C data

# Steps:
 Hi-C reads map to contigs: NWA aligner
 find best match
 scaffolding
 mis-join detection, broken
 exhansted correct Hi-C links. 









```





#### [Assessing genome assembly quality using the LTR Assembly Index (LAI)](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gky730/5068908)

[S Ou](https://scholar.google.com/citations?user=u-B7aHYAAAAJ&hl=en&oi=sra), J Chen, N Jiang - Nucleic Acids Research, 2018 - academic.oup.com

```
evaluate the repeat in assembly
LTR assembly index
assembly continuity
independent from genome size, gene space metrics.

LTR 4-20kbp
estimate age of insertion

introa-element recombination is the major process to remove LRT in rice and Ath. 

a more continuous genome assembly would result in more intact LTR elements being
identified. 



```







#### [Selective single molecule sequencing and assembly of a human Y chromosome of African origin](https://www.biorxiv.org/content/early/2018/06/08/342667)

Lukas F.K. Kuderna, Esther Lizano, Eva Julia, Jessica Gomez-Garrido, Aitor Serres-Armero, MartinKuhlwilm, Regina Antoni Alandes, Marina Alvarez-Estape, Tyler Alioto, Marta Gut, Ivo Gut, Mikkel Heide Schierup, Oscar Fornas, Tomas Marques-Bonet

bioRxiv 342667; doi: https://doi.org/10.1101/342667



#### [A chromosome-scale assembly of the sorghum genome using nanopore sequencing and optical mapping](https://www.biorxiv.org/content/early/2018/05/22/327817)

Stephane Deschamps, Yun Zhang, Victor Llaca, Liang Ye, Gregory May, Haining Lin

bioRxiv 327817; doi: https://doi.org/10.1101/327817



#### [Chromosome-scale comparative sequence analysis unravels molecular mechanisms of genome evolution between two wheat cultivars](https://www.biorxiv.org/content/early/2018/02/07/260406)

Anupriya Kaur Thind, Thomas Wicker, Thomas Mueller, Patrick M Ackermann, Burkhard Steuernagel, Brande B.H Wulff, Manuel Spannagl, Sven O Twardziok, Marius Felder, Thomas Lux, Klaus F.X Mayer, International Wheat Genome Sequencing Consortium, Beat Keller, Simon G Krattinger

bioRxiv 260406; doi: https://doi.org/10.1101/260406



#### [Long Read Annotation (LoReAn): automated eukaryotic genome annotation based on long-read cDNA sequencing](https://www.biorxiv.org/content/early/2017/12/08/230359)

David Cook, Jose Espejo Valle-Inclan, Alije Pajoro, Hanna Rovenich, Bart Thomma, Luigi Faino

bioRxiv 230359; doi: https://doi.org/10.1101/230359



#### SALSA

```markdown
# In the data generated by the Hi-C
protocol, the intrachromosomal contact probability is on
average much higher than the interchromosomal contact
probability

# previously
LACHESIS
* cluster contig based on Hi-C mapping
* initial ordering based on the maximum spanning tree
* reinsert rest ccontigs
* BUT need chr number

Kaplan method
* no contig orient

Both methods are slow, no misassembly correction. 

GRAAA:
* single chromosome in human 

# This paper
If both mates in the read pair align to the same chromosome, it
implies an intrachromosomal contact.

use a weight function to normailize the scores of Hi-C links, reduces the length biases inherent in long contigs.  

correct misassemblies. 


```

SALSA2

```markdown
`Integrating Hi-C links with assembly graphs for
`chromosome-scale assembly

#


```



















### [Beyond genomic variation-comparison and functional annotation of three Brassica rapa genomes: a turnip, a rapid cycling and a Chinese cabbage](https://bmcgenomics.biomedcentral.com/articles/10.1186/1471-2164-15-250)

K Lin, N Zhang, [EI Severing](https://scholar.google.com/citations?user=C2fAnUoAAAAJ&hl=en&oi=sra)… - BMC …, 2014 - bmcgenomics.biomedcentral.com



### [Analytical and decision support tools for genomics-assisted breeding](https://www.sciencedirect.com/science/article/pii/S1360138515002770)

RK Varshney, VK Singh, JM Hickey, X Xun… - Trends in **plant** …, 2016 - Elsevier































# Reference publications





[qxs onenote](https://monsanto365-my.sharepoint.com/personal/evrpa_monsanto_com/_layouts/OneNote.aspx?id=%2Fpersonal%2Fevrpa_monsanto_com%2FDocuments%2FXINSHUAI%20%40%20Monsanto&wd=target%28Genomics%20Working%20group%20meeting.one%7C05470CAA-18C0-4D43-99B2-C4C53CCD1112%2FLong%20Reads%20Papers%7CB778F283-E755-476C-849C-A040F6E98E9F%2F%29)

##### [*Piercing the dark matter: bioinformatics of  long-range sequencing and mapping**](https://www.nature.com/articles/s41576-018-0003-4?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%3A+nrg%2Frss%2Fcurrent+%28Nature+Reviews+Genetics+-+Issue%29)

```markdown
Note:
	• High quality:
		○ Contiguity
		○ Completeness
		○ Correctness
	• Advantage of high quality:
		○ Annotation gene and regulatorary region
		○ Cis and trans regulation 
		○ Synteny blocks
		○ SV
		○ Repeats
? Explains of the algorithm of long reads assembly
	• Error corection
		○ Self correct
		○ Illumina correct
? Why align short to long can be unreliable?

Falcon unzip 可以生成 phased genome, do we need that?
	• Miniasm: 10 X faster, but poor…

Polish:
	• Quiver/Arrow for Pacbio
	• Nanopolish for Nanopore
	• Pilon for short->long

	• Short polish long reads
		○ 20% error => <0.1%
		○ Homopolymer/repeats are hard to correct. Because short reads cannot be confidently aligned. 
？没有详细的比较这些软件的性能差异
比如所需要的时间，，，，

10X genome : phased genome
Hi-C: for scaffolding and phasing
BioNano: SV and scaffolding
 
使用三代测序update的基因组
	· maize 15
	· fruit fly 16
	· mosquito 12
 
De novo assembly quality: 24,25
	· high contiguity: N50
	· high completeness: % genome, % of genes
	· correctness: base accuracy and structural accuracy
 
质量够好了，下游：comparative genomics
annotation: 
	· genes, regulatory sequences
	· reference mapping
	· cis- trans-
	· synteny blocks
 
Canu： MHAP approach
FALCON, MARVEL : DALIGNER approach
 
FALCON- Unzip that runs after the ini
tialcontigs are assembled to create a phased assembly
for diploid samples.
 
Correct reads errors
	· Quiver
	· Arrow
	· Nanopolish
	· Pilon
	
de novo assembly,SV detection and phasing, are highly interrelated
to each other and must be addressed at the same time to produce the best results.

# 中文翻译 
Nature Reviews|突破黑暗——长片段测序技术的应用优势及其生物信息学算法
https://mp.weixin.qq.com/s/Tq1y07KXz2tjWw7Ca2nv8A##
```

1. [Improved **maize reference genome** with single-molecule technologies](https://www.nature.com/articles/nature22971?sf88114573=1)

2. [The impact of third generation genomic technologies on plant genome assembly](https://www.sciencedirect.com/science/article/pii/S1369526616301315)

3. [A field guide to whole-genome sequencing, assembly and annotation](<https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4231593/> ) 2014

   ```markdown
   Not True Genome
   	· variation, between individuals, somatic cells, polyploid chromosomee
   	· repeat region
   	· sequence error 
   	· assembly error 
    
   reads- contigs- scaffolds-chromosomes
   50 X short reads coverage
   5 X long reads coverage 
    
   genome size,
   sequencing error rates,
   repeat content and the
   degree of genome duplications
    
   Assembly software
   	· De- Bruijn Graphs based (K-mer) [RAM intensive]
   			o SOAPdenovo
   			o ALLPATHS-LGABySS
   			o Velvet
   	· Hybrid 
   			o Atlas
   			o Rau
   			o MaSuRCA
    
   equalvation 
   	· vs expected genome size
   	· N50
   	· vs RNASeq
   	· Ultra Conserved Elelment BUSCO  and CEGMA
   	· orthologous core eukaryotic protein sequences
   	· vs reference, sister genomes
   	· TransRate
    
   Gene annotation and GO term
   mask repeat regions in the genome,
   High quality genome >90%, high accuracy
   	· evidence from other genomes 
   	· from species-specific transcriptome data
   	· MAKER
   	· TransPipe 25 Phytozome database 
   	· Genewise
    
   Alignment:
   	· PASTA
    
   trade-offs:
   minimizing mis-assemblies
   improve contiguity
   
   ```

4. [Ten steps to get started in Genome Assembly and Annotation F1000](<https://f1000research.com/articles/7-148> )

   ```markdown
   	· annotation:
   			o codeing protein, non-coding RNA, TE
   			o structure
   			o functional annotation:
   			o TE annotation 
   	· know your genome:
   			o Genome size
   			o Repeats
   			o Heterozygosity
   			o Ploidy level
   			o GC content
   	· PacBio+NanoPro
   			o 10 kbp-100kbp
   	· Supporting technologies
   			o optical mapping methods (e.g., BioNano), https://www.youtube.com/watch?v=0-NFpOPADiQ
   			o linked-read technologies (e.g., 10X Genomics Chromium system), or https://www.youtube.com/watch?v=aUyFzwRFWJQ
   			o the genome folding-based approach of HiC
   	· CPU and RAM 
   	· quality control
   	· Assembly method
   			o de Bruijn graphs
   			o Overlap Layout Consensus (OLC)
   	· Evaluation
   			o QUAST
   			o Reapr
   			o FRCBam
   			o BUSCO
    
   Determining whether the assembly is ready for annotation
   It is always possible to try one more tool or one more setting, and this wish of wanting to improve the assembly just a little bit more can delay these types of projects substantially.
   It is best to have a goal in mind before starting assembly, and to stop when that goal has been reached.
    
   Genome Annotation
   	· outputstarts with repeat identification and masking
   			o ROH
   			o TEs annotation, a major task in genome project
   					§ RepeatMasker
   					§ Repet package
   	· Gene annotation approaches
   			o intrinsic: coding and splicing site in the genome
   			o extrinsic: transcriptome 更常见
   			o combined
   	· output: fasta+gff
    
    
   reproducible
   	· Docker
   	· Nextflow, Toll, Galaxy
   
   ```

   A beginner’s guide to eukaryotic genome  annotation

   nature

   <https://www.nature.com/articles/nrg3174?WT.ec_id=NRG-201205>

    

    

   Transcriptome vs Genome assembly

   <https://en.wikipedia.org/wiki/De_novo_transcriptome_assembly#Transcriptome_vs._genome_assembly>

    

   1, genome sequencing depth is usually the same across a genome, but the depth of transcripts can vary. 

   2, both strands are always sequenced in genome sequencing, but RNA-seq can be strand-specific. 

   3, transcriptome assembly is more challenging because transcript variants from the same gene can share exons and are difficult to resolve unambiguously

    

    

   Tools for building de novo transcriptome assembly

   Current Plant Bio, 2017

   <https://www-sciencedirect-com.ezproxy2.library.arizona.edu/science/article/pii/S2214662817301032>

    

    

   Contiguous and accurate de novo assembly of metazoan genomes with modest long read coverage

   <https://academic.oup.com/nar/article/44/19/e147/2468393>

   a hybrid meta-assembly approach that achieves remarkable assembly contiguity for both Drosophila and human assemblies with only modest long molecule sequencing coverage

# Reference documents

1. [Automating the selection of genome assembly software](http://www.bioinformaticszen.com/post/automating-selection-of-genome-assembly-software/)
2. [Genome Data Access Survey](https://docs.google.com/forms/d/e/1FAIpQLSfcgM0zmZnN18Hbp6b1idA5BOMcwGdB7hhnZW1rbEnZEdiB8g/viewanalytics) (from #genome-assembly@Florian Jupe; endorsed by Matt Dimmic and Zoe McKiness)]
3. [Large Genome Assembly with PacBio Long Reads](https://github.com/PacificBiosciences/Bioinformatics-Training/wiki/Large-Genome-Assembly-with-PacBio-Long-Reads)
4. [Long read sequencing A/Prof Torsten Seemann ANGUS 2015 Workshop - KBS, Michigan, USA - Sat 15 Aug 2015 The good, the bad, and the really cool. ](https://angus.readthedocs.io/en/2016/_static/Torsten_Seemann_LRS.pdf)



# Other

### centromere 

### [Inbreeding drives maize centromere evolution](http://www.pnas.org/content/early/2016/02/04/1522008113.short)

KL Schneider, [Z Xie](https://scholar.google.com/citations?user=o7uuAEoAAAAJ&hl=en&oi=sra), TK Wolfgruber… - Proceedings of the …, 2016 - National Acad Sciences



* epigenetically by the centromere-specific histone H3 variant cenH3 
* long stretches of centromere-specific tandem DNA repeats (∼1.8 Mb in maize)



Centromere-specific tandemly arranged DNA repeats vary in
length and nucleotide sequence between species. 

Functional centromeres of maize consist of 1–2 Mb of DNA



### Telomere

### [Telomere sequence localization and karyotype evolution in higher plants](https://link.springer.com/article/10.1007/BF00982962)

J Fuchs, A Brandes, I Schubert - Plant Systematics and Evolution, 1995 - Springer

(TTTAGGG)n  in 43 of 44 plant species, except Alliaceae

```markdown
**Centromeres** are responsible for the correct transmission of chromosome complements during mitosis and meiosis. 

**Telomeres** prevent degradation of the ends of linear chromosomes
by nucleases, illegitimate fusion of natural chromosome ends with each
other or with artificial ends created by chromosome breaks, and shortening of linear
DNA molecules due to incomplete replication at the 5 '-ends by DNA polymerases.

```



# Tools

**TelSeq :**	is a software that estimates telomere length from whole genome sequencing data (BAMs).

https://github.com/zd1/telseq



[paper： Estimating telomere length from whole genome sequence data](https://academic.oup.com/nar/article-abstract/42/9/e75/1249448)

[Z Ding](https://scholar.google.com/citations?user=nbIFJRAAAAAJ&hl=en&oi=sra), [M Mangino](https://scholar.google.com/citations?user=i0m7948AAAAJ&hl=en&oi=sra), A Aviv… - Nucleic acids …, 2014 - academic.oup.com

```markdown
Telomeres cap the ends of chromosomes 

In humans, telomeres comprise sequences of 5–15 kb TTAGGG tandem repeats and their telomere binding proteins

telomere length is an indicator of replicative history and replicative potential


**telomere length measurement:**
* Southern blot
* FISH...
* qPCR

Now, NGS, here:
1. 100 bp pairend Illumina
2. 75 human, 27-74 years
examine the relationship between reads containing telomere repeat sequence and telomere length





```







**Computel :** Compute mean telomere length from Whole Genome Sequencing data. 

https://github.com/lilit-nersisyan/computel

```markdown
R based 
mean telomere length
and abundance 
NGS


```



More : https://github.com/search?q=telomere



**centromere_seeker**

https://github.com/cryancampbell/centromere_seeker

bash script to search for centromeric repeat patterns in PacBio data, using several current tools (trf and R)

**GossypiumCentromeres**

https://github.com/remkv6/GossypiumCentromeres



More : https://github.com/search?q=centromere



TRF: tandem repeat finder

https://tandem.bu.edu/trf/trfdesc.html



# telomere and centromere in B73 V4

https://www.nature.com/articles/nature22971/figures/6



[Inbreeding drives maize centromere evolution](http://www.pnas.org/content/early/2016/02/04/1522008113.short)

KL Schneider, [Z Xie](https://scholar.google.com/citations?user=o7uuAEoAAAAJ&hl=en&oi=sra), TK Wolfgruber… - Proceedings of the …, 2016 - National Acad Sciences



[Stable patterns of CENH3 occupancy through maize lineages containing genetically similar centromeres](http://www.genetics.org/content/early/2015/06/10/genetics.115.177360.short)

JI Gent, K Wang, [J Jiang](https://scholar.google.com/citations?user=vIM8IBoAAAAJ&hl=en&oi=sra), RK Dawe - Genetics, 2015 - Genetics Soc America



### [Widespread gene conversion in centromere cores](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1000327)

J Shi, SE Wolf, [JM Burke](https://scholar.google.com/citations?user=fe5GDukAAAAJ&hl=en&oi=sra), GG Presting… - PLoS …, 2010 - journals.plos.org



### [A molecular view of plant centromeres](https://www.sciencedirect.com/science/article/pii/S1360138503002747)

[J Jiang](https://scholar.google.com/citations?user=vIM8IBoAAAAJ&hl=en&oi=sra), [JA Birchler](https://scholar.google.com/citations?user=MTM2HVQAAAAJ&hl=en&oi=sra), [WA Parrott](https://scholar.google.com/citations?user=H-hpEucAAAAJ&hl=en&oi=sra), RK Dawe - Trends in plant science, 2003 - Elsevier



### [**Plant centromeres**: genetics, epigenetics and evolution](https://link.springer.com/article/10.1007/s11033-018-4284-7)

LC Oliveira, GA Torres - Molecular biology reports, 2018 - Springer

```markdown
The centromeres of higher eukaryotes have conserved kinetochore proteins

Centromeres are usually composed by satellite repeats and retrotransposons 

the sequences can differ even among closely related species

Some unusual configurations containing single copy DNA

spanning several megabases of the chromosome 

The centromeric DNA evolves rapidly and has little similarity among species

The difference between the canonical histone H3 and CenH3 is the presence in the latter of an N-terminal tail that is highly divergent with respect to the length and composition, even among closely related organisms, been species-specific in some cases

Cytogenetic analyses have shown that centromeres eventually adopt new positions in the chromosomes, an event called repositioning. The centromere in this new location is referred as evolutionary new centromeres or neocentromeres



Type: 
* point centromere: very small, a small kinetochore
* holocentrics: dispersed centromere
* monocentric chromosomes :in one region
* meta-polycentric: 

 **In S. tuberosum L. (cultivated potato) each of the 12 centromeres have a different genetic composition from the other ones. **
Other plant species which also have multiple repeats associated with different centromeres are pea (Pisum sativum L.) [8] and bean (Phaseolus vulgaris L.) [39]. 


the size of centromeric repeats:
in most of the studied plant species, they are around 150–180 bp long.

long terminal repeats (LTR) retrotransposons accumulate quite often in centromeres and pericentromeres in plants and animals

# Origin and evolution


```

**![Fig. 1](https://media.springernature.com/lw785/springer-static/image/art%3A10.1007%2Fs11033-018-4284-7/MediaObjects/11033_2018_4284_Fig1_HTML.gif)**







### [ Plant centromeres](https://www.sciencedirect.com/science/article/pii/S1369526616302266)

[L Comai](https://scholar.google.com/citations?user=ZvmgIoEAAAAJ&hl=en&oi=sra), [S Maheshwari](https://scholar.google.com/citations?user=FFO1_2YAAAAJ&hl=en&oi=sra), [MPA Marimuthu](https://scholar.google.com/citations?user=XEwlUgsAAAAJ&hl=en&oi=sra) - Current opinion in plant biology, 2017 - Elsevier

```markdown
determined epigenetically bycentromeric histone 3 (CENH3) 

Normallystable, centromeres can change position over evolutionarytimes or upon genomic stress, such as when chromosomesare brok en

Centromeres are regions on dividing chromosomes thatbind spindle microtubules

** The deﬁnition of an active centromere is based onCENH3 localization.**

kinetochore 着丝粒
DNA + CENH3 + outer kinetochore complex


Most centromeres are enriched for DNA repeats ranging in size from 100 to 1000 bp [16]. 





```



### [Comparative analysis of tandem repeats from hundreds of species reveals unique insights into centromere evolution](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2013-14-1-r10)

[DP Melters](https://scholar.google.com/citations?user=BZLjcO8AAAAJ&hl=en&oi=sra), [KR Bradnam](https://scholar.google.com/citations?user=0D3JtBAAAAAJ&hl=en&oi=sra)… - Genome …, 2013 - genomebiology.biomedcentral.com



http://korflab.ucdavis.edu/Datasets/Centromere_data/

Appendix 1 

https://static-content.springer.com/esm/art%3A10.1186%2Fgb-2013-14-1-r10/MediaObjects/13059_2012_3048_MOESM1_ESM.PDF



> The remaining sequences were analyzed by TRF [[50](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2013-14-1-r10#CR50)] to identify tandem repeats. We assumed that candidate centromeric tandem repeat arrays should be continuous and occupy the majority - if not all - of any individual read.```

> the presence of tandem repeats, and their extremely high repeat abundance (often >10,000 copies per chromosome).
>
> Therefore, we hypothesized that the most abundant tandem repeat in a given genome would be the prime candidate for the centromere repeat 
>
>

 ![](https://media.springernature.com/lw785/springer-static/image/art%3A10.1186%2Fgb-2013-14-1-r10/MediaObjects/13059_2012_Article_3048_Fig1_HTML.jpg)

```
>zea_mays
CTTTAGGTCCAAAACTCATGTTTGGGGTGATTTCGCGCAATTTCGTTGCCGCACGTCACC
CATTCCGAAAACGGGTATCGGGGTGCATACAAAGCACGAGTTTTTGCCACCGGAACAATT
TCTTCGTTTTTCGCAACGAACATGCCCAATCCACTA

>glycine_max
TCACTCGGATGTCCGATTCAGGCGCATAATATATCGAGACGCTCGAAATTGAACAACGGA
AGCTCTCGAGAAATTCAAATGATCATAACTTT

>gossypium_raimondii
TTAGGGAGATAAGATCTACAATCTTCAACCTACTCCACTGCTGCTCAGGGAGATAGGACT
GGTGGCTTAAATCTGCTTCCTACTATCTCGGGAAGATAAGATTCGCCGTCTTCGATCTGC
TCCACTACTGC

>brassica_oleracea
TCTCCACTACTTTATGTATCCAAATACAGCTTCTTACATCGCGATTCATCCTGGTTTGAT
CAGAATGACGAGGAAGTTGTCATATTCCCAAACAGGAAAACTGGGATCACCTGATTTGAA
AGTGGGATAACTTCTTCATCCTAACTCCTATGAGATTTATTCAACTTCCTGGTGAT
```



# Alpha-CENTAURI: assessing novel centromeric repeat sequence variation with long read sequencing.

https://www.ncbi.nlm.nih.gov/pubmed/27153570

http://github.com/volkansevim/alpha-CENTAURI 





[Tandem Repeats Database](http://tandem.bu.edu/cgi-bin/trdb/trdb.exe?taskid=0)

[Tandom Repeats Finder](https://tandem.bu.edu/trf/trf.html)

```
Error Message.

A system error occurred. Please go back
and try to submit your data again.
Error at line 132: can't rename upload file old name new name 41DGFQfU0s4Zc
If this error persists
send an email message to yhernand@bu.edu.
```



### A bioinformatics approach to identify telomere sequences ...

https://www.future-science.com/doi/full/10.2144/btn-2018-0057

```The telomere repeat motif (TTTAGGG)n, discovered in *Arabidopsis thaliana* [[5](https://www.future-science.com/doi/full/10.2144/btn-2018-0057#B5)], is considered to be the consensus telomere motif for most land plants [[6](https://www.future-science.com/doi/full/10.2144/btn-2018-0057#B6)]. 
The telomere repeat motif (TTTAGGG)n, discovered in *Arabidopsis thaliana* [[5](https://www.future-science.com/doi/full/10.2144/btn-2018-0057#B5)], is considered to be the consensus telomere motif for most land plants [[6](https://www.future-science.com/doi/full/10.2144/btn-2018-0057#B6)]. 

https://www.intechopen.com/books/the-mechanisms-of-dna-replication/telomeres-their-structure-and-maintenance

```









# Lynch *The origin of genome architecture, chap 5*

* centromere lengths increased with the trasition from unicellularity to multicellularity 
  * repetitive DNA families 
  * accumulation of TEs.
* the boundary between centromeric and noncentromeric regions is by no mean abrupt





 













