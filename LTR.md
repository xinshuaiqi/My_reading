# LTR finder

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1933203/

### Steps:

1. find full length LTR pairs 
2. distance between the two LTRs (no oversize)
3. similarity maximum => LTR candidate [I am not fully understand this step]
4.  TG...CA box and TSR support

* check **PBS** (primer Binding sites) and **PPT** (Polypurine Tract)

# LTR harvest
LTRharvest, an efficient and flexible software for ... - BMC Bioinformatics
https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-9-18
by D Ellinghaus - ‎2008 - ‎Cited by 256 - ‎Related articles 

### Features

1. based on known LTR transposon features
2. handle large genome

### Steps:

1. LTR
2. size range and distance
3. LTR are flanked by a short target size duplication (**TSD**) 4-6 bp
4. PBS PPT



in a particular genome some or most of the LTR
retrotransposons may not have these features due to
mutations they acquired during evolution.



Large deletions or insertions
of other sequences, mainly from other transposable
elements, are often observed and lead to truncated or
nested LTR retrotransposons, respectively.



**Solo LTRs, truncated elements that lack one LTR, or elements**
**with large insertions do not fulfill the model underlying**
**LTRharvest.**

However, such copies can be detected in a
postprocessing step e.g. by homology searches of the computed
LTR retrotransposons in the genome under investigation.



# LTR-retriever

https://www.ncbi.nlm.nih.gov/pubmed/29233850

### Feature: 

1. plant focused
2. consider the nature of LTR and nature of sequencing tech
3. **filter false positive LTR** (Figure 1E); high inconsistence among different tools
4. species-specific LTR library is essential 
5. report noncanonical LTR-RTs
6. high LTR similarity
7. distance between LTRs
8. filter size, gapped, tandem repeats
9. identify TSD
10. truncated, non-LTR, nested





The structure of LTR is conserved. But the seq of LTR are not conserved

Unfortunately, the level of
false negatives becomes high when more stringent
parameters are applied



genome assemblers mistakenly join
two similar sequences that belong to different TEs from
the same family. 



Modules:

* eliminate candidates that contain substantial amounts of gaps
  and tandem repeats; controls sequence length in consideration
  of both extremely long (15 kb) and short (100 bp) LTR-RTs. (exclude 4% to 19% of
  total candidates that are very likely false positives in the
  genomes of maize and rice)
* Identify internal boundary: percentage of inaccurate
  internal boundary could be as high as 30% in the rice
  genome. recover an extra 27% of high-quality LTR candidates



### [Using **RepeatMasker** to identify repetitive elements in genomic sequences](https://onlinelibrary.wiley.com/doi/abs/10.1002/0471250953.bi0410s05)

[N Chen](https://scholar.google.com/citations?user=tEN1cS0AAAAJ&hl=en&oi=sra) - Current protocols in bioinformatics, 2004 - Wiley Online Library

* identify repetitive elements in nucleotide sequences and mask them for further analysis
* To run Repeat-Masker, one needs to select the repeat library files: repeat base
* RECON generate repeat library for new species

```
The summary file is pretty much self explanatory. Below is an example.
==================================================
file name: A-355G7.fasta
sequences:          1
total length:  139958 bp
GC level:       41.03 %
bases masked    91491 bp ( 65.37 %)
==================================================
               number of      length   percentage
               elements*    occupied  of sequence
--------------------------------------------------
SINEs:              46       12182 bp     8.70 %
      ALUs          41       11603 bp     8.29 %
      MIRs           5         579 bp     0.41 %

LINEs:              42       52641 bp    37.61 %
      LINE1         38       52296 bp    37.37 %
      LINE2          4         345 bp     0.25 %

LTR elements:       20       13441 bp     9.60 %
      MaLRs         10        5618 bp     4.01 %
      Retrov.        4        5131 bp     3.67 %
      MER4_group     3        1439 bp     1.03 %

DNA elements:        8        1741 bp     1.24 %
      MER1_type      7        1114 bp     0.80 %
      MER2_type      1         627 bp     0.45 %
      Mariners       0           0 bp     0.00 %

Unclassified:        5        9215 bp     6.58 %

Total interspersed repeats:  89220 bp    63.75 %


Small RNA:           0           0 bp     0.00 %

Satellites:          0           0 bp     0.00 %
Simple repeats:     20        1647 bp     1.18 %
Low complexity:      9         437 bp     0.31 %
==================================================

* most repeats fragmented by insertions or deletions
  have been counted as one element

The sequence(s) were assumed to be of primate origin.
RepeatMasker version  11/06/98               default
ProcessRepeats version  06/16/98
```





### [Using and understanding **RepeatMasker**](https://link.springer.com/protocol/10.1007/978-1-61779-603-6_2)

S Tempel - Mobile Genetic Elements, 2012 - Springer



