# High Molecular Weight (HMW) CTAB Extraction for FERNS

**Source**: Xie et al., 2023  
**DOI**: [https://doi.org/10.1002/aps3.11526](https://doi.org/10.1002/aps3.11526)

**Note from David**:  
This protocol describes 4 DIFFERENT ways to perform a CTAB extraction, using 1 of 4 four possible lysis buffers listed below. The original publication provides recommendations on when to use which buffer given the secondary metabolite/polysaccharide content of your material.

The TLDR for recommendations is as follows: CTAB and CTAB + PVP extractions before nearly identically, with CTAB + PVP producing slightly higher DNA concentrations and less secondary metabolites. For a test run of an extraction I would use plain CTAB, and then CTAB + PVP for anything I want to sequence. CTAB + SDS seemed to produce lower quality + quantity of DNA but performed well when polysaccharide content was high, if this matches your expectations, I would use this variant. Lastly, CTAB + sorbital generated lower quality + quantity of DNA but longer fragment lengths, if your goal is long-read sequencing I would consider this variant, but also check out protocols for high molecular weight (HMW) extractions as those can get your fragments lengths an order of magnitude larger (10-70kbp vs ~3kbp).

---

## Appendix S2: Protocol for optimizing the lysis step in CTAB DNA extractions of silica-dried and herbarium leaf tissues.

This protocol is a modified version from: Schenk, J. J., L. E. Becklund, S. J. Carey, and P. P. Fabre. 2023. What is the “modified” CTAB protocol? Characterizing modifications to the CTAB DNA extraction protocol. Applications in Plant Sciences 11(3): e11517, and includes all four extractions conducted. 
Composed by K. Marlowe, updated by J. Schenk and E. Becklund

### Reagents

**CTAB lysis buffer**
Combine
- 100 mL of 1 M Tris, pH 8.0
- 280 mL of 5 M NaCl
- 40 mL of 0.5 M EDTA
- 20 g of CTAB 
Bring up to 1 L with dH2O

**CTAB + 1% PVP-10 lysis buffer**
Combine
- 100 mL of 1 M Tris, pH 8.0 
- 280 mL of 5 M NaCl 
- 40 mL of 0.5 M EDTA 
- 20 g of CTAB
- 10 g of PVP-10 (note that CTAB + PVP should be made fresh each time) 
Bring up to 1 L with dH2O

**CTAB + 1% SDS lysis buffer**
Combine
- 100 mL of 1 M Tris, pH 8.0 
- 280 mL of 5 M NaCl 
- 40 mL of 0.5 M EDTA 
- 20 g of CTAB
- 10 g of SDS
Bring up to 1 L with dH2O

**Sorbitol extractionq2 buffer**
Combine
- 0.35 M sorbitol
- 0.1 M Tris-Cl, pH 7.6
- 0.005 M EDTA
- 10 mM β-mercaptoethanol (0.5% v/v)

**Sorbitol lysis buffer**
Combine
- 0.2 M Tris-Cl, pH 7.6
- 0.05 M EDTA
- 2 M NaCl
- 2% (w/v) CTAB

---

### Procedure

#### 0. Pre-Extraction Preparation

1.	Turn on water bath to 50°C.  
2.	Add appropriate amount of β-mercaptoethanol to CTAB right before using (see p. 5 and 6 for calculations). This is a little unclear. For any reaction EXCEPT sorbitol, add BME
3.	Weigh out 5–10 mg of dry leaf tissue. Place the tissue in a labeled 1.5-mL Bead Mill tube with 1-2 metal ball bearings that are designated for the Bead Mill (or other bead grinder) in Extraction Step 1. 
4. 	Prepare stocks of 95% and 75% ethanol with ultrapure water chilled to –20°C.

#### 1. Lysis and isolation steps

1. Place tubes with beads and tissues in the bead mill. Balance your samples. Grind at 1500 rpm for 1 minute (or longer, as needed). Some recommendations for removing headspace between tops of tubes and the tray: pad the plate with several folded paper towels between tubes and the lid, or remove the lid altogether and lower the top of the genogrinder tray to be in contact with the tubes.
2. Repeat Extraction step 1 and grind the tissues for an additional minute (up to 4 min can be used to assure that the tissue is fully ground).
3. Add 500 μL of the CTAB lysis buffer, CTAB + PVP lysis buffer, CTAB + SDS lysis buffer plus β-mercaptoethanol, or sorbitol extraction buffer to the dry tissue in each tube in the fume hood. Run samples in the Bead Mill for another minute under the above settings.
4. OPTIONAL: Remove the samples from the Bead Mill.  Allow tubes to sit at room temperature for 15–20 min to reduce foam. Vortex refrigerated proteinase-K to dissolve any precipitate and then spin for ~1 s in the microcentrifuge. Add 4.0 μL of proteinase-K to each sample and briefly pipette mix or vortex and spin to condense liquid at the bottom of tube. BE CAREFUL WHEN VORTEXING STRIP TUBES, IT IS VERY EASY TO SHAKE THE LIDS FREE AND SPILL.
5. If using sorbitol, centrifuge at 13,000 (3700 for plate-spinners) rpm for 8 min, otherwise go to Step 8. Remove supernatant with a pipette and discard, keeping the pellet. The pellet will not be solid at the bottom of the tube.
6. Add 300 μL of the sorbitol extraction buffer and mix by hand.
7. Add 400 μL of the sorbitol lysis CTAB buffer plus β-mercaptoethanol. Mix well by hand.
8. Incubate samples for 1 h at 50°C in a water bath. Weigh down the tops of the tubes so that the lids don’t pop loose under the heat. Let cool and drain dry, keeping lids weighed down.
9. Add 500 μL of 24:1 CIA (chloroform isoamyl alcohol) to each tube under the fume hood.
10. Vortex for 10 s and spin at 13,000 (3700 for plate-spinners) rpm for 5 min at room temperature (~21°C).
11. Label a new set of sterile 1.5-mL microcentrifuge tubes (Sample number [on hinge], taxon, and collection or ID number; see image below for an example) and place them into a rack.
12. *Note from David: The mixture should have separated into two layers at this point with a layer of solid-ish “gunk” dividing them, the upper layer is TYPICALLY what you want (the “aqueous supernatant”), although I’ve heard rare stories of the layers getting switched. Remove the tubes from the centrifuge carefully to not disrupt phases. Remove the aqueous phase supernatant with a pipette and transfer the supernatant to the newly labeled tubes from Step 8, being careful not to disrupt the phase transition zone. If you pipette or disrupt the lower organic phases, remix the solution by vortexing and repeat Extraction Step 7 (10?). After removing supernatant, remove ball bearings and discard the old tube into a waste container in fume hood. Follow ball bearing decontamination protocol for reuse.*

#### 2. Cleaning step

1. Add 1 mL of 95% ethanol or isopropanol chilled to –20°C to the aqueous phase of each sample. Precipitate DNA overnight at –20°C. 
2. Spin samples in centrifuge at 4°C for 20 min at 13,000 (3700 for plate spinners) rpm with the hinge of the tube's lid toward the outside to know where the DNA pellet will concentrate (see images below). After centrifuging, place the tubes in a cold block to keep the pellet frozen.

#### 6. Elution and quantification

1. Add 50 μL of 1X TE buffer to each sample, pipetting up and down to dislodge and mix the pellet
2. Resuspend the pellet at 50°C for 30 min if needed to dissolve the pellet.
3. Run a 0.8% agarose test gel infused with SYBR Safe to visualize the extraction.
4. Quantify DNA using Qubit using a high-sensitivity kit. If the concentrations are too large for the machine to read with the high-sensitivity kit (>100 ng/μL), use the broad range kit.
5. Resuspended DNA should be stored in the –20°C freezer for current use or in the –80°C freezer for longer-term storage. 

**Adding 0.5% β-mercaptoethanol:**

**Ratio of CTAB : β-merc.** = 100 mL : 500 μL	    or	100,000 μL : 500 μL 	(200 : 1)

100,000 μL CTAB + 500 μL β-merc. = 100,500 μL total volume

Calculate the total volume needed:

Number of reactions × 500 μL  + 250 μL = Y μL	(250 μL is to account for pipetting error)

100,500/Y = Z

100,000/Z μL = A μL	 (this is the amount of CTAB needed)

500 μL/Z = B 	(this is the amount of β-merc. needed)

A + B should equal Y; A/B should equal 200 (the ratio)

---
