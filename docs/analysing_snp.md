# Analysing SNP data {#snp-analysis}



## STRs vs. SNPs

STRs have been and remain the dominant marker used in forensic genetics.

This is mainly due to the fact that STRs have a high mutation rate, therefore
are more diverse in human populations. This explains their high __power of discrimination__. 
Furthermore, they can also be used in deciphering mixture components, a very common
case in forensics. Finally, they can be combined in multiplex assays, which is convenient when lowamounts of biological material can be recovered.

Even though STRs will still remain the standard markers in forensic genetics 
for many years, the application of sequencing data, especially the analyses 
of SNPs became more and more popular in recent years. 

Indeed, it nowadays easier and cheaper to generate whole-genome sequences than before.
One could wonder why STRs are still so popular in forensic practice, and have not been replaced by SNPs that are easily generated from Next-Generation Sequencing (NGS) data.

The advantages of SNPs are a higher multiplex capacity (with STRs and CE we can 
analyse not much more than 25 markers in parallel) and therefore a higher 
discriminative power and shorter amplicon size (interesting for degraded samples).

## How to analyse SNP data in STRAF?

It is in theory possible to use any marker type in STRAF, as long as the input
format corresponds to what is expected from the software, that is:

* 2 columns per locus for diploid data, 1 for haploid;

* alleles are encoded by a number: for example, a diallelic SNP could be encoded as
100 for the reference allele, and 101 for the alternative allele.

The main challenge remains encoding these values and converting from the initial
data format. As an example, a genotype table is easier to convert than raw sequences
or bioinformatics-specific formats such as the Variant Calling Format (VCF).
 
