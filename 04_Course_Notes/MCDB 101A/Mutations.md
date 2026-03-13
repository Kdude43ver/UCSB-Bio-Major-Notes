# Mutations

**Course:** [[Course Dashboard]] | **Yield:** MEDIUM ⭐⭐

---

## 🎯 Learning Objectives

1. Distinguish spontaneous from induced mutations; classify by molecular mechanism
2. Describe the Luria-Delbrück fluctuation test and what it proves
3. Apply the Poisson distribution to estimate mutation rates from fluctuation test data
4. Classify mutations as transitions, transversions, frameshift, nonsense, missense, or silent

---

## 🧠 Core Concepts

### Types of Mutations

**By Molecular Change**

| Type | Change | Example |
|------|-------|---------|
| **Transition** | Purine↔purine or pyrimidine↔pyrimidine | A→G, C→T |
| **Transversion** | Purine↔pyrimidine | A→T, G→C |
| **Frameshift** | Insertion or deletion | +1 bp shifts reading frame |
| **Silent (synonymous)** | Codon change but same amino acid | AGA→AGG (both Arg) |
| **Missense** | Codon changes amino acid | AAA (Lys)→GAA (Glu) |
| **Nonsense** | Codon → stop codon | CAA (Gln)→UAA (Stop) |
| **Suppressor** | Mutation that reverses mutant phenotype | Intragenic or intergenic |

**Molecular Causes**

| Cause | Mechanism | Mutation type |
|-------|---------|--------------|
| Tautomeric shifts | Rare enol/imino forms of bases mispair | Transitions |
| Deamination | C→U (→T after replication); 5-methylC→T | Transitions at CpG hotspots |
| Depurination | Loss of purine → AP site → mutations | Transversions |
| Oxidation (ROS) | 8-oxoguanine pairs with A | G:C → T:A transversions |
| Alkylation | O⁶-methylguanine pairs with T | G:C → A:T transitions |
| UV light | Pyrimidine dimers (TT, TC, CC) | Frameshift or transition |

### The Luria-Delbrück Fluctuation Test (1943)

**Historical Significance**

Won the Nobel Prize (1969). Proved that mutations arise randomly and spontaneously, NOT in response to environmental selection (directed/adaptive mutation hypothesis disproved).

**Experimental Design**

- Grow many replicate small cultures of bacteria (same starting inoculum)
- Grow one large control culture for the same time
- Plate all cultures on selective medium (e.g., T1 phage) and count resistant colonies

**Two Hypotheses Being Tested**

| Hypothesis | Prediction |
|-----------|-----------|
| **Directed mutation:** Phage causes mutation in response to contact | Each culture acquires similar number of resistant colonies; **low variance** |
| **Random (spontaneous) mutation:** Mutations arise before phage exposure | Early mutations → large clonal expansion → some cultures have **many** resistant colonies; late mutations → few; **high variance** |

**Result**

Cultures showed **high variance** (jackpot cultures with very many colonies, most cultures with very few). **Conclusion: Mutations are random/spontaneous, not directed by the selective agent.**

### Poisson Distribution — Rare Events

**When to Apply**

Mutations are rare events. The Poisson distribution describes the probability of k events when the average rate per trial is μ:

$$P(k) = \frac{e^{-\mu} \cdot \mu^k}{k!}$$

**P(0) Method for Estimating Mutation Rate**

- P(0) = probability of zero mutations in a culture
- Measure the fraction of cultures with zero resistant colonies (f₀)
- Then: $f_0 = e^{-\mu}$, so $\mu = -\ln(f_0)$
- Mutation rate per cell per generation = μ / N (where N = total cells at time of plating)

**Example Calculation**

- 20 replicate cultures, each grown to 10⁷ cells
- 6 cultures have zero resistant colonies
- f₀ = 6/20 = 0.30
- μ = −ln(0.30) ≈ 1.2 mutations per culture
- Mutation rate ≈ 1.2 / 10⁷ = 1.2 × 10⁻⁷ per cell per generation

### Mutational Hotspots

**Definition**

Positions in a gene that mutate at much higher frequency than average.

**Causes**

1. **5-methylcytosine (m⁵C):** Spontaneously deaminates to T → hotspot at CpG dinucleotides
2. **Repetitive sequences:** Slippage during replication → frameshifts
3. **DNA secondary structures:** Hairpins/cruciforms stall replication → deletions

### Mutagenic Agents

| Agent | Mechanism | Mutation Type |
|-------|---------|--------------|
| 5-Bromouracil (5-BU) | Base analog; BU* pairs with G → A→G transitions | Transitions |
| 2-Aminopurine (2-AP) | Base analog; pairs with C → T→C transitions | Transitions |
| Hydroxylamine | Converts C→hydroxylaminocytosine → pairs with A → C:G→T:A | Transitions |
| Nitrous acid | Deaminates A→hypoxanthine (→G), C→U (→T) | Transitions |
| Acridine dyes | Intercalate between base pairs → frameshifts | Frameshifts |
| EMS (ethyl methane sulfonate) | Alkylates G at O⁶ → pairs with T | G:C→A:T transitions |
| UV light | Pyrimidine dimers; distorts helix | Frameshifts + transitions |
| X-rays | DSBs; ionizing radiation | Deletions, translocations |

---

## ⚠️ Exam Traps

- ❌ **"Luria-Delbrück proved mutations are always random"** — It proved that at least some mutations (phage resistance) arise before selection, not that all mutations are untargeted.
- ❌ **"Transition mutations are more common than transversions"** — Transitions are more common (tautomers, deamination) but transversions do occur.
- ❌ **"A silent mutation has no phenotype"** — Silent mutations can affect codon usage, mRNA stability, splicing (in eukaryotes), and ribosome pausing.

---

## Practice Questions

1. In a Luria-Delbrück experiment, 100 replicate cultures are grown to 10⁸ cells. Twenty cultures have zero T1-resistant colonies. Estimate the mutation rate per cell per generation.

2. Why does deamination of 5-methylcytosine specifically create a hotspot for C→T transitions? Why doesn't uracil glycosylase fix this?

3. A mutation creates a premature stop codon (nonsense mutation) in *lacZ*. Would this mutation be recessive or dominant in a cell that also has a wild-type *lacZ* gene? Explain.

4. Acridine dyes such as proflavin cause frameshifts. If a +1 frameshift is introduced 30 codons from the start of a gene, what would be the consequence for the protein? If a −1 frameshift is introduced 5 codons downstream, what happens?

5. Explain why the Poisson distribution is appropriate for modeling mutation events but not for modeling replication errors overall.

---

## Related Concepts

- [[Luria-Delbrück Fluctuation Test]]
- [[Luria-Delbrück Fluctuation Test]]
- [[DNA Repair Pathways]] — repairs the mutations described here
- [[Transcription]] — nonsense mutations affect downstream genes in operons (polarity)
- [[Translation]] — missense and nonsense mutations affect protein function
