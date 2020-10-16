---
title: Primers
linktitle: Primers
type: book
date: ""

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 4
---

For a metabarcoding project you will need two set of primers. The first set of primers will amplify your target locus. The second set of primers will add a barcode (to uniquely mark your sample) and the necessary nucleotide sequence for the machine to recognize your amplicons as part of a library.

### First primer set

This is pretty straightforward. You will need just two primers that you can use for all your samples. The primer pair depends on your target.

| Target                             |                       FW (5'-3')                        |                      REV (5'-3')                       |
| ---------------------------------- | :-----------------------------------------------------: | :----------------------------------------------------: |
| 16S (e.g. bacteria). **515F-806R** |  TCGTCGGCAGCGTCAGATGTGTATAAGAGACAGGTGYCAGCMGCCGCGGTAA   | GTCTCGTGGGCTCGGAGATGTGTATAAGAGACAGGGACTACNVGGGTWTCTAAT |
| ITS2 (e.g. fungi). **ITS1f-ITS2**  | TCGTCGGCAGCGTCAGATGTGTATAAGAGACAGCTTGGTCATTTAGAGGAAGTAA | GTCTCGTGGGCTCGGAGATGTGTATAAGAGACAGGCTGCGTTCTTCATCGATGC |

There are many other primer pairs that target other loci. Consult the literature to choose correctly the primer pair according to your target. Do not forget to add the overhang sequence at the 5' end of your locus-specific primer, otherwise the second PCR run will not work. Here is an example:

| Primer | Overhang                           | Locus-specific           | Final primer                                               |
| ------ | ---------------------------------- | ------------------------ | ---------------------------------------------------------- |
| FW     | TCGTCGGCAGCGTCAGATGTGTATAAGAGACAG  | **GTGYCAGCMGCCGCGGTAA**  | TCGTCGGCAGCGTCAGATGTGTATAAGAGACAG**GTGYCAGCMGCCGCGGTAA**   |
| REV    | GTCTCGTGGGCTCGGAGATGTGTATAAGAGACAG | **GGACTACNVGGGTWTCTAAT** | GTCTCGTGGGCTCGGAGATGTGTATAAGAGACAG**GGACTACNVGGGTWTCTAAT** |

**Do not forget that both FW and REV primers have to be in 5'-3' direction**

### Second primer set

For the second PCR you can use the primers from the Nextera Library Prep Kits. 

You can download a {{% staticref "files/primer_list.xls" "newtab" %}}list of primers here{{% /staticref %}}. This allows you to work with a maximum of 96 samples per time.

If you need more primer pairs, you can expand the list above with the barcodes {{% staticref "files/illumina_adapters.pdf" "newtab" %}}listed at pp. 10-13 here{{% /staticref %}}. When building the primer set follow the example below.

**FW**. 5'-CAAGCAGAAGACGGCATACGAGAT[**<u>i7</u>**]GTCTCGTGGGCTCGG-3'

**REV**. 5'-AATGATACGGCGACCACCGAGATCTACAC [**<u>i5</u>**]TCGTCGGCAGCGTC -3'

You can build your custom i7 and i5. Remember that they can be 6-8bp long and **must be unique**!!! Also there are some technical requirements to keep in mind, so make sure to read the literature thorougly.

