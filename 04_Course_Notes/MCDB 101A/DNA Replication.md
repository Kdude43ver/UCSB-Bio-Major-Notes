# DNA Replication

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## 🎯 Learning Objectives

1. Describe the Meselson-Stahl experiment and explain how it proves semiconservative replication
2. Identify the key components of the prokaryotic replication machinery and their functions
3. Explain the mechanism of leading and lagging strand synthesis
4. Describe how 3'→5' exonuclease proofreading increases replication fidelity
5. Define and explain the roles of oriC, DnaA, helicase, primase, SSBs, and clamp loader

---

## 🧠 Core Concepts

### The Meselson-Stahl Experiment (1958)

**Setup**
- Grow *E. coli* in heavy ¹⁵N medium until all DNA is fully labeled (¹⁵N/¹⁵N = heavy)
- Transfer to light ¹⁴N medium; harvest after 1, 2, 3 generations
- Analyze DNA density by CsCl equilibrium density gradient centrifugation

**Results & Interpretation**

| Generation | Band pattern | Interpretation |
|-----------|-------------|----------------|
| 0 | One heavy band (¹⁵N/¹⁵N) | All DNA fully labeled |
| 1 | One intermediate band (¹⁵N/¹⁴N) | Each new DNA has one old + one new strand |
| 2 | One intermediate + one light band | Half hybrid, half fully light |
| 3 | Mostly light + some intermediate | 1:3 ratio intermediate:light |

**Conclusion:** DNA replication is **semiconservative** — each daughter strand retains one parental strand.

**Why this rules out alternatives**
- **Conservative:** Would show separate heavy and light bands at generation 1 — NOT observed
- **Dispersive:** Would show a single band that shifts continuously lighter — NOT observed (stays as discrete bands)

### Origin of Replication (oriC)

**Prokaryotic oriC**

In *E. coli*:
- oriC = ~245 bp on the chromosome
- Contains **DnaA boxes** (9-mer repeats) and **AT-rich 13-mer repeats**

**Initiation Steps**

1. **DnaA** (initiator protein) binds DnaA boxes
2. Multiple DnaA monomers oligomerize → wraps DNA, melts AT-rich region
3. **DnaB** (helicase, hexamer) loads at melted region via **DnaC** (loader)
4. DnaB unwinds the double helix 5'→3' (relative to the strand being read)
5. **SSB proteins** stabilize single-stranded regions
6. **Primase (DnaG)** synthesizes RNA primers
7. **Clamp loader (γ complex)** loads **β-clamp** (sliding clamp/processivity factor)
8. **DNA Pol III** (core: α, ε, θ subunits) extends from primer

### The Replication Fork

**Key Enzymes and Functions**

| Protein | Function |
|---------|---------|
| DnaA | Initiator; recognizes and opens oriC |
| DnaB (helicase) | Unwinds dsDNA in 5'→3' direction |
| DnaC | Helicase loader |
| SSB | Stabilizes ssDNA; prevents re-annealing and secondary structures |
| Primase (DnaG) | Synthesizes short RNA primers (~10–12 nt) |
| DNA Pol III (core) | Main replicative polymerase; 5'→3' synthesis + 3'→5' proofreading |
| β-clamp | Processivity factor; tethers Pol III to template |
| γ-complex (clamp loader) | ATP-dependent loading of β-clamp |
| DNA Pol I | 5'→3' polymerase + 5'→3' exonuclease; removes primers, fills gaps |
| DNA Ligase | Joins Okazaki fragments; seals nicks (uses NAD⁺ in bacteria, ATP in eukaryotes) |
| Gyrase (Topo II) | Relieves positive supercoiling ahead of fork |

**Leading vs. Lagging Strand**

```
5' ←————————————————————— 3'    (template for lagging)
    ← Okazaki    ← Okazaki
              ↑ fork
    →  →  →  →  →  →  →  →
3' ——————————————————————→ 5'    (template for leading)
```

| Feature | Leading Strand | Lagging Strand |
|---------|---------------|----------------|
| Direction | Continuous synthesis (5'→3') | Discontinuous synthesis |
| Primers | One primer at start | One primer per Okazaki fragment |
| Okazaki fragments | None | ~1,000–2,000 nt each (bacteria); ~100–200 nt (eukaryotes) |
| Final steps | None needed | Pol I removes primers, fills gaps; ligase seals |

### Proofreading — 3'→5' Exonuclease

**Mechanism**

1. DNA Pol III incorporates a wrong nucleotide (e.g., T instead of C)
2. Mismatch distorts the primer terminus → slows extension
3. 3'→5' exonuclease activity (ε subunit of Pol III) excises the mismatched base
4. Polymerase re-incorporates the correct nucleotide

**Error Rates**
- Without proofreading: ~10⁻⁵ errors/bp
- With proofreading: ~10⁻⁷ errors/bp
- After MMR: ~10⁻¹⁰ errors/bp

**Key Distinction**
- **3'→5' exonuclease = proofreading** (removes last-added base; part of Pol III)
- **5'→3' exonuclease = primer removal** (part of DNA Pol I, not Pol III core)

### Termination

- *E. coli* chromosome is circular; bidirectional replication from oriC
- Forks converge at **Ter** sites
- **Tus protein** binds Ter sites and blocks DnaB helicase in one orientation (polar arrest)
- **Topoisomerase IV** decatenates the two interlinked daughter chromosomes

### Eukaryotic vs. Prokaryotic Replication (Key Differences)

| Feature | Prokaryotes | Eukaryotes |
|---------|------------|-----------|
| Chromosome | Circular | Linear |
| Origins | 1 (oriC) | Many (thousands per genome) |
| Main polymerase | DNA Pol III | DNA Pol δ (lagging), Pol ε (leading) |
| Primer removal | DNA Pol I | FEN1 + RNase H |
| Clamp | β-clamp | PCNA |
| Helicase | DnaB | MCM2-7 complex |
| Telomere problem | N/A | Telomerase extends 3' end |

---

## ⚠️ Exam Traps

- ❌ **"DNA Pol III can remove primers"** — No, DNA Pol I (5'→3' exonuclease) removes primers.
- ❌ **"Proofreading fixes all errors"** — Proofreading only checks the most recent base added; MMR corrects what escapes.
- ❌ **"DnaB helicase moves 3'→5'"** — DnaB translocates on the lagging strand template in the 5'→3' direction.
- ❌ **"Semiconservative means both old strands end up in the same daughter cell"** — No: each daughter gets one old + one new strand.

---

## Practice Questions

1. In the Meselson-Stahl experiment, if replication were dispersive, what pattern would you observe after 2 generations in ¹⁴N medium?

2. A temperature-sensitive mutation in DnaB prevents replication initiation at the restrictive temperature. Would this also affect elongation of already-initiated forks? Explain.

3. What would happen if a cell expressed a DNA Pol III with a defective 3'→5' exonuclease? How would mutation rate change, and how would the organism compensate?

4. Why does the lagging strand require multiple primers but the leading strand requires only one? Draw a diagram to support your answer.

5. Distinguish between the roles of DNA Pol I and DNA Pol III in DNA replication.

---

## Related Concepts

- [[Meselson-Stahl Experiment]]
- [[DNA Replication]]
- [[DNA Topology]] — supercoiling ahead of fork
- [[Mismatch Repair]] — corrects errors that escape proofreading
- [[Okazaki Fragments]]
