---
title: Protocol
linktitle: Protocol
type: book
date: ""

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 2
---

{{% alert note%}}

Tips

* Before beginning thaw all the reagents and keep them on ice
* Also, clean your working station thorougly with 70% ethanol or 5% bleach

* Use **filter tips** when working with reagents or dispensing the master mix
* Always wear new gloves when you begin, this will reduce the chances of contamination

{{% /alert %}}

<br/>

The first step to perform a PCR is to make the **master mix**. This is a mix of all the reagents required for  PCR with the exclusion of your samples. In this tutorial we are using a ready mix reagent, which means that MgCl<sub>2<sub/> and dNTPs are already mixed into the solution. If you are not using a ready mix, consult the reagent's protocol for instructions.

When assembling the master mix, it is important to keep constant the ratio between the reagents. So, you can scale up or scale down the total volume per sample according to your needs. For a standard metabarcoding project, 20µl per sample are enough to work with.

It is also important to increase the volume of each reagent by ~10% to correct for pipette errors.

To know which primer set best suits your project, check the primer section below.

Keep in mind that all the reagents are very expensive, and if you are working on a microbiome project it is very easy to contaminate these reagents (microbes are everywhere). So put extra care when you handle these reagents, and always use filtered tips when you handle them, especially if you share pipettes with other users or if you perform multiple procedures with the same pipettes.

When you are ready, you can assemble the mastermix using this table as example. Remember to change the amount of reagent per sample if you are scaling up or scaling down you reaction volume, and the amount of samples if it is different. Also, keep a look at the total final volume, and make sure to not exceed 1000µl per tube . A higher amount would make the mixing process difficult. You can always prepare multiple tubes for the same run.

| Reagent          | Amount per sample (µl) | Nr. of samples | Adjustement | Final Volume (µl) |
| ---------------- | :--------------------: | :------------: | :---------: | :---------------: |
| Water            |          7.8           |       24       |    x1.1     |       205.9       |
| FW primer        |          0.6           |       24       |    x1.1     |       15.84       |
| REV primer       |          0.6           |       24       |    x1.1     |       15.84       |
| Reagent mix (2X) |           10           |       24       |    x1.1     |        264        |
|                  |           19           |                |             |      501.58       |

After assembling the master mix, mix it well with a vortex (medium speed) and spin it down with a centrifuge (few seconds).

Using a filtered tip, dispense the amount of mix per sample (19µl in the example).

After dispensing the right amount of mix per sample, you can add the DNA (1µl for this example).

Remember to include **ALWAYS** two extra samples in your analysis:

* a **positive** control. It is a sample that you know will lead to a correct amplification. It can be DNA extracted from a bacterial culture (16S), a fungal culture (ITS) or from an environmental sample.
* a **negative** control. This is very important. This control will test for reagents or instrument contamination. Here, you will replace the DNA sample with water. At the electrophoresis, no band should be visible otherwise you have to discard the whole bulk of samples you amplified using the same master mix. If you obtain a amplification band in your negative control, try to make a new set of working solution for your primers and use another bottle of water. If this does not solve the problem, try again after thoroughly cleaning your pipettes and autoclaving them. As last resource, try another stock of reagent mix.

After all your samples are correctly dispensed, close your reaction tubes tightly and mark them. This is especially important if you use single tubes or sube strips. If you are using a plate, seal it with the adhesive foil. You can use [this template](http://www.cellsignet.com/media/plates/96.jpg) to keep track of the samples in each well.

When your tubes (or plate) are tightly sealed, vortex them briefly and quickly spin them with the centrifuge.

**Your samples are now ready for the thermocycler!**

