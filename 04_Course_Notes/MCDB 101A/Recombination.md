# Recombination

**Course:** [[Course Dashboard]] | **Yield:** MEDIUM ⭐⭐

---

## 🎯 Learning Objectives

1. Describe the Holliday model of homologous recombination and the steps it predicts
2. Explain the double-strand break (DSB) repair model and how it differs from the Holliday model
3. Define heteroduplex DNA and gene conversion
4. Explain the role of RecA in strand exchange
5. Distinguish homologous recombination from site-specific recombination

---

## 🧠 Core Concepts

### Overview of Recombination Types

| Type | Sequence Requirement | Key Proteins | Examples |
|------|---------------------|-------------|---------|
| **Homologous (HR)** | Long regions of sequence homology | RecA, RuvA, RuvB, RuvC | Repair of DSBs, meiotic crossovers |
| **Site-specific** | Short specific sequences at defined sites | Integrase, Cre/lox, Flp/FRT | λ integration, transposon excision |
| **Transposition** | Terminal repeats (TIRs or LTRs) | Transposase | IS elements, Tn3, retrotransposons |

### The Holliday Model (1964)

**Steps**

1. **Alignment:** Two homologous duplexes align in parallel (same polarity)
2. **Single-strand nicking:** One strand of each duplex is nicked at equivalent positions by an endonuclease
3. **Strand exchange:** The nicked strands cross over and invade the complementary strand of the other duplex → **Holliday junction** formed
4. **Branch migration:** The Holliday junction can move in either direction, extending the heteroduplex region (RuvA/RuvB in bacteria)
5. **Resolution:** RuvC (Holliday junction resolvase) cuts at the junction in one of two orientations:
   - **Splice resolution (crossover):** Cuts strands that were NOT originally exchanged → flanking markers recombine
   - **Patch resolution (non-crossover):** Cuts the strands that WERE exchanged → flanking markers stay parental; only the heteroduplex patch remains

**Heteroduplex DNA**

Region where one strand is from each parental duplex. Can contain mismatches if the two parents differ in that region → repaired by MMR → **gene conversion** (non-Mendelian segregation).

**Limitations of the Holliday Model**

- Requires two simultaneous nicks at exactly equivalent positions (unlikely)
- Cannot initiate recombination at a DNA break

### Double-Strand Break (DSB) Repair Model (Szostak et al., 1983)

**Steps**

1. **DSB formation:** A double-strand break is introduced in one duplex
2. **Resection (5'→3' exonuclease):** 5' ends at the break are resected, leaving 3' single-stranded tails
3. **Strand invasion:** One 3' tail invades the intact homologous duplex → D-loop (displacement loop) forms
4. **DNA synthesis:** The invading 3' end is extended using the intact duplex as template; the displaced strand also becomes a template
5. **Two Holliday junctions form:** The elongated invading strand anneals with the other resected end → two HJs
6. **Resolution:** Each HJ is resolved independently → can produce crossover or non-crossover products
7. **Ligation:** Nicks sealed by ligase

**Key Advantages Over Holliday Model**

- Explains DSB repair: initiated at an existing break, not requiring simultaneous nicks
- Explains gene conversion: the broken molecule uses the intact duplex as template → conversion of sequence at the break site
- Better supported by experimental evidence

### RecA and Strand Exchange

**RecA Functions**

- **ssDNA binding:** RecA polymerizes on ssDNA (3'→5' polarity preferred) in presence of ATP → nucleoprotein filament
- **Homology search:** RecA filament samples dsDNA for complementary sequences
- **Strand exchange (strand invasion):** RecA catalyzes displacement of one strand of dsDNA and annealing of the ssDNA template → D-loop
- **ATP hydrolysis:** Drives directional strand exchange (3'→5' on ssDNA = 5'→3' on displaced strand)

**RecA Eukaryotic Homolog**

**RAD51** performs the same function in eukaryotes; essential for DSB repair via HR.

### RuvABC — Holliday Junction Processing

| Protein | Function |
|---------|---------|
| **RuvA** | Recognizes and binds Holliday junction; recruits RuvB |
| **RuvB** | AAA+ ATPase; drives branch migration (∼1–10 bp/step) |
| **RuvC** | Resolvase; cuts HJ at specific sequences (5'-A↓TTG-3'); produces nicked duplexes |

### Site-Specific Recombination — λ Integration

**Mechanism**

- λ **Integrase (Int)** + **IHF** (integration host factor)
- **attP** (phage attachment site) × **attB** (bacterial attachment site) → **attL** + **attR** flanking the integrated prophage
- Int makes staggered cuts at the overlap region of attP and attB
- Two-step strand exchange (topoisomerase I-like): no high-energy cofactor required
- **Excision:** Int + **Xis** (excisionase) catalyze the reverse reaction (attL × attR → attP + attB)

**Directionality**

- Integration: Int alone can do it (Xis not present → prevents excision in the lysogen)
- Excision: requires Xis (induced during SOS/lytic cycle)

### Gene Conversion

**Definition:** Non-reciprocal transfer of genetic information between two sequences — one sequence is converted to the other's sequence at the recombination site.

**Mechanism:** Arises when heteroduplex DNA containing a mismatch is repaired using one strand as template → both strands of the heteroduplex region end up with the same sequence as one parent.

**Evidence:** In fungi (tetrad analysis), a locus can show 3:1 or 1:3 segregation instead of the expected 2:2 → indicates one chromatid was converted.

---

## ⚠️ Exam Traps

- ❌ **"The Holliday model requires a DSB"** — The original Holliday model used single-strand nicks; the DSB repair model was a later improvement.
- ❌ **"Gene conversion is always associated with crossover"** — Gene conversion can occur without a crossover (patch resolution).
- ❌ **"RuvC creates the Holliday junction"** — RuvC resolves it; RecA creates the initial strand invasion.

---

## Practice Questions

1. In the Holliday model, what determines whether resolution produces a crossover or a patch (non-crossover) product? Draw the two resolution orientations.

2. The DSB repair model predicts gene conversion at the site of the break. Explain mechanistically why this occurs.

3. A mutation in *ruvC* prevents resolution of Holliday junctions. What would be the consequences for homologous recombination in this bacterium?

4. RecA requires ssDNA to initiate strand exchange. What cellular process generates the ssDNA substrate that activates RecA during the SOS response?

5. Compare and contrast homologous recombination and λ site-specific recombination in terms of sequence requirements, proteins involved, and biological outcomes.

---

## Related Concepts

- [[Holliday Junction]]
- [[Holliday Junction]]
- [[Recombination]]
- [[DNA Repair]] — DSB repair overlaps with HR
- [[Bacteriophage Lambda]] — λ integrase uses site-specific recombination
- [[Gene Transfer]] — conjugation involves RecA-mediated recombination of transferred DNA
