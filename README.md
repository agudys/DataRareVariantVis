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
Structural variants called using speedseq from Coriell Institute trio daughter sample (NA12878) sequenced in Genomics Core Facility, University of Bergen, Norway. Details regarding sample are given in CoriellIndex_S1.vcf.gz section.

## CoriellIndex_S1.vcf.gz
Single nucleotide variants called using speedseq from Coriell Institute trio daughter sample (NA12878) sequenced in Genomics Core Facility, University of Bergen, Norway.

### Details for Coriell trio samples:
Pilot Genome (NA12878): 

NIST RM 8398 (HG001): Available at http://tinyurl.com/giabpilot
NIST ID: HG001 Link to NA12878 DNA and GM12878 cell line from Coriell: https://catalog.coriell.org/0/Sections/Search/Sample_Detail.aspx?Ref=NA12878&Product=DNA. Source: http://jimb.stanford.edu/giab-resources/

Parents of NA12878:

NA12891: https://catalog.coriell.org/0/Sections/Search/Sample_Detail.aspx?Ref=GM12891

NA12892: https://catalog.coriell.org/0/sections/Search/Sample_Detail.aspx?Ref=GM12892

## ExAC.r0.3.1.sites.vep_chr19.vcf.gz
File includes ExAC 0.3.1 variants (chromosome 19 only) extracted from original ExAC vcf:
ftp://ftp.broadinstitute.org/pub/ExAC_release/release0.3.1/ExAC.r0.3.1.sites.vep.vcf.gz

## RareVariants_CoriellIndex_S1.txt
Output of RareVariantVis for NA12878 sample. 

## RareVariants_Coriell_S2.txt
Output of RareVariantVis for NA12891 sample - father of NA12878.

## RareVariants_Coriell_S3.txt
Output of RareVariantVis for NA12892 sample - mother of NA12878.

## StructuralVariants_CoriellIndex_S1.txt
Output of RareVariantVis for NA12878 sample - structural variants.

## StructuralVariants_Coriell_S2.txt
Output of RareVariantVis for NA12891 sample - father of NA12878 - structural variants.

## StructuralVariants_Coriell_S3.txt
Output of RareVariantVis for NA12892 sample - mother of NA12878 - structural variants.

## UCSC_hg19_refSeq_160702.txt

## nexterarapidcapture_exome_targetedregions_v1.2.bed
Illumina Nextera capture kit bed file which could be useful when running RareVariantVis on exome data. Could be alternatively replaced with other transcriptome bed files, depending on user needs.
Source: http://support.illumina.com/downloads/nextera-rapid-capture-exome-v1-2-product-files.html

## uniprot-all.txt
Uniprot annotation table for reviewed genes only. It includes following columns: 
Entry	Status, Protein names, Gene names,	Annotation,	Tissue specificity,	Gene ontology (biological process),	Involvement in disease	Cross-reference (Orphanet) and	PubMed ID.
Source: http://www.uniprot.org/uniprot/?query=*&fil=reviewed%3Ayes+AND+organism%3A"Homo+sapiens+(Human)+[9606]"
