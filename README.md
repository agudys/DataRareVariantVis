# Annotation resources and example data for RareVariantVis 2.0.1 package

Second version of RareVariantVis package aims to annotate, filter and present genomic single nucleotide and structural variants (especially rare ones) in a global, per chromosome way. It accepts variants directly from caller - for example GATK or Speedseq. Output of package are lists of variants together with adequate visualization. 

Visualization of variants is performed in two ways - standard that outputs png figures and interactive that uses JavaScript d3 package. Interactive visualization allows to analyze trio/family data, for example in search for causative variants in rare Mendelian diseases. The package includes homozygous region caller and allows to analyse whole human genomes in less than 30 minutes. 

Here we present resources used by the package and explain how they were generated.


## All_20160601_chr19.vcf.gz
File includes dbSNP 147 variants (chromosome 19 only) extracted from original dbSNP vcf:
ftp://ftp.ncbi.nih.gov/snp/organisms/human_9606_b147_GRCh37p13/VCF/00-All.vcf.gz

## CentromeresHg19.txt
Hg19 centromere positions downloaded from UCSC table browser - All Tables - table: gap - type: centromere
https://genome.ucsc.edu/cgi-bin/hgTables

## CoriellIndex_S1.sv.vcf.gz
Structural variants called using speedseq from Ashkenazim trio son sample sequenced in Genomics Core Facility, University of Bergen, Norway. Details regarding sample are given in CoriellIndex_S1.vcf.gz section.

## CoriellIndex_S1.vcf.gz
Single nucleotide variants called using speedseq from Ashkenazim trio son sample sequenced in Genomics Core Facility, University of Bergen, Norway.

#### Details for Coriell Ashkenazim trio samples:
Ashkenazim father-mother-son trio from personal genome project:
Candidate NIST RMs 8391 (son only) and 8392 (entire trio):
www.tinyurl.com/giabajson
www.tinyurl.com/giabajtrio
NIST IDs: HG002/HG003/HG004 (Son/Father/Mother)
PGP IDs: huAA53E0/hu6E4515/hu8E87A9 (Son/Father/Mother; For some phenotype information, see participant profiles at http://www.personalgenomes.org/harvard/data)
Coriell IDs: GM24385/GM24149/GM24143 (Son/Father/Mother; cell lines and DNA available at https://catalog.coriell.org/)
Source: http://jimb.stanford.edu/giab-resources/

## ExAC.r0.3.1.sites.vep_chr19.vcf.gz
File includes ExAC 0.3.1 variants (chromosome 19 only) extracted from original ExAC vcf:
ftp://ftp.broadinstitute.org/pub/ExAC_release/release0.3.1/ExAC.r0.3.1.sites.vep.vcf.gz

## RareVariants_CoriellIndex_S1.txt

## RareVariants_Coriell_S2.txt

## RareVariants_Coriell_S3.txt

## StructuralVariants_CoriellIndex_S1.txt

## StructuralVariants_Coriell_S2.txt

## StructuralVariants_Coriell_S3.txt

## UCSC_hg19_refSeq_160702.txt

## nexterarapidcapture_exome_targetedregions_v1.2.bed

## uniprot-all.txt
