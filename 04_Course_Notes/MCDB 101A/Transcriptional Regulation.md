# Transcriptional Regulation

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## 🎯 Learning Objectives

1. Describe the Lac operon: components, regulatory logic, and effector molecules
2. Distinguish negative vs. positive regulation using the Lac operon as a model
3. Explain catabolite repression and the role of CRP-cAMP
4. Predict operon expression under all combinations of lactose/glucose conditions
5. Describe transcription attenuation using the Trp operon as an example

---

## 🧠 Core Concepts

### The Lac Operon — Overview

**Gene Components**

| Component | Protein / RNA | Function |
|-----------|--------------|---------|
| *lacI* | Lac repressor (tetramer) | Negative regulator; binds operator |
| *lacZ* | β-galactosidase | Cleaves lactose → glucose + galactose |
| *lacY* | Lac permease | Transports lactose into cell |
| *lacA* | Thiogalactoside transacetylase | Acetylates lactose (role unclear) |

**Regulatory DNA Elements**

| Element | Location | Function |
|---------|---------|---------|
| Promoter (Plac) | Upstream of *lacZ* | RNAP binding site |
| Operator (O1) | +11 region | Repressor binding site; overlaps TSS |
| O2, O3 | Downstream/upstream | Auxiliary operators; enhance repression |
| CRP site | –61 from TSS | CRP-cAMP binding; activates transcription |

### Negative Regulation by Lac Repressor

**Default State (no lactose)**

1. Lac repressor (I gene product) binds O1 (and auxiliary operators)
2. RNAP cannot initiate transcription → **operon is OFF**

**Induction by Allolactose**

1. A small amount of basal β-galactosidase converts lactose → **allolactose** (true inducer)
2. Allolactose binds the inducer-binding domain of Lac repressor
3. Conformational change reduces repressor-DNA affinity ~1,000×
4. Repressor dissociates from operator → RNAP can transcribe → **operon is ON**

**Note:** IPTG (isopropyl-β-D-thiogalactoside) is a gratuitous inducer used in lab — induces without being metabolized.

**Gratuitous Induction**

Because allolactose is derived from lactose, the operon is auto-regulated: expression increases as substrate increases.

### Positive Regulation by CRP-cAMP

**Catabolite Repression (Glucose Effect)**

When glucose is present, the Lac operon is expressed at low levels even if lactose is present. This is because glucose suppresses cAMP levels.

**cAMP and CRP**

| Condition | [Glucose] | [cAMP] | CRP state | Transcription |
|-----------|-----------|--------|-----------|--------------|
| Glucose present | High | Low | Inactive (no cAMP) | Low (catabolite repressed) |
| Glucose absent | Low | High | Active (CRP-cAMP complex) | High |

**Mechanism of CRP Activation**

1. Low glucose → adenylyl cyclase is active → high cAMP
2. cAMP binds CRP (catabolite activator protein; also called CAP)
3. CRP-cAMP binds CRP site at –61
4. α subunit CTD of RNAP contacts CRP → increases RNAP recruitment ~50-fold

### Combined Logic Table

| Glucose | Lactose | Allolactose | Repressor bound? | CRP-cAMP? | Transcription |
|---------|---------|-------------|-----------------|-----------|--------------|
| + | – | – | Yes | No | Very low (off) |
| + | + | + | No | No | Low (moderate) |
| – | – | – | Yes | Yes | Very low (off) |
| **–** | **+** | **+** | **No** | **Yes** | **High (fully induced)** |

**Maximum expression** requires: lactose present (inducer removes repressor) AND glucose absent (CRP-cAMP activates).

### Lac Operon Mutant Analysis

**Constitutive Mutants**

| Mutation | Phenotype |
|---------|---------|
| *lacI*⁻ (null) | No repressor made → always ON |
| *lacI*^s (super-repressor) | Repressor cannot bind allolactose → always OFF |
| *lacO*^c (operator-constitutive) | Operator can't bind repressor → always ON |

