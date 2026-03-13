# MCDB 101A Final Exam Study Guide
## Comprehensive Post-Midterm 2 Genetics Review

**Course:** Molecular Genetics I (MCDB 101A)
**Level:** Junior Undergraduate
**Exam Scope:** Lectures 11–17 (Mutations, DNA Repair, Recombination, Gene Transfer, Molecular Techniques)
**Study Mode:** Complete & Interactive
**Last Updated:** 2026-03-12

---

## Table of Contents

1. [Module 1: Mutations](#module-1-mutations)
2. [Module 2: DNA Repair Systems](#module-2-dna-repair-systems)
3. [Module 3: Recombination & Mapping](#module-3-recombination--mapping)
4. [Module 4: Horizontal Gene Transfer](#module-4-horizontal-gene-transfer)
5. [Module 5: Molecular Techniques](#module-5-molecular-techniques)
6. [Study Strategies & Exam Tips](#study-strategies--exam-tips)
7. [Practice Test Bank](#practice-test-bank)

---

# MODULE 1: MUTATIONS

## Quick Reference Card

| Concept | Definition | Key Details |
|---------|-----------|------------|
| **Spontaneous Mutation** | Random change in DNA sequence without external mutagen | Rate: 10^-9 to 10^-10 per bp per generation; causes: replication errors, spontaneous lesions, tautomeric shifts |
| **Induced Mutation** | Change caused by external mutagen (chemical, radiation) | Chemical: alkylating agents, intercalators, base analogs; Physical: UV, ionizing radiation, nitrous acid |
| **Point Mutation** | Single nucleotide change | Transition (purine ↔ purine) vs. Transversion (purine ↔ pyrimidine) |
| **Frameshift** | Insertion/deletion not divisible by 3 | Shifts reading frame; affects ALL downstream codons |
| **Silent Mutation** | No amino acid change (wobble position) | Synonymous; usually least harmful |
| **Missense Mutation** | Amino acid change | May or may not affect protein function |
| **Nonsense Mutation** | Creates stop codon | Premature termination; severe damage |

## Luria-Delbrück Fluctuation Test — The Classic Experiment

### Why It Matters
Proves that mutations arise **before selection**, not in response to it.

### Experimental Design
```
Flasks with separate cultures (many small flasks)     |    One large flask
      ↓                                               |        ↓
  Random, independent growth                       Synchronized growth
  Various mutation times                              All cells together
         ↓                                                   ↓
 Plate on selective medium                    Plate on selective medium
         ↓                                                   ↓
HIGH VARIANCE in resistant                  LOW, consistent variance
   colony counts (0, 0, 2, 56, etc.)           in resistant colonies
     (Some "jackpot" cultures)
         ↓
    CONCLUSION: Mutations pre-exist
    (If induced by phage, all would show similar numbers)
```

### Key Statistics
- **Fluctuation cultures**: Mean ≠ Variance (high variance)
- **Large culture**: Mean ≈ Variance (Poisson distribution)
- **High variance ≈ pre-existing mutations**
- **Low variance ≈ spontaneous mutations during growth**

### Interpretation
If resistant mutants arose randomly during growth:
- Early mutations → many descendants (jackpot)
- Late mutations → few descendants
- Creates HIGH variance

If mutations induced by phage (adaptation):
- All cultures equally stressed
- Mutations at consistent frequency
- Creates LOW variance

---

## Mutation Types & Nomenclature

### By Molecular Change
```
Wild-type DNA: 5'-ATGCGATCG-3'

POINT MUTATION:
↓ Transition (A-T ↔ G-C)
  5'-ATGCGATCG-3' → 5'-ATGCGATGG-3' (T→G, A→C on complement)

↓ Transversion (Purine ↔ Pyrimidine)
  5'-ATGCGATCG-3' → 5'-ATGCTATCG-3' (A→T on complement: G-C → T-A)

INSERTION:
  5'-ATGCGATCG-3' → 5'-ATGCGAATCG-3' (insert A after position 5)

DELETION:
  5'-ATGCGATCG-3' → 5'-ATGCATCG-3' (delete G at position 4)
```

### By Reading Frame (Codon Shift)
Original: ATG CGT AAC GAA (Met-Arg-Asn-Glu)

**Frameshift +1 (insertion of 1 bp)**: ATG CXG TAA CGA A (completely different after insertion)

**Frameshift +3 (insertion of 3 bp)**: ATG XXX CGT AAC GAA (restores frame after insertion)

---

## Sources of Spontaneous Mutations

### 1. Replication Errors
**Challenge**: DNA polymerase III is very accurate (error rate ~10^-10 after 3'→5' exonuclease proofreading)
- Still, ~1 error per 10^9–10^10 nucleotides incorporated
- Tautomeric shifts: rare tautomeric form of base allows mis-pairing

### 2. Spontaneous Lesions
**Deamination**:
- Cytosine → Uracil (recognized by uracil glycosylase; repaired by BER)
- 5-methylcytosine → Thymine (often escapes repair → C:G → T:A mutation)

**Oxidation**:
- 8-oxoguanine (8-oxoG): mimics thymine; pairs with adenine → G:C → A:T after replication
- Reactive oxygen species (ROS) from cellular respiration

### 3. Transposable Elements
- **Insertion sequences**: Direct insertion of transposon into gene → frameshift or nonsense

---

## Induced Mutations — Mutagen Classes

### Chemical Mutagens

**Alkylating Agents** (EMS, MMS, nitrosamines):
- Add alkyl group to purine bases
- Causes mispairing → transition mutations (usually)
- Example: Guanine methylation (7-methylguanine) → mispairs with adenine → G:C → A:T

**Base Analogs** (5-bromouracil, 2-aminopurine):
- Incorporated into DNA during replication (mimic natural bases)
- Exhibit abnormal tautomeric shifts → aberrant pairing in next replication round
- 5-BrU usually pairs with A; rare tautomeric form pairs with G → T:A → C:G or G:C → A:T

**Intercalating Agents** (acridine dyes, ethidium bromide):
- Insert between base pairs (distort double helix)
- Causes frameshift mutations (insertion or deletion during replication)
- Used in research labs; mutagenic!

### Physical Mutagens

**UV Light** (254 nm, most mutagenic):
- Thymine dimerization: forms covalent bond between adjacent T on same strand
- Creates 6-4 photoproducts
- Blocks replication fork & transcription
- Repaired by NER (see Module 2)

**Ionizing Radiation** (X-rays, gamma rays, alpha particles):
- High-energy; causes **double-strand breaks** (DSBs)
- Also causes single-strand breaks, oxidative damage
- Repaired by DSB repair pathways (see Module 2)

**Nitrous Acid (HNO₂)**:
- Deaminates amino groups on bases
- A → hypoxanthine (pairs with C) → A:T → G:C
- C → uracil (pairs with A) → C:G → T:A
- G → xanthine (still pairs with C) → no change
- T unaffected
- Result: A:T ↔ G:C transitions

---

## Mutation Rates & Calculation

### Notation
- **μ** = mutation rate per cell per generation (or per base pair per replication)
- **N** = number of cells
- **r** = number of mutants observed

### Basic Relationship
E(r) = μN

### Example Problem
**Given**: 10 separate cultures of *E. coli* (~10^8 cells each) grown, then plated on phage-containing medium:
- Culture 1: 0 resistant colonies
- Culture 2: 0
- Culture 3: 0
- Culture 4: 0
- Culture 5: 0
- Culture 6: 0
- Culture 7: 2
- Culture 8: 0
- Culture 9: 0
- Culture 10: 56

**Calculate**: Mutation rate

**Solution**:
1. Identify jackpot (culture 10 with 56 colonies)
2. Calculate mean from non-jackpot cultures: (0+0+0+0+0+0+2+0+0)/9 = 0.22
3. Use median or robust estimate: typically use **culture with smallest number of mutants** as best estimate of new mutations during sampling
4. μ = r / N = 0.22 / 10^8 = 2.2 × 10^-9 per cell per generation

**Interpretation**: For every 10^9 cells that divide, roughly 2 spontaneous mutations occur (very low baseline rate).

---

# MODULE 2: DNA REPAIR SYSTEMS

## The Four Main Pathways

```
              DNA DAMAGE
                 ↙  ↓  ↘
            /    │    \
      MMR    NER     BER      DSB Repair
       │      │       │          │
    Replication  Large   Small   Double-
     Errors     Lesions   Lesions  Strand
    (G-T, A-A)  (TT dim)  (oxidn)  Breaks
                          (uracil)
```

---

## PATHWAY 1: MISMATCH REPAIR (MMR)

### What It Repairs
- Replication errors NOT caught by polymerase 3'→5' exonuclease
- Typical mismatches: G-T, A-A, C-C, T-T
- Replication error rate: ~10^-10 with proofreading; MMR reduces to ~10^-12

### The *E. coli* System

**Key Proteins**:

| Protein | Role |
|---------|------|
| **MutS** | Mismatch recognition; recruits MutL |
| **MutL** | Coordinates repair; recruits MutH and endonucleases |
| **MutH** | Endonuclease; nicks unmethylated strand |
| **Exonuclease I** | Degrades nicked strand (5'→3' direction) |
| **DNA Pol III** | Resynthesizes excised region |
| **DNA Ligase** | Seals final nick |

### Strand Discrimination — The Clever Part

**Problem**: How does the cell know which strand has the error?

**Solution**: **Dam Methylation**
- Dam methylase methylates adenine in GATC sequences (genome-wide)
- Timing: parental strand fully methylated; new strand is **transiently hemimethylated** after replication
- MutH recognizes hemimethylated GATC and nicks **unmethylated strand** (the new one)
- This ensures removal of the error-prone new strand

**Timeline**:
```
Replication Fork
    ↓
New strand synthesized (unmethylated GATC initially)
    ↓
Parental strand (fully methylated GATC)
    ↓
MutH scans for hemimethylated GATC
    ↓
Nicks unmethylated adenine (new strand)
    ↓
Exonuclease I removes new strand (5'→3')
    ↓
Pol III resynthesizes; Ligase seals
    ↓
Dam methylase methylates new strand (now mature)
```

### Eukaryotic MMR (Different Mechanism)

- Uses **PCNA** (processivity clamp) instead of methylation
- PCNA encircles DNA; the 3' end of the strand being synthesized is more exposed
- MutSα (MSH2/MSH6) recognizes mismatch; recruits MLH1/MLH3
- MLH1 has endonuclease activity; nicks strand containing 3' end or strand discontinuities

---

## PATHWAY 2: NUCLEOTIDE EXCISION REPAIR (NER)

### What It Repairs
- **Thymine dimers** (from UV light)
- **Bulky adducts** (chemicals, oxidized bases)
- Any lesion causing significant DNA distortion

### Key Enzymes & Mechanism

**Discovery**: Hans Kraemer, 1970s; won Nobel Prize

**Enzyme Complex**:

| Protein | Role |
|---------|------|
| **UvrA** | ATPase; scans DNA for distortion |
| **UvrB** | Binds to lesion; verifies distortion; remains bound |
| **UvrC** | Endonuclease; makes two incisions (5' and 3' of lesion) |
| **UvrD** | Helicase II; unwinds and removes oligonucleotide |
| **DNA Pol I** | Fills gap; also has 5'→3' exonuclease to remove damaged nucleotide |
| **DNA Ligase** | Seals final nick |

### Step-by-Step Mechanism

**Step 1: Recognition**
- UvrA (dimer) scans DNA using ATP
- UvrB joins; complex continues scanning
- Upon lesion (distortion), UvrB undergoes conformational change; remains bound
- UvrA dissociates

**Step 2: Dual Incision**
- UvrC arrives at UvrB
- UvrC makes two incisions:
  - 5' incision: ~5 nucleotides 5' of lesion (on 5' side of distortion)
  - 3' incision: ~8 nucleotides 3' of lesion (on 3' side)
  - **Total removed**: 12–13 nucleotides

**Step 3: Removal**
- UvrD (helicase) unwinds the oligonucleotide from 5' incision site
- Oligonucleotide (with lesion) dissociates

**Step 4: Resynthesis**
- DNA Pol I fills 12–13 nt gap
- Pol I also has 5'→3' exonuclease; removes damaged nucleotide at 5' end while filling

**Step 5: Ligation**
- DNA Ligase seals nick between new DNA and parental strand

### UV Damage: Thymine Dimer Formation

```
Normal:              After UV (254 nm):
Thy---Thy            Thy=Thy (covalent cyclobutane ring)
  |   |
DNA   DNA
```

**Consequence**:
- Distorts DNA helix
- Blocks RNA Polymerase → no transcription
- Blocks DNA Polymerase → no replication
- **Lethal unless repaired**

### Eukaryotic NER (TFIIH Complex)

- Transcription-coupled repair: TFIIH recognizes stalled RNA Pol II at lesion
- XPA, XPB, XPD, XPE, XPF nucleases perform similar dual incision
- Larger excision: 25–32 nucleotides (vs. bacterial 12–13)
- Mutations in human XPA–XPG → Xeroderma Pigmentosum (extreme UV sensitivity, skin cancer)

---

## PATHWAY 3: BASE EXCISION REPAIR (BER)

### What It Repairs
- **8-oxoguanine** (oxidation product)
- **Uracil** (from cytosine deamination or dUMP incorporation)
- **Thymine glycol** (from UV-induced oxidation)
- **Alkylated bases** (from chemical mutagens)
- **Abasic sites** (AP sites from base loss)

### Key Enzymes

| Step | Enzyme | Action |
|------|--------|--------|
| **1. Base Recognition & Removal** | DNA glycosylase (base-specific) | Recognizes damaged base; cleaves N-glycosidic bond → AP site |
| **2. AP Site Cleavage** | AP endonuclease (APE1) | Cuts backbone 5' to AP residue; leaves 3'-OH & 5'-deoxyribose |
| **3a. Short-Patch** | DNA Pol I | Removes AP residue + adds 1 nt; Ligase seals |
| **3b. Long-Patch** | DNA Pol δ | Adds multiple nt; Flap endonuclease (FEN1) removes 5' flap |
| **4. Ligation** | DNA Ligase | Seals final nick |

### Glycosylase Specificity

**Uracil DNA Glycosylase (UDG)**:
- Removes uracil opposite adenine
- Also recognizes mismatches (C-uracil from deamination)

**8-oxoguanine Glycosylase (OGG1)**:
- Removes 8-oxoG (oxidized guanine)
- Prevents mispairing of 8-oxoG with adenine

**Thymine Glycol Glycosylase**:
- Removes thymine glycol (from UV-induced oxidation)

### Two Sub-Pathways

**Short-Patch BER** (~80% of cases):
- Pol I removes damage + adds 1 replacement nucleotide
- Quick; limited scope

**Long-Patch BER** (~20% of cases):
- When damage affects multiple nucleotides or AP site structure
- Pol δ adds multiple nucleotides past lesion
- FEN1 "flips out" and cleaves 5' flap structure
- More thorough

---

## PATHWAY 4: DOUBLE-STRAND BREAK (DSB) REPAIR

### Two Main Routes

```
      DSB (Double-Strand Break)
         ↙        ↘
   Homologous    Non-Homologous
   Recombination  End Joining
   (accurate)     (error-prone)
   [Requires          [Direct
    template]          ligation]
```

### Route A: Homologous Recombination (HR)

**Requirements**:
- Homologous DNA template (sister chromatid, homolog, or duplicate region)
- RecBCD complex, RecA, RuvAB, RuvC

**RecBCD Pathway** (Primary in *E. coli*):

**Step 1: Recognition**
- RecBCD complex binds broken DNA end
- RecB: 3'→5' helicase + nuclease
- RecC: chi site recognition protein
- RecD: 5'→3' helicase

**Step 2: Processing & Chi Recognition**
- RecBCD unwinds and degrades dsDNA in 3'→5' direction
- Upon encountering **Chi site** (5'-GCTGGTGG-3'):
  - RecC detects Chi
  - Nuclease activity **switches**
  - Complex now generates 3' **single-stranded DNA tail** (~10 kb)

**Step 3: RecA Loading**
- RecA protein coats 3' ssDNA tail (ATP-dependent)
- Forms nucleoprotein filament (RecA*)
- Filament performs homology search in dsDNA

**Step 4: Strand Invasion**
- RecA-ssDNA scans dsDNA
- Upon finding homologous sequences, invades duplex
- 3' end of invading strand primes DNA synthesis
- Creates **D-loop** (displacement loop)

**Step 5: DNA Synthesis & Resolution**
- DNA Pol III extends invading 3' end
- **RuvAB** complex binds Holliday junction (motor protein activity)
- **RuvC** endonuclease cleaves Holliday junctions
  - Two cleavage options:
    - **Crossover products**: Results in genetic recombination
    - **Patch products**: Results in non-crossover

### Route B: Non-Homologous End Joining (NHEJ)

- Direct, template-independent ligation of broken ends
- Error-prone; often deletes small sequences at break point
- More prevalent in eukaryotes (Ku70/Ku80 complex)
- Rare in *E. coli*; used only if HR fails

---

## PATHWAY 5: THE SOS RESPONSE (Emergency Mode)

### Trigger: DNA Damage Detection

**Stimulus**: Single-stranded DNA (ssDNA)
- From stalled replication forks (replication polymerase blocked by lesion)
- From unrepaired damage
- Recognized by RecA protein

### Mechanism

**Step 1: RecA Activation**
- RecA binds ssDNA
- Undergoes conformational change → **RecA*** (activated form)
- Can now interact with LexA repressor

**Step 2: LexA Autocleavage**
- RecA* stimulates LexA (repressor protein) to self-cleave
- Uses intrinsic serine protease activity
- LexA normally represses ~40 SOS genes

**Step 3: SOS Gene Derepression**
As LexA levels drop, SOS genes transcribed:

| Gene Class | Examples | Function |
|------------|----------|----------|
| **DNA Repair** | *recF*, *recN*, *recO*, *uvrA*, *uvrB*, *uvrC*, *polB* | Recombination, NER, other repairs |
| **Error-Prone Polymerases** | *umuDC* (Pol V), *dinB* (Pol IV) | **Bypass lesions** (G:C → A:T or C:G) |
| **Mutagenic Recombination** | *recA*, *recF*, *recO*, *recR* | Enhanced recombination |
| **Transposases** | *tnpA*, *tnpR* | Transposon mobilization |
| **Nucleotide Salvage** | *dnaB*, *dnaK*, *groES* | Support replication/repair machinery |

### Transient Mutagenesis

**Key insight**: Cells accept increased mutation rate to survive otherwise lethal damage.

**Error-Prone Polymerases**:
- **Pol V** (*umuDC*): Bypasses many lesions but low fidelity; makes errors ~10^-1 (vs. Pol III ~10^-10)
- **Pol IV** (*dinB*): Similar low fidelity

**Consequence**:
- Transient 100–1000× increase in mutation rate
- Most mutations deleterious; some increase fitness
- Evolutionary advantage (in population, some cells gain beneficial mutations)

### Recovery & Shutdown

- Upon repair of damage: ssDNA disappears
- RecA* reverts to inactive RecA
- LexA synthesis (no longer repressed) accumulates
- LexA re-represses SOS genes
- Mutagenesis stops

---

# MODULE 3: RECOMBINATION & MAPPING

## The Holliday Model of Homologous Recombination

### Historical Context
Robin Holliday, 1964: Proposed symmetrical model for meiotic recombination; applies to mitotic and bacterial recombination.

### Key Structure: The Holliday Junction

**4-way branch point**: Two homologous DNA molecules connected at single point; strands cross over.

```
        Strand from Molecule 1
               ↗  ↖
        ─── A ╱    ╲ B ───
            ╲     ╱
             ╲   ╱
              ╲ ╱
          Holliday
          Junction
              ╱ ╲
             ╱   ╲
            ╱     ╲
        ─── a ╱    ╲ b ───
               ↙  ↘
   Strands from Molecule 2 (homologous)

Read as: A and a on top/bottom; B and b on left/right (rough diagram)
```

### Steps of Homologous Recombination

#### Step 1: Strand Breakage & Invasion
- Single-strand nick (or DSB) initiates in one molecule
- Invading strand displaces complementary strand
- Creates **D-loop** (displacement loop)

#### Step 2: Strand Extension
- Invading 3' end primes DNA synthesis
- DNA polymerase extends invading strand using template

#### Step 3: Branch Migration
- Holliday junction moves along DNA
- Displacement of complementary strands
- Can migrate hundreds or thousands of bp
- Allows **heteroduplex DNA formation** (mismatched bases at polymorphic sites)

#### Step 4: Mismatch Correction (Optional)
- Heteroduplex regions contain mismatches (from natural polymorphisms or mutations)
- Mismatch repair can "correct" either allele
- Leads to **gene conversion** (non-reciprocal transfer)

#### Step 5: Holliday Junction Resolution
- **RuvC** endonuclease recognizes and cleaves Holliday junction
- **Two cleavage options**:

```
OPTION 1: Horizontal cut (one pair of opposite strands)
→ Non-crossover (patch) product: sister chromatids recombined locally; no crossover at outer markers

OPTION 2: Vertical cut (orthogonal pair of opposite strands)
→ Crossover product: Recombined; outer markers traded between chromatids
```

---

## Gene Conversion & Non-Reciprocal Recombination

### Definition
One DNA sequence "corrected" to match another in heteroduplex DNA.

### Mechanism
During branch migration, heteroduplex forms. If polymorphism exists (e.g., A on one side, a on other):

```
Heteroduplex:
  5'─── A ───3'
         |  (mismatch, e.g., A-a)
  3'─── a ───5'

Mismatch repair acts on A-a pair; can "correct" to:
  A-A (converted to A allele) OR
  a-a (converted to a allele)

Result: Non-Mendelian segregation (3:5 or 5:3 instead of 4:4 in meiosis)
```

### Observable in Meiosis
- **4:4 ratio**: Normal (no gene conversion)
- **3:5 or 5:3 ratio**: Gene conversion (biased repair toward one allele)
- Can track which allele is "converting" (suggests specific repair pathway preference)

---

## Mapping by Recombination Frequency

### Principle
Frequency of recombination between two loci is proportional to distance.

### Basic Calculation

```
Testcross: A B / a b (heterozygote) × a b / a b (homozygous recessive)

Progeny observed:
  A B (parental): 450
  a b (parental): 430
  A b (recombinant): 35
  a B (recombinant): 40

Total: 955

Recombination Frequency (RF) = (# recombinants / total) × 100%
                              = (35 + 40) / 955 × 100%
                              = 75 / 955 × 100%
                              ≈ 7.9%
                              ≈ 8 map units (m.u.) or centiMorgans (cM)

Interpretation: Genes are ~8 m.u. apart
```

### Multiple Crossovers & Interference

**In three-point crosses** (3 linked genes), determine:

1. **Parental class**: Most frequent classes
2. **Double crossover (DCO) class**: Rarest classes (crossover in both intervals)
3. **Gene order**: Single crossover between outer genes determines middle gene
4. **Coefficient of Coincidence (COC)**: Observed DCO / Expected DCO
5. **Interference**: 1 - COC (measures inhibition of second crossover by first)

---

## Hfr Mapping (Interrupted Mating)

### Context: Hfr Strains

**Hfr** (High frequency recombination): F plasmid integrated into bacterial chromosome.

### Hfr × F- Mating

**Key process**:
1. Hfr initiates chromosome transfer from integrated **oriT**
2. Chromosome transfers **linearly**, single-strand
3. Genes enter F- recipient in predictable **time order**
4. Mating usually interrupted before complete transfer

### Time of Entry (TOE) Mapping

```
Hfr Origin            oriT
  ↓
  ├─ 5 min ─┤ gal+ ├─ 7 min ─┤ lac+ ├─ 6 min ─┤ trp+ ├─→
  0 min                  5 min           12 min           18 min

Time of Entry:
  gal+ enters at 5 min
  lac+ enters at 12 min (7 min after gal+)
  trp+ enters at 18 min (6 min after lac+)

Map Distance:
  gal to lac = 7 m.u.
  lac to trp = 6 m.u.
  gal to trp = 13 m.u.
```

### Experimental Procedure

1. **Mating**: Hfr × F- in liquid medium
2. **Timed Interruption**: At intervals (1, 2, 5, 10, 15, 20 min), interrupt mating (e.g., by vigorous agitation)
3. **Selection**: Plate on medium selecting for F- markers (e.g., *lac-* selected, looking for *lac+* recombinants from Hfr)
4. **Graph**: Plot time of entry vs. frequency of recombinants

### Advantages
- **Linear transfer** → clear gene order
- **Temporal separation** → determines distance
- Can map hundreds of genes quickly

---

# MODULE 4: HORIZONTAL GENE TRANSFER

## Overview: Three Main Mechanisms

```
       HORIZONTAL GENE TRANSFER
              (HGT)
        ↙       ↓       ↘
    Transformation  Transduction  Conjugation
      (naked DNA)   (via phage)    (direct transfer)
        │            ├─ Generalized
        │            │  (any genes)
        │            └─ Specialized
        │               (genes near prophage)
        │
    No mechanism needed;
    cell absorbs DNA
    from environment
```

---

## MECHANISM 1: TRANSFORMATION

### Definition
Uptake of naked DNA from environment.

### Requirements
1. **Competence**: Ability to take up DNA
   - Natural: Some species (*Streptococcus*, *Vibrio*, *Bacillus*, *Haemophilus*)
   - Artificial: CaCl₂-treatment, electroporation

2. **DNA**: ssDNA or dsDNA available

3. **Competence Proteins**: ComE, ComD, ComF, ComG (species-specific)

### Process

```
1. DNA Binding:
   DNA encounters cell surface competence proteins (ComE, ComD)

2. Single-Strand Import:
   One strand imported into cell
   Complementary strand degraded (or exported)

3. Protection:
   ssDNA protected from nucleases inside cell

4. Chromosomal Integration:
   RecA-mediated homologous recombination into chromosome
   OR
   Circularization as plasmid (if all replication genes present)
```

### Efficiency
- Typically low: 0.1%–1% of treated cells take up DNA
- Higher in naturally competent species
- Depends on: DNA size, fragment length, homology

### Griffith Experiment (1928) — Classic Proof

***Streptococcus pneumoniae*—Two Forms**:

| Form | Capsule | Colony | Virulence |
|------|---------|--------|-----------|
| **S (Smooth)** | Present | Smooth | High (kills mice) |
| **R (Rough)** | Absent | Rough | Low (mice survive) |

**Experimental Results**:

```
Group 1: Live S + Live R → Mice die; S recovered from blood
Group 2: Heat-killed S + Live R → Mice survive
Group 3: Live R alone → Mice survive
Group 4: Heat-killed S alone → Mice survive
Group 5: Heat-killed S + Live R (with DNase) → Mice survive

CONCLUSION: "Transforming principle" (later identified as DNA)
from heat-killed S transformed R to S phenotype.
Heat-killed S's DNA can transform living R cells.
```

---

## MECHANISM 2: TRANSDUCTION

### Definition
Bacterial DNA transfer **via bacteriophage** vector.

### Type A: Generalized Transduction

**Occurs with**: Lytic phages (e.g., P1, P22 in *Salmonella*)

**Mechanism**:

```
1. Lytic phage infects cell; replicates vigorously
2. Phage DNA + host DNA fragmented
3. Phage head packaging machinery randomly packages:
   - Correctly: Phage DNA (~10 m.u. size)
   - Incorrectly: Adjacent bacterial DNA (same size) → NO phage genes
4. Transducing particle released
5. Particle infects new cell; injects bacterial DNA
6. Bacterial DNA integrates (if homologous) or circularizes
```

**Characteristics**:
- **Any genes** can be transduced (equal probability)
- Frequency: ~1 per 10^6 phage particles
- **Abortive transduction**: Transduced DNA not integrated → unstable (diluted out)
- **Stable transduction**: Integration via recombination OR circularization (if it replicates)

### Type B: Specialized Transduction

**Occurs with**: Temperate phages (e.g., lambda integrating into *E. coli*)

**Mechanism**:

```
1. Lambda integrated as prophage between gal and bio genes

2. Normal excision: Prophage excises precisely
   → releases lambda DNA
   → host chromosome intact

3. Aberrant excision (RARE):
   Excises at one att site normally
   BUT at wrong site on other end
   → takes adjacent BACTERIAL genes (gal or bio)
   → leaves behind PHAGE genes
   → produces DEFECTIVE phage carrying gal or bio

4. Example: λdgal (lambda defective in gal)
   Carries gal+ genes; missing essential phage genes
   Can only replicate if co-infected with helper phage (wild-type lambda)
```

**Characteristics**:
- **Only genes adjacent to integration site** transduced
- Phage carries both **phage AND bacterial DNA**
- Requires **helper phage** for replication
- Frequency: ~1 per 10^4–10^5 phage (rarer than generalized)

**Uses**:
- Gene mapping (which genes are transduced together = located together)
- Strain construction (introduce specific genes via helper phage)

---

## MECHANISM 3: CONJUGATION

### F Plasmid — The Fertility Factor

**Size**: ~100 kb

**Genes**:
- **tra genes** (transfer): pilus proteins, coupling factors, ATPases
- **ori**: Origin of replication
- **oriT**: Origin of transfer (single-strand nick site)

### F+ (Donor) × F- (Recipient) Mating

**Process**:

```
1. F+ cell produces pilus (coded by tra genes)
2. Pilus extends and contacts F- cell
3. Pilus retracts; cells come together via mating pair stabilization
4. DNA transfer channel forms
5. Rolling Circle Replication at oriT:
   - Single strand nicked at oriT
   - Nicked 3' end primes synthesis
   - As new strand synthesizes, old strand unwinds and is transferred
6. Complementary strand synthesized in:
   - Donor (replaces transferred strand)
   - Recipient (as incoming strand transferred)
7. Both donor and recipient become F+

Time: ~100 minutes for complete transfer
Efficiency: Very high (~100% of F+ pairs if mating undisturbed)
```

### Hfr (High Frequency Recombination) × F- Mating

**Key Difference**: F plasmid **integrated into chromosome**

**Process**:

```
1. Hfr initiates transfer from integrated oriT
2. Chromosome transfers **linearly**:
   - Genes nearest oriT enter first
   - Genes farther away enter later (in time-dependent order)
3. Mating usually **interrupted** before complete transfer (~12 min for first markers)
4. Recipient: F- merodiploid (partial diploid) for transferred genes
   - Can express Hfr alleles temporarily
   - Recombination determines stability
```

**Result**:
- Most recipients remain F- (F plasmid not transferred; DNA is)
- Some can become F+ if mating continues until integrated F reaches end

### F' (F-prime) — Plasmid Carrying Bacterial Genes

**Origin**: Aberrant excision of integrated F from Hfr

**Example**: F' (*lac*+) carries *lac* genes on F plasmid

**Uses**:
- **Complementation testing**: F' (*lac*+) / *lac*- (on chromosome) → diploid for region
- **Dominant/recessive testing**: F' carries wild-type or mutant alleles

**Stability**: Plasmid replication → stable inheritance (unlike Hfr merodiploid)

---

## Summary: Which Mechanism for Genetic Analysis?

| Task | Best Mechanism | Why |
|------|----------------|-----|
| Map genes | **Hfr interrupted mating** | Linear transfer; time indicates distance |
| Identify linked genes | **Generalized transduction** | Co-transduced genes are linked |
| Introduce specific genes | **Transformation** or **Specialized transduction** | Precise control |
| Create merodiploids | **F' conjugation** | Stable partial diploid |
| Broad survey of genome | **Generalized transduction** | Any genes can be transduced |

---

# MODULE 5: MOLECULAR TECHNIQUES

## TECHNIQUE 1: RESTRICTION ENZYMES

### What They Are
Bacterial **endonucleases** that recognize specific DNA sequences and cut.

### Discovery & Function
- Bacteria use as defense against foreign DNA (restriction-modification system)
- Bacteria methylate own recognition sites (modification) → protect from self-cleavage
- First discovered in *E. coli* RY13 (EcoRI); revolutionized molecular biology

### Palindromic Recognition Sequences

**Key principle**: Most restriction sites are **palindromic** (read same 5'→3' on both strands)

```
EcoRI recognizes: 5'-G A A T T C-3'
                  3'-C T T A A G-5'

Read 5'→3' on top: G A A T T C
Read 5'→3' on bottom: C T T A A G → Reverse = G A A T T C ✓ PALINDROME!
```

### Cutting Patterns: Sticky vs. Blunt

**Sticky Ends** (Cohesive Ends):
- Offset cut → single-stranded overhangs
- Example (EcoRI):
  ```
  5'─── G        A A T T C ───3'
  3'─── C T T A A        G ───5'
        ↑           ↑
      These 4 nt overhangs are sticky; can base-pair with complementary overhangs
  ```
- Advantage: Easy ligation (overhangs hold pieces together); specific association

**Blunt Ends**:
- Straight cut across both strands
- Example (PvuII):
  ```
  5'─── CA G CT G ───3'
  3'─── G T C GA C ───5'
           ↑↑ (both cut here)
  No overhangs; strands are flush
  ```
- Disadvantage: Hard to ligate (no base pairing to hold pieces); non-specific
- Advantage: Can ligate any blunt ends together

### Common Restriction Enzymes

| Enzyme | Source | Recognition Seq | Cut Pattern | Overhang Size |
|--------|--------|-----------------|-------------|---------------|
| **EcoRI** | *E. coli* K12 | GAATTC | G^AATTC | 4 nt 5' (sticky) |
| **BamHI** | *Bacillus amyloliquefaciens* | GGATCC | G^GATCC | 4 nt 5' (sticky) |
| **PstI** | *Providencia stuartii* | CTGCAG | CTGCA^G | 3 nt 3' (sticky) |
| **PvuII** | *Proteus vulgaris* | CAG^CTG | CAG^CTG | Blunt |
| **HaeIII** | *Haemophilus aegyptius* | GG^CC | GG^CC | Blunt |
| **SalI** | *Streptomyces albus* | GTCGAC | G^TCGAC | 4 nt 5' (sticky) |
| **NotI** | *Nocardia otitidiscaviarum* | GCGCGC | GC^GCGC | 5 nt 5' (sticky) |

### Restriction Mapping

**Goal**: Determine order and distance of restriction sites.

**Method**:
1. Digest DNA with single restriction enzyme → fragments
2. Measure fragment sizes (gel electrophoresis)
3. Digest with different enzymes singly and in combination
4. Compare patterns; deduce map by analyzing overlaps

**Example**:
```
Digest with EcoRI: 4 kb, 6 kb (total 10 kb)
Digest with BamHI: 3 kb, 7 kb
Digest with EcoRI + BamHI: 2 kb, 2 kb, 1 kb, 5 kb

Analysis:
- EcoRI cuts at positions 4 and 10 (circular plasmid)
- BamHI cuts at position 3
- Double digest: fragments 0-2 (2kb), 2-3 (1kb), 3-4 (1kb), 4-10 (6kb)
  Wait, let's recalculate...
  [Typically requires careful deduction with all three digests]

Final map (example):
  EcoRI ──4 kb── BamHI ──3 kb── EcoRI
  (Position 0)  (at 4)  (at 7)   (at 10, circular)
```

---

## TECHNIQUE 2: DNA CLONING & RECOMBINANT DNA

### General Strategy

```
Step 1: Choose vector (plasmid, cosmid, or phage) and insert DNA
Step 2: Digest both vector and insert with same restriction enzyme
Step 3: Mix; DNA ligase seals nicks
Step 4: Introduce into bacterial host (transformation, transduction, conjugation)
Step 5: Select recombinant clones
Step 6: Analyze, propagate, or express insert
```

### Vectors & Their Features

**Plasmid**:
- Small (~5–10 kb), can carry inserts up to ~15 kb
- Features:
  - **ori** (origin of replication): Low, medium, or high copy number
  - **Selectable marker**: Antibiotic resistance (amp^R, tet^R, kan^R)
  - **Cloning site**: Multiple restriction sites (MCS, polylinker)

**Cosmid**:
- Large (up to 45 kb inserts)
- Combination of plasmid + phage lambda sequences
- Requires *in vitro* packaging into lambda heads

**Bacteriophage Lambda (λ)**:
- Can carry inserts up to 20 kb
- Requires helper phage for replication (if essential genes deleted)
- Higher insert capacity than plasmids

### Blue-White Screening (*lacZ* System)

**Principle**: Insertional inactivation of *lacZ* gene

**Setup**:
1. Vector contains *lacZ* gene (encodes β-galactosidase)
2. Cloning site is within *lacZ*
3. Medium contains X-gal (substrate for β-galactosidase) + IPTG (inducer)

**Results**:
- **White colonies**: *lacZ* disrupted (insert present) → no β-galactosidase → no color
- **Blue colonies**: *lacZ* intact (no insert) → β-galactosidase produced → hydrolyzes X-gal → blue color

---

## TECHNIQUE 3: PCR (POLYMERASE CHAIN REACTION)

### Historical Context
**Kary Mullis**, 1983. Revolution in molecular biology. Nobel Prize 1993.

### Principle: Exponential Amplification

After n cycles: DNA ≈ 2^n × (initial DNA)

Example: Start with 1 DNA molecule
- After 20 cycles: 2^20 ≈ 10^6 copies
- After 30 cycles: 2^30 ≈ 10^9 copies

### Requirements

1. **Template DNA**: Even a single copy (or contaminating DNA)
2. **Two Primers**: Oligonucleotides (18–25 nt), homologous to target flanking sequences
3. **dNTPs**: All four deoxynucleotides (dATP, dCTP, dGTP, dTTP)
4. **Thermostable DNA Polymerase**: *Taq* polymerase (from *Thermus aquaticus*, survives 94°C)
5. **Buffer & Salts**: Optimized for Taq enzyme
6. **Thermal Cycler**: Switches temperatures for denaturation, annealing, extension

### The Three-Step Cycle (Repeated 25–40 Times)

**Step 1: Denaturation (94–95°C, 20–30 sec)**
- Double-stranded DNA melts → single-stranded DNA
- Heat breaks hydrogen bonds

**Step 2: Annealing (50–65°C, 20–60 sec)**
- Temperature lowered (typically: Tm - 5°C, where Tm = primer melting temperature)
- Primers anneal to complementary sequences on template strands
- **Both forward and reverse primers** bind (flanking target region)

**Step 3: Extension (72°C, varies by insert size)**
- *Taq* polymerase extends from primer 3' end
- Synthesizes new strand using template strand (3'→5' direction on template)
- Rate: ~1000 nt/sec (so 1 kb insert ≈ 1 min)
- Both forward and reverse primers extended simultaneously

### Primer Design

**Sequence Design**:
- 18–25 nucleotides long
- Flanks target region on opposite strands
- Forward primer: 5'→3', homologous to sense strand
- Reverse primer: 5'→3', homologous to antisense strand (actually reverse complement)

**Melting Temperature (Tm)**:
- Rough formula: Tm = 4(G+C) + 2(A+T)
- More accurate: Tm = 64.9 + 41 × (G+C - 16.4)/(A+T+G+C)
- Typical Tm: 50–65°C

**Primer Specificity**:
- Should not be self-complementary (no hairpins)
- Should not form primer-dimers (forward + reverse binding to each other)
- Should not be highly repetitive in genome (would bind multiple sites)

### Cycle Efficiency & Plateau Effect

**Ideal**: Doubles with each cycle (2^n amplification)

**Reality**:
- Early cycles: Efficient doubling
- Later cycles: Plateau effect
  - dNTPs depleted
  - Polymerase slows
  - Primers compete with accumulated DNA
  - Efficiency drops below doubling
- Typical maximum: 25–35 useful cycles (further cycling adds little)

### Applications

1. **Gene Amplification**: For cloning, expression studies
2. **Diagnostics**: qPCR to detect pathogens (COVID-19, malaria, etc.)
3. **Mutation Detection**: Amplify region, sequence, or digest for known mutations
4. **Copy Number Variation (CNV)**: qPCR with internal controls
5. **Forensics**: Amplify short tandem repeats (STRs) from small DNA samples
6. **Gene Expression**: RT-PCR (reverse transcription then PCR of mRNA)

---

## TECHNIQUE 4: SANGER SEQUENCING (CHAIN-TERMINATION METHOD)

### Historical Context
**Frederick Sanger**, 1977. First method to sequence DNA. Nobel Prize 1980 (second Nobel for Sanger).

### Principle: ddNTPs Block Synthesis

**ddNTP** (dideoxyribonucleoside triphosphate):
- Lacks the 3'-OH group (unlike dNTPs)
- When incorporated, prevents addition of next nucleotide
- Chain termination

### Chemical Difference

```
dNTP:                      ddNTP:
    5'-triphosphate            5'-triphosphate
        ↓                           ↓
    3'-OH present            3'-H (no OH) ← KEY DIFFERENCE
        ↓                           ↓
    Can chain extend          CANNOT chain extend
    to next nucleotide        (chain terminates)
```

### Experimental Procedure

**Step 1: Prepare Reaction Mix**
- Single-stranded template DNA (unknown sequence to read)
- Primer (oligonucleotide, immediately 5' to region of interest)
- DNA polymerase (usually Klenow fragment, or modern modified polymerase)
- **dNTPs** (high concentration, ~100 µM each)
- **ddNTPs** (low concentration, ~1 µM each, fluorescently labeled)
  - Each ddATP, ddCTP, ddGTP, ddTTP has different color label
- Buffer

**Step 2: Primer Annealing & Extension**
- Denature template to ssDNA
- Anneal primer (provides 3'-OH for polymerase)
- Polymerase begins extending from primer
- For each position: randomly incorporates either dNTP (99%) or ddNTP (1%)

**Step 3: Chain Termination**
- If ddNTP incorporated: chain stops (no 3'-OH for next nucleotide)
- If dNTP incorporated: continues to next position
- Result: Population of DNA fragments of varying lengths, each terminating with one labeled ddNTP

```
Template:    5'─── A T G C T A ───3'
Primer:      3'───         ←──5' (annealed here; arrow = 3'→5' direction of synthesis)

Synthesis:
Position 1: G incorporated (dNTP) → continues
Position 2: C incorporated (dNTP) → continues
Position 3: 50% chance ddC incorporated → terminates; fragment: primer + G + C + ddC
            OR dC incorporated (dNTP) → continues
...and so on

Result: Mixture of fragments:
  primer + G + ddC (terminator after position 2)
  primer + G + C + ddG (terminator after position 3)
  primer + G + C + G + ddA (terminator after position 4)
  ... every possible termination point ...
```

### Fragment Separation & Detection

**Traditional (Slab Gel Electrophoresis)**:
- Load mixture on polyacrylamide gel
- Run at high voltage (separates by size)
- Radioactive label on ddNTPs detected by autoradiography
- Read sequence from bottom (smallest) to top (largest)

**Modern (Capillary Electrophoresis)**:
- Load into capillary tube
- Apply electric field
- Fragments separate by size
- Fluorescence detector scans as each fragment passes
- Reads label (color) for each fragment
- Sequence generated automatically (5'→3' from first to last fragment)

### Accuracy & Read Length

- **Accuracy**: ~99.9% per base
- **Read length**: 500–1000 bp per reaction (depends on template quality, polymerase)
- **Why limited length?**:
  - Long ssDNA templates form secondary structures
  - Polymerase slows with longer extension
  - ddNTP incorporation becomes uneven at distance
  - Signal-to-noise ratio decreases

### Advantages vs. Disadvantages

**Advantages**:
- Highly accurate
- Widely available
- Robust; works well for most templates
- Inexpensive per reaction

**Disadvantages**:
- Low throughput (thousands of reads, not millions)
- Limited read length
- Requires single-stranded template (or separation)
- GC-rich regions can cause problems (secondary structure)

---

## TECHNIQUE 5: qPCR (QUANTITATIVE/REAL-TIME PCR)

### What It Measures
**Real-time amplification** monitoring (not just endpoint detection)

### Key Advantage
Allows **quantification** of starting DNA (standard PCR only gives endpoint)

### How It Works

**Fluorescent Reporter**:
- SYBR Green: Intercalates into dsDNA; fluorescence increases as DNA accumulates
- TaqMan Probes: Oligonucleotide probe + quencher; fluorescence released upon cleavage during extension

**During Each Cycle**:
- Polymerase extends primer
- dsDNA accumulates
- Fluorescence increases (measured in real-time)
- Threshold cycle (Ct): The cycle at which fluorescence exceeds background

**Quantification**:
- Ct inversely correlates with starting DNA amount
- Compare unknown sample's Ct to standard curve
- Can determine original DNA concentration

### Applications

1. **Copy Number Variation (CNV)**
2. **Gene Expression** (with reverse transcription: RT-qPCR)
3. **Pathogen Detection** (faster than traditional PCR + gel)
4. **Quality Control** (verify successful cloning, amplification)
5. **Mutation Detection** (if mutation alters Tm or probe hybridization)

---

## TECHNIQUE 6: OTHER MOLECULAR TECHNIQUES (Brief Overview)

### DNA Gel Electrophoresis
- Separate DNA by size
- Applied voltage; DNA migrates through agarose gel matrix
- Smaller fragments move faster/farther
- Visualize with ethidium bromide (intercalates, fluoresces under UV)

### Southern Blot
- Digest DNA with restriction enzymes
- Separate on gel
- Transfer to nitrocellulose/nylon membrane (blot)
- Hybridize with labeled probe (specific sequence)
- Detect hybridized bands
- Useful for: Detecting specific sequences, determining copy number, identifying restriction polymorphisms

### DNA Ligation
- DNA ligase catalyzes phosphodiester bond formation
- Seals nicks between DNA fragments
- Requires: ATP (or NAD+ for some ligases), intact 3'-OH and 5'-phosphate

### Cloning Strategies

**TA Cloning**:
- PCR polymerase (*Taq*) adds single dA to 3' end of product
- Vector has dT overhangs
- A-T pairing stabilizes insert
- No need for specific restriction sites

**TOPO Cloning**:
- Topoisomerase nicked into vector DNA; catalyzes ligation
- Fast, efficient

**Gateway Cloning**:
- Site-specific recombination using phage att sites
- Efficient for cloning multiple inserts

---

# STUDY STRATEGIES & EXAM TIPS

## High-Yield Topic Hierarchy

### MUST KNOW (Likely on Exam)

1. **MMR Mechanism**
   - Dam methylation → hemimethylation
   - MutH recognizes unmethylated strand
   - Exonuclease I removes; Pol III resynthesizes

2. **RecBCD + Chi Site**
   - DNA degradation until Chi site
   - Nuclease switches to generate 3' ssDNA tail
   - RecA loads on ssDNA

3. **Hfr Mapping (Time of Entry)**
   - Linear chromosome transfer
   - Time indicates gene order and distance
   - Interrupted mating procedure

4. **PCR Fundamentals**
   - Three-step cycle (denature, anneal, extend)
   - Primer design (Tm, specificity)
   - Exponential amplification (2^n)

5. **Sanger Sequencing Mechanism**
   - ddNTPs lack 3'-OH
   - Chain termination at every position
   - Separation by size; fluorescent detection

6. **Holliday Junction Resolution**
   - RuvC cleaves; two options (crossover vs. patch)
   - Gene conversion from mismatch repair during branch migration

### SHOULD KNOW (Probable)

1. NER pathway (dual incision, 12-13 nt excision)
2. SOS response (RecA*, LexA, error-prone polymerases)
3. Luria-Delbrück fluctuation test (variance analysis)
4. Transformation & Griffith experiment
5. Conjugation (F+, Hfr, time of entry)
6. Restriction enzyme recognition & sticky ends

### NICE TO KNOW (Lower Probability)

1. BER pathway (glycosylase types)
2. Specialized transduction (defective phage)
3. qPCR quantification method
4. Blue-white screening details
5. Poisson distribution (MOI calculations)

---

## Common Exam Question Types & How to Answer

### TYPE 1: Mechanism Questions
**Format**: "Describe the steps of MMR in *E. coli*."

**Answer Strategy**:
1. List all enzymes/proteins involved
2. Walk through each step (1, 2, 3...)
3. Explain the role of each enzyme
4. Include the chemical outcome (what's being removed/repaired)
5. Mention the importance of strand discrimination if relevant

**Example Answer Structure**:
- Enzyme/protein name → Action → Result
- "MutS recognizes mismatch → recruits MutL → signals MutH → MutH nicks hemimethylated GATC → Exonuclease I removes new strand → Pol III resynthesizes → Ligase seals."

---

### TYPE 2: Comparative Questions
**Format**: "How does NER differ from BER?"

**Answer Strategy**:
Create a comparison table:

| Feature | NER | BER |
|---------|-----|-----|
| Damage | Large lesions (TT dimers, bulky) | Small lesions (oxidation, deamination) |
| Recognition | UvrA/UvrB (distortion) | Glycosylase (base-specific) |
| Excision Size | 12-13 nt | 1-2 nt (short-patch) or multiple nt (long-patch) |
| Key Enzyme | UvrC (dual incision) | Glycosylase or APE1 (base/AP cleavage) |

---

### TYPE 3: Problem-Solving Questions
**Format**: "An Hfr strain transfers markers at the following times (min): A=5, B=10, C=15. What is the map distance between B and C?"

**Answer**:
- B to C = 15 - 10 = 5 minutes = 5 map units
- Answer: 5 m.u. apart

---

### TYPE 4: Prediction Questions
**Format**: "A mutation in *uvrB* is introduced. What would happen if cells were exposed to UV light?"

**Answer Strategy**:
1. Identify what *uvrB* does (UvrB is part of NER; recognizes lesions)
2. Predict consequence of loss (NER cannot function)
3. Predict what damage accumulates (thymine dimers not removed)
4. Predict cell outcome (death, mutagenesis if SOS activated, or survival if repaired by other pathways)

**Example Answer**:
"UvrB is essential for NER. Without UvrB, the UvrBC complex cannot recognize thymine dimers. Thymine dimers would accumulate in DNA, blocking replication and transcription. The cell would likely die unless the SOS response is activated (error-prone polymerases may bypass lesions). However, UV survival would be severely reduced."

---

### TYPE 5: Multiple-Choice with Distractor Analysis

**Format**: "Which is the PRIMARY function of RuvC?"
A. Loading RecA onto ssDNA
B. Cleaving Holliday junctions
C. Unwinding DNA at double-strand breaks
D. Recognizing Chi sites

**Distractor Analysis**:
- A: FALSE → RecA loads on ssDNA generated by RecBCD, not RuvC
- B: TRUE → RuvC endonuclease cleaves Holliday junctions (our answer)
- C: FALSE → RuvAB (not RuvC) binds junctions; UvrD unwinds
- D: FALSE → RecC (not RuvC) recognizes Chi sites

**Answer**: B

---

## 60-Minute Exam Strategy

**Time Allocation** (10 questions, 6 min per question average):

1. **Read ALL questions first** (2 min)
   - Identify question types
   - Note which require diagrams, which are pure concept

2. **Answer easiest/shortest questions** (20 min)
   - Quick conceptual questions
   - Multiple-choice where answer is clear

3. **Tackle mechanism questions** (25 min)
   - Require more detailed explanation
   - Allocate ~3-5 min per question
   - Draw diagrams if helpful (e.g., restriction map, Hfr transfer)

4. **Problem-solving** (10 min)
   - Hfr mapping, PCR calculations, mutation rate
   - Check work before moving on

5. **Review & finish** (3 min)
   - Quickly review answers
   - Fix obvious errors

**Pro Tips**:
- Write clearly (graders can't give credit for illegible work)
- Show your work (partial credit for correct method, wrong answer)
- Label diagrams carefully
- Use arrows to show direction of reactions
- Define abbreviations on first use

---

## Avoiding Common Mistakes

| Mistake | Why It's Wrong | Correct Understanding |
|---------|---|---|
| "Restriction enzymes always cut DNA" | Methylation status matters | Methylated sites are protected from cleavage |
| "MMR uses methylation in all organisms" | Eukaryotes use different mechanism | Only bacteria like *E. coli* use Dam methylation |
| "PCR creates 2^n DNA in every cycle" | Plateau effect limits later cycles | Early cycles: doubling; later: plateau |
| "RecA loads on dsDNA" | RecA is ssDNA-binding protein | RecA specifically recognizes single-stranded DNA |
| "Transduction always gives stable genes" | Abortive transduction exists | Only integrated transductants are stable |
| "Hfr transfers F plasmid" | F is integrated in chromosome | Hfr transfers chromosome; F+ transfers F plasmid |
| "ddNTPs terminate because of charge" | Chemical reason is different | No 3'-OH prevents next phosphodiester bond |
| "Gene conversion always produces 1:1 ratio" | Non-reciprocal | Can produce 3:5 or 5:3 ratios in meiosis |

---

# PRACTICE TEST BANK

## Section A: Conceptual Questions (Open-Ended)

### Q1: DNA Repair Decision Tree
A cell experiences a thymine dimer (TT adduct) on one side of the chromosome and a single oxidized guanine (8-oxoG) on another side. Describe which repair pathway would address each lesion and why that pathway is specialized for that damage type.

**Model Answer**:
- **Thymine dimer** → NER (nucleotide excision repair)
  - TT dimer causes significant DNA distortion
  - NER recognizes distortion (via UvrA/UvrB)
  - Excises large segment (12-13 nt) containing lesion
  - Removes both damaged nucleotides in one repair event

- **8-oxoG** → BER (base excision repair)
  - 8-oxoG is small damage; doesn't distort helix significantly
  - BER specialized for single base damage
  - 8-oxoguanine glycosylase recognizes 8-oxoG specifically
  - Removes single base; creates AP site; refilled with normal guanine

**Why specialized**: Different pathways because lesion sizes and distortion levels differ; using right pathway is efficient and prevents over-repair.

---

### Q2: Luria-Delbrück Interpretation
You perform a fluctuation test and observe high variance in numbers of resistant mutants across replicates, with some cultures showing 0 mutants and one showing 47 mutants. Explain what this pattern tells you about when mutations arise.

**Model Answer**:
High variance indicates **pre-existing mutations**.

Explanation:
- If mutations were induced BY phage (adaptive response), all cultures would experience same selection pressure → similar numbers
- High variance suggests some cultures had mutations early in growth → many descendants; others had none or late mutations → few descendants
- Single large jackpot (47) likely arose from one mutation early, then proliferated during remaining growth
- This pattern matches Luria-Delbrück prediction for random, pre-existing mutations

**Conclusion**: Mutations are spontaneous and arise before selection.

---

### Q3: SOS Response Narrative
Describe the complete SOS response pathway from DNA damage to expression of error-prone polymerase genes, explaining why this seems maladaptive but is actually adaptive.

**Model Answer**:

**Mechanism**:
1. UV damage creates TT dimers; replication fork stalls
2. ssDNA generated at stalled fork
3. RecA binds ssDNA → RecA* (active form)
4. RecA* stimulates LexA (repressor) to autocleavage
5. LexA levels drop; SOS genes (*umuDC*, *recF*, etc.) derepressed
6. Error-prone Pol V synthesizes past lesions (wrong nucleotides incorporated)

**Seeming paradox**: Mutagenesis seems bad (errors); why activate it?

**Adaptive logic**:
- Alternative: replication completely blocked → cell dies
- With Pol V: cell survives; 99% of mutations are deleterious, but some are neutral or beneficial
- Population-level advantage: some mutants have altered phenotypes that improve fitness
- Short-term cost (transient mutagenesis) < long-term benefit (survival to pass genes)
- SOS is emergency response: "accept mutations to survive; hope natural selection eliminates bad ones later"

---

### Q4: Hfr Mapping from Time of Entry Data
An Hfr strain (*gal*+ *lac*+ *trp*+ *met*+) is mated with F- strain (*gal*- *lac*- *trp*- *met*-). Interrupted mating data:

| Time (min) | % Recipients with *gal*+ | % with *lac*+ | % with *trp*+ | % with *met*+ |
|------------|----------------------|--------------|--------------|---------------|
| 5 | 1 | 0 | 0 | 0 |
| 10 | 50 | 2 | 0 | 0 |
| 15 | 80 | 45 | 5 | 0 |
| 20 | 90 | 75 | 40 | 2 |

(a) Determine time of entry (TOE) for each marker
(b) Draw a genetic map with distances
(c) Explain why % recombinants doesn't reach 100%

**Model Answer**:

**(a) Time of Entry** (when frequency first becomes detectable, ~>1%):
- *gal*+: ~5 min
- *lac*+: ~10-12 min (reading between 10: 2%, 15: 45%)
- *trp*+: ~15 min
- *met*+: ~18-20 min

**(b) Genetic Map**:
```
  oriT ─5 min─ gal+ ─5-7 min─ lac+ ─3-5 min─ trp+ ─3-5 min─ met+
    0          5            ~12          15           ~20
```

**(c) Why not 100% recombinants?**
- Mating is interrupted before complete transfer
- Recipients receive partial merodiploid (F- chromosome + some Hfr markers)
- Recombination requires homologous recombination between Hfr DNA and recipient chromosome
- Not all recipients undergo recombination for every marker
- Some recipients are disrupted before gene enters; some fail to recombine afterward
- Efficiency decreases with distance (later markers have lower recombination frequency)

---

## Section B: Multiple-Choice Questions

### Q5: PCR Primer Design
You want to design primers to amplify a 500 bp region. The forward primer sequence is 5'-ATGCGATTACGATCC-3' with Tm = 58°C. The reverse primer is 5'-GATCCGTACGTAAA-3' with Tm = 60°C. What is the optimal annealing temperature for PCR?

A. 48°C
B. 52°C
C. 56°C
D. 62°C

**Answer**: **B (52°C)**

**Explanation**:
- Use **Tm of lowest-Tm primer (forward: 58°C) minus 2-5°C**
- 58 - 5 = 53°C (or 58 - 2 = 56°C)
- Best answer is ~52-56°C range; closest is B (52°C)
- This ensures primer hybridization without being so high that specificity is lost or polymerase is inhibited

---

### Q6: NER Mechanism
Which of the following best describes what happens when UvrD binds to the complex at a thymine dimer lesion?

A. UvrD cuts the DNA backbone upstream and downstream of the lesion
B. UvrD unwinds and displaces the oligonucleotide segment containing the lesion
C. UvrD catalyzes methylation to distinguish new from old DNA strand
D. UvrD recruits DNA polymerase to synthesize a replacement strand

**Answer**: **B**

**Explanation**:
- UvrD is a helicase (unwindase), not a nuclease or methylase
- After UvrC makes dual incisions (5' and 3' of lesion), UvrD unwinds the gap
- Unwinds and displaces the 12-13 nt oligonucleotide containing lesion
- DNA Pol I then fills gap (not UvrD's job)
- A is wrong (UvrC cuts, not UvrD)
- C is wrong (methylation is MMR, not NER)
- D is wrong (Pol I does synthesis, not UvrD)

---

### Q7: Conjugation F+ vs. Hfr
Which of the following statements best distinguishes F+ × F- conjugation from Hfr × F- conjugation?

A. F+ transfers circular F plasmid; Hfr transfers linear chromosome segment
B. F+ creates more stable merodiploids; Hfr creates transient partial diploids
C. F+ mating requires pilus; Hfr mating does not
D. F+ transfers all F genes; Hfr transfers F genes first

**Answer**: **A**

**Explanation**:
- F+: F plasmid is autonomous, transfers as unit → rolling circle replication → creates copy in recipient → stable F+ formation
- Hfr: F integrated in chromosome; transfer begins at integrated origin → chromosome transfers linearly → recipient is F- merodiploid (if mating interrupted before trailing F sequences)
- B: Both create merodiploids (F+ = for whole plasmid; Hfr = for partial chromosome)
- C: Both use pilus (made by *tra* genes)
- D: Hfr transfers chromosome genes first (from *oriT*); F genes are at end (usually not transferred if interrupted)

---

### Q8: Restriction Enzyme Specificity
Restriction enzyme *PstI* recognizes the sequence 5'-CTGCAG-3' and cuts such that the overhang is 3'-CGTAC-5'. This means:

A. *PstI* produces sticky ends with 4 nt 5' overhang
B. *PstI* produces blunt ends
C. *PstI* produces sticky ends with 3 nt 3' overhang
D. The recognition sequence is not palindromic

**Answer**: **C**

**Explanation**:
- Recognition: 5'-CTGCAG-3' / 3'-GACGTC-5'
- Cuts: 5'-CTGCA^G-3' / 3'-GAC^GTC-5'
- After cut:
  ```
  5'─── CTGCA ───3'     (3' overhang: GT is complementary to AC on other strand)
  3'─── G  ───5'

  3'─── GACGTC ───5'
  5'─       AC ───3'    (5' overhang: AC)
  ```
  Wait, let me reconsider...

  If cuts at CTGCA^ and G:
  ```
  5'─── CTGCA      ───3'
  3'─── G  ACGTC ───5'  → left with 3' overhang (AC hanging off the 3' end)
  ```

  3 nt overhang on one end; it's a 3' overhang on one strand = complementary to 5' overhang on other

  Answer: **C** (3 nt 3' overhang on one strand = sticky end)

---

### Q9: Holliday Junction & Gene Conversion
During homologous recombination, if a mismatch (A-a) forms in the heteroduplex region of a Holliday junction and mismatch repair "corrects" all A-a pairs to A-A, what would be the genetic consequence in meiotic segregation?

A. 4:4 ratio (normal Mendelian)
B. 3:5 ratio (gene conversion toward A)
C. 5:3 ratio (gene conversion toward a)
D. 0:8 ratio (all A phenotype)

**Answer**: **B**

**Explanation**:
- Normal: heteroduplex has A on one side, a on other
- Normal segregation: one chromatid A, one a → 4:4 ratio
- Gene conversion: mismatch repair "corrects" all to A-A (in heteroduplex)
- After Holliday resolution: both products carry A allele
- Meiotic segregation: 3 A : 5 a (or 5 A : 3 a, depending on which products are converted)
- Here: A is "winning" → 3:5 ratio (more As than expected)
- Or equivalently: can't produce as many as (only 3 instead of 4)

Answer: **B** (3:5 indicates conversion toward A allele)

---

### Q10: SOS Response Logic
A bacterial culture is exposed to X-ray radiation, which causes double-strand breaks (DSBs). RecA activates the SOS response. Which of the following genes would you NOT expect to be upregulated as part of the SOS response?

A. *recF* (homologous recombination protein)
B. *umuDC* (error-prone polymerase V)
C. *uvrA* (nucleotide excision repair)
D. *dnaB* (replication helicase); *dnaK* (chaperone)

**Answer**: **C** (or possibly **D** if the question expects that *uvrA* is already constitutively expressed)

**Better Answer**: **C**, because...

**Explanation**:
- **SOS response upregulates**:
  - *recF*, *recO*, *recR* → homologous recombination (repair DSBs)
  - *umuDC* → error-prone Pol V (bypass lesions)
  - *dnaB*, *dnaK* → replication/repair machinery support

- **SOS response does NOT typically upregulate**:
  - *uvrA*, *uvrB*, *uvrC* → **NER (nucleotide excision repair)**
  - NER is for lesions like TT dimers (distortion)
  - DSBs are handled by HR/DSB repair, not NER
  - *uvrA* is already expressed at basal levels; not part of SOS

**Answer**: **C** (*uvrA* is not part of the SOS response)

---

## Section C: Integration & Problem-Solving

### Q11: Multi-Step Integration Problem
An *E. coli* K-12 strain undergoes spontaneous mutation at rate μ = 2 × 10^-8 per cell per generation. A culture of 10^8 cells is grown for 10 generations. Assuming each cell divides once per generation:

(a) What is the expected number of new mutations in the population?
(b) If one of these mutations is phage resistance, and phage is added to the culture, approximately what percentage of cells would be uninfected if multiplicity of infection (m) = 1?
(c) Explain how the Luria-Delbrück test would distinguish whether these resistant cells arose before or after phage addition.

**Model Answer**:

**(a) Expected number of mutations**:
- Formula: E(mutations) = μ × N × generations
- N = 10^8 cells/generation; 10 generations = 10^8 × 10 = 10^9 total cells produced
- E(mutations) = 2 × 10^-8 × 10^9 = 2 × 10^1 = **20 mutations**
- Or: per generation: μ × N = 2 × 10^-8 × 10^8 = 2 mutations/generation × 10 generations = 20 total

**(b) Uninfected cells at m=1**:
- Poisson formula: P(uninfected) = e^(-m) = e^(-1) ≈ **0.368 or 37%**
- (At m=1, about 37% of cells escape infection; 63% infected)

**(c) Luria-Delbrück test**:
- **Setup**: Parallel cultures (small, independent flasks) vs. one large culture
- **Parallel cultures**: Mutations arise at different times → high variance
  - Some flasks get early mutation (many descendants) → jackpot
  - Others get no mutation → zero
  - Variance >> mean
- **Large culture**: Single culture experiences same growth → consistent number
  - Variance ≈ mean
- **Result if observed**: High variance in parallel = **PRE-EXISTING mutations** (supports our prediction from part a)
- If mutations induced by phage: variance would be low in both (all cultures equally stressed)

---

### Q12: Hfr Mapping Challenge
An Hfr strain is crossed with F- recipient. Interrupted mating reveals: *gal*+ at 8 min, *arg*+ at 15 min, *his*+ at 22 min, *thr*+ at 28 min.

(a) What is the distance (in map units) between *arg* and *his*?
(b) If you wanted to map genes to one side of *thr*, which direction would you need to change? (i.e., what would have to happen?)
(c) Propose a reciprocal Hfr strain that transfers genes in opposite order. What would be required?

**Model Answer**:

**(a) Distance *arg*+ to *his*+**:
- Time of entry *arg*+: 15 min
- Time of entry *his*+: 22 min
- Distance = 22 - 15 = **7 map units** (1 min = 1 m.u.)

**(b) Mapping genes beyond *thr*+**:
- *thr*+ enters at 28 min; this is late in the 30-min observation window
- To map genes beyond *thr*+, need:
  - Longer mating times (extend beyond 28 min) → observe when next marker enters
  - OR use reciprocal Hfr (orient so *thr*+ region transfers from the other direction, allowing earlier entry)

**(c) Reciprocal Hfr design**:
- Current Hfr: oriT is between *gal*+ and *arg*+; transfers toward *thr*
- Reciprocal Hfr: F integrated in opposite orientation
  - Transfer order reversed: *thr*+ enters first, then *his*+, *arg*+, *gal*+
  - Would allow mapping genes beyond *thr*+ with earlier entry times
  - Requires: F plasmid to excise and reintegrate at same location but opposite strand orientation

---

### Q13: Sanger Sequencing Analysis
In a Sanger sequencing reaction, you use ddA (red label), ddC (blue), ddG (yellow), ddT (green). After electrophoresis, fragments are separated by size. Reading from smallest to largest fragment, you observe the following dye labels:

**Capillary reading** (smallest → largest fragment): Blue, Red, Blue, Yellow, Red, Blue, Green

Assuming the primer annealed immediately 5' to the sequence shown:
(a) What is the DNA sequence of the template strand (3'→5' direction)?
(b) What would be the complementary strand sequence (5'→3')?
(c) Why is the sequence read from smallest to largest fragment?

**Model Answer**:

**(a) Template strand sequence (3'→5')**:
Reading the dye labels in order:
- Blue = ddC → first nucleotide incorporated was C (no wait, it's the terminator)
- Red = ddA
- Blue = ddC
- Yellow = ddG
- Red = ddA
- Blue = ddC
- Green = ddT

Wait, let me reconsider. Each fragment represents synthesis from primer to a termination point.

Actually, if reading smallest to largest:
- Smallest fragment: primer + 1 nt + ddC → first nt is C
- Next: primer + 2 nt + ddA → second nt is A (reading 5' direction of new strand)
- Next: primer + 3 nt + ddC → third nt is C
- Next: primer + 4 nt + ddG → fourth nt is G
- Next: primer + 5 nt + ddA → fifth nt is A
- Next: primer + 6 nt + ddC → sixth nt is C
- Largest: primer + 7 nt + ddT → seventh nt is T

New strand synthesized 5'→3': primer - C - A - C - G - A - C - T
(But the primer is before our read sequence)

Template strand (3'→5', template for synthesis): **3'-G T G C A C G-5'** (or just: GTGCACG read 3'→5')

**(b) Complementary strand (5'→3')**:
Complement to 3'-GTGCACG-5' is **5'-CACGTGC-3'**
(Or the new strand synthesized: 5'-CACGTGC-3')

**(c) Why read smallest to largest?**
- Smallest fragments = shortest synthesis = terminated early = closest to primer
- As fragment size increases, termination point moves farther from primer
- Reading order: close to far → sequence 5'→3' direction of template

---

## Final Exam Practice: Full-Length Mini Test (30 minutes, 5 questions)

### Q14 (Mechanism, 5 min)
Describe the complete process of mismatch repair in *E. coli*, including how the cell distinguishes the new (error-prone) strand from the parental (template) strand. Why is this strand discrimination critical to repair fidelity?

### Q15 (Concept, 3 min)
Why is the SOS response considered both dangerous (mutagenic) and beneficial (adaptive)? Explain the biological logic.

### Q16 (Problem, 5 min)
An Hfr(*gal* *lac* *trp*) ×  F-(*gal*- *lac*- *trp*-) mating is interrupted at 12 minutes. What recombinant classes would you expect to recover if you select for *lac*+ recombinants?

### Q17 (Multiple-choice, 2 min)
In PCR, which of the following would INCREASE the specificity of primer binding?
A. Lowering the annealing temperature
B. Increasing primer concentration
C. Designing primers with higher Tm
D. Using more cycles

### Q18 (Application, 10 min)
Design an experiment to test whether a newly isolated antibiotic-resistant strain acquired resistance via spontaneous mutation or via horizontal gene transfer from another species. Describe the key assay you would perform (e.g., DNA detection, mating test, fluctuation test) and interpret the results.

---

## Answer Key (Brief)

| Q | Answer | Key Points |
|---|--------|-----------|
| Q5 (PCR Tm) | B (52°C) | Use lowest-Tm primer minus 2-5°C |
| Q6 (NER) | B | UvrD is helicase; unwinds and removes oligonucleotide |
| Q7 (Conj) | A | F+ transfers F plasmid; Hfr transfers chromosome |
| Q8 (PstI) | C | 3 nt 3' overhang (sticky end) |
| Q9 (Holliday) | B | Gene conversion toward A allele → 3:5 ratio |
| Q10 (SOS) | C | NER (*uvrA*) not upregulated in SOS response |

---

## Self-Assessment Checklist

After studying, you should be able to:

- [ ] Explain spontaneous vs. induced mutation with examples
- [ ] Describe Luria-Delbrück experiment; interpret variance patterns
- [ ] Walk through MMR mechanism (all enzymes, strand discrimination, methylation)
- [ ] Explain NER dual incision (location, size, enzymes)
- [ ] Describe RecBCD pathway; role of Chi site
- [ ] Understand Holliday junction formation and resolution
- [ ] Calculate recombination frequency and map distances
- [ ] Perform Hfr interrupted mating mapping (time of entry)
- [ ] Distinguish transformation, transduction, conjugation
- [ ] Explain F+ vs. Hfr conjugation
- [ ] Design PCR primers (Tm, specificity)
- [ ] Explain ddNTP mechanism in Sanger sequencing
- [ ] Distinguish sticky vs. blunt restriction ends
- [ ] Explain why SOS response is adaptive despite mutagenesis
- [ ] Apply molecular techniques to experimental scenarios

---

**File Location**: `/sessions/practical-happy-hopper/mnt/Obsidian Vault/04_Course_Notes/MCDB 101A/NOTION_Final_Study_Guide.md`

**Recommended Next Steps**:
1. Review high-yield topics (Module 6 of main lesson)
2. Work through all practice problems without notes
3. Create flashcards for mechanism steps
4. Form study group; explain concepts to peers (best learning)
5. Time yourself on practice test to build exam pacing
6. Review any questions you miss by reading the mechanism completely

**Good luck on your final exam!**
