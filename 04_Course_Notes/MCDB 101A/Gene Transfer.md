# Gene Transfer

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## 🎯 Learning Objectives

1. Distinguish transformation, transduction, and conjugation as mechanisms of horizontal gene transfer
2. Describe the structure and replication of plasmids; define incompatibility groups
3. Explain generalized vs. specialized transduction and what each can map
4. Describe the F plasmid, Hfr strains, and interrupted mating to map gene order and distances
5. Calculate cotransduction frequencies to estimate gene distances

---

## 🧠 Core Concepts

### Overview of Horizontal Gene Transfer

| Mechanism | DNA Source | Vector | Frequency | Recombination Required? |
|-----------|-----------|--------|-----------|------------------------|
| **Transformation** | Naked DNA from environment | None | Low (natural); high (lab) | Yes (for chromosomal integration) |
| **Transduction** | Donor cell DNA packaged in phage | Bacteriophage | ~10⁻⁶–10⁻⁸ | Yes (for generalized) |
| **Conjugation** | Donor cell via cell-cell contact | F plasmid / pili | ~10⁻¹–10⁻⁶ (Hfr) | Yes (for chromosomal markers) |

### Plasmids

**Definition**

Autonomously replicating extrachromosomal DNA elements; usually circular dsDNA.

**Types**

| Type | Example | Key Feature |
|------|---------|------------|
| Fertility (F) plasmid | F factor | Conjugation; 100 kb; encodes tra genes |
| Resistance (R) plasmid | R1, RP4 | Antibiotic resistance genes; often conjugative |
| Col plasmid | ColE1 | Encodes colicins; kills competing bacteria |
| Virulence plasmid | pINV (Shigella) | Encodes virulence factors |
| Metabolic plasmid | CAM (Pseudomonas) | Encodes catabolic enzymes |

**Plasmid Replication and Copy Number**

- **High copy number** (e.g., ColE1, ~20–700 copies): rely on host RNAP, relaxed replication control
- **Low copy number** (e.g., F plasmid, ~1–2 copies): tight replication control; active partitioning (par system)

**Incompatibility**

Two plasmids of the same **incompatibility group** (Inc group) cannot stably coexist — they share the same replication origin control and partition system → one is lost over time.

### Transduction

**Generalized Transduction**

- **Phage:** P1 (E. coli), P22 (Salmonella)
- **Mechanism:** During lytic infection, phage packaging machinery occasionally packages a segment of host chromosomal DNA (~2% of phage genome length) instead of phage DNA → transducing particle
- **Any gene** on the chromosome can be transduced (non-specific packaging)
- **Cotransduction:** Two genes are co-packaged and co-transferred → used to measure linkage

**Cotransduction frequency ↑ with decreasing distance:**
$$\text{Cotransduction frequency} = \left(1 - \frac{d}{L}\right)^3$$
where d = distance between genes, L = size of transducible fragment (~2 min on E. coli map)

**Specialized Transduction**

- **Phage:** λ (and related phages)
- **Mechanism:** Imprecise excision of integrated prophage includes adjacent chromosomal genes → packaged into phage heads
- **Only genes flanking the att site** can be transduced (genes near attB: bio and gal in E. coli)
- Products: **λdgal** (λ defective gal) or **λdbio** (λ defective bio)

**Key Difference**

| Feature | Generalized | Specialized |
|---------|------------|------------|
| Genes transferred | Any | Only those flanking att site |
| Phage | Lytic (e.g., P1) | Temperate (e.g., λ) |
| Mechanism | Random packaging error | Imprecise prophage excision |
| Use in mapping | Cotransduction frequencies | Identifies genes near att site |

### Conjugation — The F Plasmid

**F Plasmid Structure**

- ~100 kb; ~1/40 of E. coli chromosome
- Encodes **tra** (transfer) genes: F pili, mating pair stabilization, DNA transfer machinery
- Has **oriT** (origin of transfer) — where transfer nicking occurs

**Mating Types**

| Strain | F status | Can donate? | Can receive? |
|--------|---------|------------|-------------|
| F⁺ | Carries F plasmid | Yes (transfers F) | No |
| F⁻ | No F plasmid | No | Yes |
| **Hfr** | F integrated into chromosome | Yes (transfers chromosomal DNA) | No |
| F' | F plasmid carrying chromosomal genes | Yes (transfers chromosomal genes at high freq) | No |

**F⁺ × F⁻ Mating**

