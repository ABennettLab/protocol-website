---
# Title, summary, and page position.
linktitle: General workflow
summary: 
weight: 2
icon: book
icon_pack: fas

# Page metadata.
title: General workflow
date: ""
type: book  # Do not modify.
---

This is the general workflow for a matabarcoding project.

### Step 1 – DNA extraction
The first step is to extract DNA from our samples. There are a variety of methods, so I advice to consult the DNA extraction section below for further details. After DNA extraction, you need to perform a quick QC using a spectrophotometer (Nanodrop). This instrument will tell you how much DNA there is in your sample (in ng/µl) and if there is contamination by proteins or other organic compounds. If DNA is not pure enough, you can opt to perform a purification procedure using the SPRI protocol.

### Step 2 – PCR
Now that DNA is extracted. We need isolate our target for sequencing. This target may vary according to the scope of our experiment (16S for bacteria, ITS for fungi, and so on), and to isolate this short fragment (usually < 500bp) we use PCR to make thousands and thousands copies of our target. The primers we use for this first PCR have some modifications. They are made of two sections, attached to each other. We have a section that matches our target (target-specific, e.g. 16S), so it can be used for amplification. A second section, placed before the target-specific one, has a unique nucleotide sequence that matches the primers that will be used for the second PCR (see below).

### Step 3 – Gel electrophoresis
Now that our PCR is done, we need to check if it was successful. To do so, we use gel electrophoresis. This will allow us to check if our amplicons are there, and if they are (roughly) of the size we expect. Remember that here our positive control MUST show amplification, and our negative control MUST be clear, otherwise you have to repeat the PCR.

### Step 4 – Amplicon clean-up
If you got a successful amplification – congrats! Now it is time to clean it from all the stuff we do not want to carry over (enzymes, spare nucleotides and especially primers). Thus, you can use the SPRI protocol to perform this step.

### Step 5 – 2nd PCR
Now that you have a sample with just the amplicons, it is time to run a second PCR. This has a lower number of cycles (<10) and we use it for two reasons. First, we need to uniquely tag each sample, so during sequencing the machine can split the data for each sample. Second, we need to attach a short fragment to make our amplicons sequencer-readable. See the section below for details.

### Step 6 – Amplicon clean-up
Now you have to cross your fingers, because there is no immediate way to check if your second PCR was successful. Thus, no electrophoresis needed here. You can directly purify your amplicons using the SPRI method.

### Step 7 – Final steps
Almost there! Now you have a library of amplicons for each of your starting samples. Each library is uniquely barcoded, so the sequencer can split the reads according to you samples. Before submitting your sample for sequencing, there are few things to do.

1. Quantify the concentration of amplicons for each of your sample using a fluorometer (Qubit). Here, a value is very low (< 5 ng/µl) should be considered as red flag. Consider to prepare the library again for those samples, and to reach out for advice.
2. Once quantified, you need to pool all your samples together. To ensure that each sample would be sequenced at the same depth, we need to pool them according to their concentration. Consult the section below for further instruction.
3. Quantify again the final pool using a Qubit, and dilute it according to the instructions from the sequencing facility.
4. Run your final pool on a Agilent BioAnalyzer (or Agilent TapeStation), to accurately measure the size of the amplicons in your pool.

### Step 8 – Submit your sample for sequencing
Congratulations! You are done!

**Consult your sequencing facility for further instructions on how to submit your sample, and good luck with the sequencing run and data analysis.**

{{% alert note%}}
If you want to know more about each single technique, you will find some material to study at the beginning of each section.
{{% /alert %}}

### General consumables required

| Consumables                                    | Producer | Cat. no.  |
| ---------------------------------------------- | -------- | --------- |
| Disposable Microcentrifuge Tubes. 2ml. 500pc   | VWR      | 20170-170 |
| Pipet Tips, Standard Line 1000ul               | VWR      | 10017-224 |
| Pipet Tips, Standard Line 200ul                | VWR      | 10017-222 |
| Pipet Tips, Standard Line 10ul                 | VWR      | 10017-218 |
| Low-Retention Aerosol Filter Pipet Tips 1000ul | VWR      | 89174-530 |
| Low-Retention Aerosol Filter Pipet Tips 100ul  | VWR      | 10126-388 |
| Low-Retention Aerosol Filter Pipet Tips 10ul   | VWR      | 89174-522 |

