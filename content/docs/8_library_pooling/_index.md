---
# Title, summary, and page position.
linktitle: Library pooling
summary: 
weight: 8
icon: book
icon_pack: fas

# Page metadata.
title: Library pooling
date: ""
type: book  # Do not modify.
---

Now that each sample is uniquely barcoded, we can safely mix them together before shipping a unique pool to the sequencing facility.

To increase the chances that each sample will be sequenced at the same depth (i.e. we will get roughly the same amount of reads) we need to normalize the concentration of each sample. You can use {{% staticref "files/pooling.xlsx" "newtab" %}}this spreadsheet{{% /staticref %}} where you will add the Qubit reading for each sample (see below), the amplicon size (roughly estimated by gel electrophoresis or measured on a subset of samples using the Bioanalyzer) and you will get the amount of each sample that you have to mix to obtain the final library pool.

<br/>

### Qubit

Qubit is a fluorometer, and provides a more accurate quantification of amplicons than Nanodrop. You can follow the video instructions below. 

Before measuring samples, samples need to be prepared according to the following protocol:

1. **Prepare the working solution**. In a 50ml tube add 199µl of Qubit buffer and 1µl of Qubit reagent for each sample. Remember to add two samples to the total count, which we be used as standard.

| Reagent       | Amount per sample (µl) | Nr. of samples | Total |
| ------------- | :--------------------: | :------------: | :---: |
| Qubit buffer  |          199           |     n + 2      |       |
| Qubit reagent |           1            |     n + 2      |       |

2. **Aliquot the working solution in each tube**. For each sample tube aliquot 199µl, for the two standard tubes aliquot 190µl. Make sure to use the Qubit Assay tubes (see Materials below)
3. **Add standards**. In one of the standard tubes add Standard #1 and add Standard #2 to the other one. Mark tubes accordingly.
4. **Add samples**. In each of the other tubes, add 1µl of each sample. Mark tubes accordingly.
5. **Vortex** each tube for 4-5 seconds and quickly **centrifuge** it.
6. Measure amplicon concentration using follow **the video instructions below**. 

<br/>

{{< youtube pfVbbdu9-nc >}}

<br/>

### Materials

| Reagent                  | Producer     | Cat. no. |
| ------------------------ | ------------ | -------- |
| Qubit dsDNA HS Assay Kit | ThermoFisher | Q32854   |
| Qubit  Assay Tubes       | ThermoFisher | Q32856   |