1. F pilus extends from F⁺ and contacts F⁻
2. Mating pair stabilized; F pilus retracts to bring cells together
3. **Rolling circle replication** at oriT: one strand of F is nicked, 5' end transferred to F⁻
4. Both cells synthesize complementary strand → both become F⁺
5. Chromosomal genes rarely transferred (F remains extrachromosomal)

### Hfr Strains — Chromosomal Gene Transfer

**How Hfr Forms**

F plasmid integrates into the bacterial chromosome at regions of homology (IS elements) → **Hfr** (high-frequency recombination) strain.

**Hfr × F⁻ Mating**

1. oriT is nicked; transfer begins at the **origin** end of the integrated F
2. Chromosomal genes are transferred in **linear order**, starting with genes nearest to oriT
3. Transfer takes ~100 min for complete chromosome (at 37°C)
4. **Complete transfer is rare** — mating pairs usually separate before the entire chromosome is transferred
5. The **trailing end of F is transferred last** → F⁻ recipient **rarely becomes F⁺**

**Key Points**

- Recipient remains F⁻ (almost always) because transfer is incomplete
- Transferred ssDNA must recombine with recipient chromosome via RecA → requires homology
- The **order of gene transfer** reflects their **position on the chromosome** relative to oriT

### Interrupted Mating — Gene Mapping

**Principle**

Mix Hfr × F⁻ cells; at timed intervals, separate mating pairs (blender/vortex) and plate on selective medium for specific donor markers.

**Reading a Transfer Map**

- The **time at which a gene first appears** in recombinants = the gene's distance from oriT (in minutes)
- **1 minute of transfer ≈ ~47 kb** on the E. coli chromosome
- Plot: % recombinants vs. time → each gene shows a characteristic entry time
- **Gradient of transfer:** Genes farther from oriT enter later and at lower frequency

**Example**

Hfr donates markers in order: **thr⁺ (8 min) → leu⁺ (9 min) → azi^R (11 min) → ton^R (11.5 min) → lac⁺ (25 min)**
→ Gene order: oriT → thr → leu → azi → ton → ... → lac

**Building the Complete Circular Map**

Use multiple Hfr strains with different integration sites and orientations → combine entry times to assemble the complete *E. coli* circular chromosome map.

### Sexduction (F' Plasmids)

- Hfr undergoes imprecise excision → **F' plasmid** carries chromosomal genes
- F' × F⁻: chromosomal genes transferred at high frequency → **merodiploid/partial diploid**
- Used to test **dominance/recessiveness** and **cis/trans** relationships (complementation in bacteria)

---

## ⚠️ Exam Traps

- ❌ **"Hfr strains transfer F to the recipient"** — Hfr strains almost never transfer the complete F, so the recipient stays F⁻.
- ❌ **"Cotransduction frequency directly equals physical distance in kb"** — Use the formula; it's not linear.
- ❌ **"Specialized transduction transfers any gene"** — Only genes flanking the phage attachment site (attB) can be incorporated into the transducing phage.
- ❌ **"F⁺ × F⁻ transfers chromosomal genes at high frequency"** — Only F plasmid is efficiently transferred; chromosomal transfer requires Hfr.

---

## Practice Questions

1. In a P1 transduction experiment, genes A and B are cotransduced at 35% frequency. Genes B and C are cotransduced at 42%. Genes A and C are cotransduced at 5%. What is the order of these three genes on the chromosome?

2. An Hfr strain transfers markers in the following order: met⁺ (5 min), his⁺ (10 min), trp⁺ (20 min), leu⁺ (35 min). If mating pairs are separated at 25 minutes, which markers will be found in recombinants?

3. Explain why Hfr × F⁻ matings rarely produce F⁺ exconjugants, while F⁺ × F⁻ matings almost always do.

4. Two F⁻ mutations (*lacZ*⁻ and *lacY*⁻) are tested against each other using an F' plasmid carrying *lac*⁺. Predict whether complementation will restore β-galactosidase activity.

5. Specialized transduction with λ can only transduce genes near attB. A researcher wants to use λ to transduce the *trp* operon (located far from attB). What modification to the experimental system would allow this?

---

## Related Concepts

- [[Conjugation]]
- [[Hfr Conjugation Mapping]]
- [[Transduction]]
- [[Plasmids]]
- [[Recombination]] — transferred DNA must recombine into recipient chromosome
- [[Bacteriophage Lambda]] — λ specialized transduction