**Dominance/Recessiveness**

- *lacI*⁻ is **recessive** — complemented by *lacI*⁺ in trans (repressor is diffusible)
- *lacO*^c is **cis-dominant** — operator is not diffusible; affects only genes on same chromosome
- *lacI*^s is **dominant** — super-repressor titrates out wild-type inducer in trans

**Key Rule**

**cis-acting elements** (operators, promoters) affect only genes on the same DNA molecule.
**trans-acting elements** (repressors, activators) can act on any copy of the regulated gene in the cell.

### Transcription Attenuation — Trp Operon

**Overview**

The Trp operon encodes enzymes for tryptophan biosynthesis. In addition to repressor-based regulation (TrpR + tryptophan as co-repressor), the operon uses **attenuation** — regulation by premature transcription termination.

**Leader Peptide**

- The *trpL* region (leader) encodes a 14 aa peptide (**trpL peptide**) rich in Trp residues (2 Trp at positions 10 and 11)
- This allows the ribosome to sense intracellular [Trp]

**mRNA Structure — 4 Alternative Stem-Loops**

| Region | Hairpin Pair | Consequence |
|--------|-------------|-------------|
| Segments 1:2 | Antiterminator-like | Ribosome stalled at Trp codons in 1 |
| Segments **3:4** | **Terminator hairpin** | RNAP terminates → no Trp operon transcription |
| Segments **2:3** | **Antiterminator hairpin** | Prevents 3:4 formation → RNAP reads through |

**Two Conditions**

**High [Trp] — Transcription Terminated:**
1. [Trp] high → ribosome translates leader peptide without stalling
2. Ribosome sits on segment 1, prevents 1:2 pairing
3. Segments 3:4 form terminator hairpin → RNAP terminates → no *trpEDCBA* transcription

**Low [Trp] — Read-through:**
1. [Trp] low → ribosome stalls at Trp codons in segment 1
2. Segment 2 is free → 2:3 antiterminator hairpin forms
3. Segments 3:4 cannot pair → no terminator → RNAP reads through → Trp biosynthesis genes expressed

**Key Requirement**

Attenuation requires **coupled transcription-translation** (prokaryotes only). Ribosome must be translating the leader while RNAP is still transcribing downstream regions.

---

## ⚠️ Exam Traps

- ❌ **"The Lac operon is induced by lactose"** — The true inducer is **allolactose** (isomer of lactose formed by β-galactosidase).
- ❌ **"CRP-cAMP acts by blocking the repressor"** — CRP-cAMP acts independently; it's a positive activator that recruits RNAP.
- ❌ **"Attenuation is the same as repression"** — Attenuation is premature transcription termination; repression prevents initiation. Both control expression but by different mechanisms.
- ❌ **"O^c mutations are recessive"** — cis-acting operator mutations are **cis-dominant** because the operator cannot diffuse to the other chromosome.

---

## Practice Questions

1. A bacterium has the following genotype: *lacI*⁻ *lacZ*⁺ *lacY*⁻ / *lacI*⁺ *lacZ*⁻ *lacY*⁺ (partial diploid). In the presence of lactose but absence of glucose, predict the expression of *lacZ* and *lacY* on each chromosome. Explain your reasoning.

2. Explain why removing glucose activates CRP even if cAMP is added exogenously. What is the molecular link?

3. In the Trp operon, a mutation deletes the two Trp codons in the leader peptide. Predict the effect on attenuation when intracellular [Trp] is high.

4. You isolate a mutation in *lacI* that prevents allolactose binding but not DNA binding. Is this allele dominant or recessive? Why?

5. Propose an experiment using *lacI*^s to determine whether CRP-cAMP acts in cis or trans.

---

## Related Concepts

- [[Lac Operon]]
- [[Catabolite Repression]]
- [[Transcription Attenuation]]
- [[Transcription]] — σ factor basics
- [[Bacteriophage Lambda]] — another example of genetic switch logic
