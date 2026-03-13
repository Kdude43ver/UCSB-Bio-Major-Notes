# Recombination

## Definition
Recombination is the process of **exchange between DNA molecules** resulting in new combinations of genetic material. In bacteria, homologous recombination (HR) requires long stretches of DNA sequence identity (≥50–100 bp) and is essential for: repairing double-strand breaks (DSBs), restarting stalled replication forks, and enabling genetic exchange during conjugation, transduction, and transformation.

---

## The Holliday Model (Single Crossover)

The classical model describing the physical exchange of strands between homologous duplexes.

### Steps
1. **Alignment**: Two homologous DNA duplexes align in register
2. **Strand Invasion**: A nick is introduced in each duplex; single-stranded regions invade the complementary duplex → form **heteroduplex DNA** (strands from different parents)
3. **Holliday Junction**: The crossed-strand structure connecting both duplexes
4. **Branch Migration**: The junction slides along DNA (mediated by RuvA/RuvB) — extends the region of heteroduplex
5. **Resolution**: RuvC endonuclease cleaves the Holliday junction in two orientations:
   - **Horizontal cut** → **Patch** recombinants (parental flanking markers; gene conversion possible in heteroduplex region)
   - **Vertical cut** → **Splice** recombinants (flanking markers exchanged = crossover)

---

## The Double-Strand Break (DSB) Repair Model

The primary mechanism for repairing broken chromosomes in bacteria, mediated by the **RecBCD pathway**.

### RecBCD Complex
- **RecB**: 3'→5' helicase + nuclease
- **RecD**: 5'→3' helicase (faster)
- **RecC**: Regulatory; DNA recognition
- RecB and RecD move at different speeds → creates a **loop in the 3' strand**

### Chi Sites (χ = GCTGGTGG)
- Act as a "molecular throttle" recognized by RecBCD
- When RecBCD encounters a Chi site: **RecD is inactivated** → nuclease activity switches from 3' strand to 5' strand → generates a **3' single-stranded overhang**
- Chi sites are overrepresented in E. coli genome → promotes recombination near DSBs

### RecA — The Central Recombinase
- Loads onto the 3' ssDNA overhang (coated by SSB first)
- **RecA filament** performs **strand invasion**: searches for homology on intact duplex, inserts the ssDNA → forms D-loop (displacement loop)
- Drives **strand exchange** with ATP hydrolysis
- Result: heteroduplex DNA identical to Holliday junction intermediate

### RuvABC Resolution Complex
- **RuvA**: DNA-binding; binds Holliday junction; targets RuvB
- **RuvB**: ATPase/translocase; drives **branch migration** (moves junction along DNA)
- **RuvC**: **Endonuclease**; resolves Holliday junction; cleaves at consensus sequence (A/TTG↓C)
  - Cuts in one of two orientations → determines patch vs. splice outcome

---

## Outcomes of Recombination

| Outcome | Flanking Markers | Description |
|---------|-----------------|-------------|
| **Splice (crossover)** | Exchanged | Traditional crossover; flanking alleles recombined |
| **Patch (non-crossover)** | Parental | Flanking markers unchanged; heteroduplex region may show gene conversion |

### Gene Conversion
- Repair of mismatched heteroduplex DNA results in one parental sequence "converting" to the other
- Observed as non-Mendelian segregation ratios (e.g., 3:1 instead of 2:2 in fungi)

---

## Recombination in Genetic Mapping

Recombination frequency between two loci is proportional to distance:
- **Closer genes** → lower recombination frequency → fewer crossovers
- Used to construct **linkage maps** (map units = centimorgans, cM)
- In bacteria: used to map gene order in interrupted mating (conjugation) and cotransduction

---

## Key Proteins Summary

| Protein | Function |
|---------|----------|
| RecBCD | Helicase/nuclease complex; processes DSB ends; recognizes Chi sites |
| RecA | Strand invasion; homology search; D-loop formation |
| SSB | Stabilizes ssDNA; removed by RecA |
| RuvA | Binds Holliday junction; recruits RuvB |
| RuvB | Branch migration (ATPase) |
| RuvC | Holliday junction resolution (endonuclease) |

---

## Key Exam Points
- Holliday junction = crossed-strand intermediate; resolved by **RuvC**
- **RecA** is the central strand exchange protein — coats ssDNA, finds homology, drives invasion
- Chi sites **stimulate** recombination by switching RecBCD nuclease activity
- RuvABC: A = binds junction, B = migrates junction, C = resolves junction
- **DSB repair model** (RecBCD → Chi → RecA → RuvABC) is the primary bacterial pathway
- Patch vs. splice outcome depends on **orientation of RuvC cleavage**
- Gene conversion = marker from one parental DNA "converts" the other; non-Mendelian segregation
- Recombination is required for Hfr × F⁻ gene integration and phage transduction

---

## Related Concepts
- [[Conjugation]]
- [[Transduction]]
- [[DNA Repair Pathways]]
- [[Deletion Mapping]]
- [[Mutations]]

## Prerequisites
- DNA structure and replication
- Bacterial chromosome organization
- Basic genetics and linkage

## Importance: HIGH YIELD
RecA, RecBCD, Chi sites, RuvABC, Holliday junction resolution, and patch vs. splice outcomes are all heavily examined.
