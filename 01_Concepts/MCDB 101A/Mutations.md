# Mutations

## Definition
A mutation is a **measurable, permanent alteration in the DNA sequence**. Mutations are rare (rates of 10⁻⁶ to 10⁻¹¹ per base per replication) — rare enough to maintain genome stability, yet frequent enough to provide variation for evolution.

---

## Types of Mutations

### Point Mutations (Single Base-Pair Changes)
- **Transitions**: Purine ↔ Purine (A ↔ G) or Pyrimidine ↔ Pyrimidine (C ↔ T) — same class
- **Transversions**: Purine ↔ Pyrimidine (A/G ↔ C/T) — different class
- Transitions more common spontaneously; some mutagens preferentially cause transversions

### Insertions and Deletions (Indels)
- Addition or removal of one or more base pairs
- **Frameshift mutations**: Indels that are NOT multiples of 3 → shift the reading frame → downstream codons all misread → typically truncated, nonfunctional protein
- Indels in multiples of 3: in-frame insertions/deletions → add/remove amino acids but preserve frame

### Macrolesions
- Large-scale rearrangements: inversions, duplications, translocations, transpositions

### Classification by Phenotypic Effect
| Class | Definition |
|-------|-----------|
| **Silent (synonymous)** | Codon change, same amino acid (due to degeneracy) |
| **Missense** | Codon change, different amino acid |
| **Nonsense** | Sense codon → stop codon → premature termination |
| **Frameshift** | Reading frame shifted; usually catastrophic |

---

## Spontaneous Mutations

Arise under normal conditions without exogenous mutagens.

### Tautomerization
- Bases exist in rare **tautomeric forms** (imino or enol)
- Rare tautomers have altered base-pairing: e.g., rare **enol-G** pairs with T instead of C → G:C → A:T transition after two rounds of replication

### Depurination
- Spontaneous hydrolysis of N-glycosidic bond releases purine base → **AP (apurinic) site**
- Estimated ~5,000 depurinations/cell/day in humans
- Unrepaired AP site causes **transversion** at that position

### Deamination
- Spontaneous removal of amino group:
  - **Cytosine → Uracil** (most common) → G:C to A:T transition if unrepaired (repaired by BER/UNG)
  - **5-methylcytosine → Thymine** (at CpG sites) → G:C to A:T transition; **mutational hotspot** because T is not recognized as damage by some repair pathways
  - Adenine → Hypoxanthine (pairs with C instead of T)

### Replication Errors
- DNA Pol III misincorporation rate: ~1 error per 10⁷ nt
- 3'→5' proofreading reduces error rate to ~10⁻⁸–10⁻¹⁰
- **Slipped strand mispairing**: polymerase slips on repetitive sequences → frameshifts; **hotspots** often at homopolymer runs

---

## Induced Mutations

Caused by exogenous chemical or physical agents (**mutagens**).

### Chemical Mutagens

| Mutagen | Mechanism | Type of Mutation |
|---------|-----------|-----------------|
| **EMS** (ethylmethane sulfonate) | Alkylates O⁶ of guanine → O⁶-ethylG pairs with T | G:C → A:T transitions |
| **Nitrous acid (HNO₂)** | Deaminates C→U, A→hypoxanthine | Transitions (C:G→T:A; A:T→G:C) |
| **5-Bromouracil (5-BU)** | Base analog; replaces T; enol form pairs with G | Transitions |
| **2-Aminopurine (2-AP)** | Base analog; replaces A; pairs with C | Transitions |
| **Acridines (proflavin)** | Intercalate between base pairs → polymerase slippage | Frameshifts (insertions/deletions) |
| **ICR-191** | Bifunctional alkylator | Frameshifts |

### Physical Mutagens

| Mutagen | Mechanism | Damage |
|---------|-----------|--------|
| **UV light** (254 nm) | Energy absorbed by thymine → **pyrimidine dimers** (CPDs, 6-4 PPs) | Distort helix; block replication; repaired by NER |
| **X-rays / γ-rays** | Ionize DNA; generate ROS | DSBs, base oxidation |

---

## Mutational Hotspots
- Sites with unusually high mutation frequency
- Causes: repetitive sequences (slippage), methylated cytosines (CpG → C→T), palindromes
- **5-methylcytosine** at CpG dinucleotides is a classic hotspot: deamination to T produces a C:G → T:A change; repair is imperfect because T:G mismatch is ambiguous

---

## Reversions and Suppressors

### True Reversion
- Second mutation at the **same base pair** as the original → restores original sequence
- Can also be nearby change that restores reading frame or amino acid function

### Intragenic Suppressor
- Second mutation **within the same gene** but at different position compensates for first
- e.g., second frameshift of opposite sign (+1 and −1) = restored frame; or compensatory amino acid change in protein

### Extragenic (Intergenic) Suppressor
- Second mutation in a **different gene** compensates for first
- **Nonsense suppressor tRNA**: mutation in tRNA anticodon → reads stop codon as amino acid
- Missense suppressor: tRNA charged with wrong amino acid restores function

---

## Luria-Delbrück Fluctuation Test
- **Question**: Are mutations pre-adaptive (random, spontaneous) or post-adaptive (directed by environment)?
- **Experiment**: Multiple small cultures grown from single cells; exposed to T1 phage; count resistant colonies
- **Result**: High **variance** between cultures (some have many resistant colonies, some have none) → consistent with **pre-adaptive (random) mutations** arising before selection
- **Conclusion**: Mutations are **spontaneous and random**, not directed by the environment
- Jackpot cultures (very high resistant count) arise when mutation occurred early in culture growth

---

## Mutation Rate vs. Mutation Frequency
- **Mutation rate**: Probability of a mutation occurring **per gene per replication** (e.g., 10⁻⁸)
- **Mutation frequency**: Proportion of cells in a **population** carrying a mutation (e.g., 10⁻⁶) — cumulative over many generations

---

## Ames Test (Salmonella Mutagenicity Assay)
- Tests whether a chemical is mutagenic (and potentially carcinogenic)
- Uses **his⁻ Salmonella** strains (histidine auxotrophs); mutagen → reversion to his⁺ → colonies on −His plates
- Rat liver extract (**S9 fraction**) added to convert promutagens to active mutagens
- Higher reversion frequency than spontaneous = mutagenic

---

## Key Exam Points
- Transitions: same-class change; Transversions: class switch
- Acridines → frameshifts (not base substitutions)
- EMS → G:C→A:T transitions (alkylates G)
- UV → pyrimidine dimers → NER substrate
- Luria-Delbrück: high variance = pre-adaptive mutations; low variance = post-adaptive (directed)
- Mutation rate ≠ mutation frequency (rate = per replication; frequency = proportion in population)
- CpG sites are mutational hotspots due to 5-methylcytosine deamination → T
- Nonsense suppressor tRNA inserts amino acid at stop codon

---

## Related Concepts
- [[DNA Repair Pathways]]
- [[Base Excision Repair]]
- [[Transcription]]
- [[Translation]]
- [[Recombination]]
- [[Deletion Mapping]]

## Prerequisites
- DNA structure and replication
- Genetic code and translation
- DNA polymerase fidelity

## Importance: HIGH YIELD
Mutagen mechanisms, transition vs. transversion, Luria-Delbrück logic, and reversion/suppression are all heavily tested.
