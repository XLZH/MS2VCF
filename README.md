MS2VCF
=================
Convert the MSMS or MS output to VCF file format

Usage
=================
      python Ms2Vcf.py <in.ms> <haps_num>
          eg. python Ms2Vcf.py example.ms 10

      1. example.ms: output of MSMS or MS
            eg. msms -N 10000 -ms 10 1 -s 10 > example.ms

      2. haps_num:  the number of haplotype

Note
==================
In order to make the script more easier to use, there are some prerequisites:

* The Haplotypes number must be even number (eg. 2, 4, 6, 8, ...)
* Only one repeat is allowed in MS/MSMS (you could do multiple times with MS/MSMS)
* All the Ref/Alt are set to A/T (it is just used to occupy a filed of VCF file)
* Because Human is diploid, I use two adjacent haplotypes to construct the genotype of one sample.
