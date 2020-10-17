---
title: Protocol 2nd PCR
linktitle: Protocol 2nd PCR
type: book
date: ""

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 2
---

{{% alert note%}}

This protocol is very similar to the one before. Be careful: some reagents quantities and the thermocycler program are slightly different.

{{% /alert %}}

<br/>

For this second PCR, the master mix has to be prepared according to the table below.

| Reagent          | Amount per sample (µl) | Nr. of samples | Adjustement | Final Volume (µl) |
| ---------------- | :--------------------: | :------------: | :---------: | :---------------: |
| Water            |           4            |       24       |    x1.1     |       105.6       |
| Reagent mix (2X) |           10           |       24       |    x1.1     |        264        |

You might have noticed that primers are not in the master mix. This is correct, and it is because you need to add a different combination of primers to each well. If you look carefully at the primer list, you will notice that both i7 (FW) and i5 (REV) primers have unique barcodes. We will use their combination to uniquely barcode our samples, so it will be safe to mix them all together and segregate reads during the bioinformatic analysis. 

For example if we have a plate, we will use a set of twelve i7 primers (one for each column) and eight i5 primers (one for each row). They will form a grid, and they combination is unique (12 x 8 = 96 unique combinations for 96 wells in a plate!). So, practically, what you need to do is:

1. Dispense **14µl of master mix** for each well.
2. Arrange your twelve i7 primers in a imaginary row and aliquot **2µl** of  the same i7 primer in all the eight wells forming the column of a 96-well PCR plate. Then, arrange the eight i5 imers in a imaginary column  nd aliquot **2µl** of the same i5 primer in all the twelve wells forming the row of a 96-well PCR plate. Each well will have a different combination of primers. Have a look at {{% staticref "files/Illumina_protocol_16S.pdf" "newtab" %}} pp. 10-12 here{{% /staticref %}} for a visual representation. <u>If you have less then 96 samples</u>, plan carefully this step by scaling down the number of primers but keeping in mind the same phylosophy that each combination of primers **MUST BE UNIQUE**. You can use [this template](http://www.cellsignet.com/media/plates/96.jpg) to keep track of the primer you use in each well.
3. Add **2µl of a single DNA sample** to each well. You can use [this template](http://www.cellsignet.com/media/plates/96.jpg) to keep track of the samples in each well. There is no need to add positive/negative controls.
4. After all your samples are correctly dispensed, close your reaction tubes tightly and mark them. This is especially important if you use single tubes or sube strips. If you are using a plate, seal it with the adhesive foil.
5. When your tubes (or plate) are tightly sealed, vortex them briefly and quickly spin them with the centrifuge.
6. Put samples in the thermocycler and run the program below:

* 95°C x 3 min
* 8 cycles of:
  * 95°C for 30 seconds
  * 55°C for 30 seconds
  * 72°C for 30 seconds
* 72°C for 5 minutes
* Hold at 4°C

