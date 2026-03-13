# Molecular Techniques

**Course:** [[Course Dashboard]] | **Yield:** MEDIUM ⭐⭐

---

## 🎯 Learning Objectives

1. Describe the PCR reaction: components, thermocycling steps, and exponential amplification logic
2. Explain how gel electrophoresis separates DNA fragments and how to interpret a gel
3. Compare Sanger sequencing and next-generation sequencing (NGS) methods
4. Describe Southern blotting and its applications
5. Explain how restriction enzymes are used in cloning and mapping

---

## 🧠 Core Concepts

### Polymerase Chain Reaction (PCR)

**Components**

| Component | Role |
|-----------|------|
| Template DNA | Contains the target sequence |
| Forward primer (5'→3') | Anneals to bottom strand; defines left boundary |
| Reverse primer (5'→3') | Anneals to top strand; defines right boundary |
| dNTPs (dATP, dCTP, dGTP, dTTP) | Building blocks for new strand |
| **Taq polymerase** | Thermostable DNA polymerase (from *Thermus aquaticus*); active at 72°C; no 3'→5' proofreading |
| MgCl₂ | Cofactor for Taq polymerase |
| Buffer | Maintains pH |

**Thermocycling Steps (1 Cycle)**

1. **Denaturation (94–98°C, ~30 sec):** Heat melts dsDNA → ssDNA templates
2. **Annealing (50–65°C, ~30 sec):** Primers bind their complementary sequences on template
3. **Extension (72°C, ~1 min/kb):** Taq extends from 3' end of primers in 5'→3' direction

**Amplification Kinetics**

- Cycles 1–2: Long products (extend past target)
- Cycle 3+: Short, **defined-length products** between the two primers
- After n cycles: up to **2ⁿ copies** of the target; exponential amplification

**Key Applications**

- Diagnostic PCR (detect pathogen DNA)
- RT-PCR (first reverse-transcribe RNA → cDNA, then PCR)
- Quantitative PCR (qPCR) — real-time fluorescence to quantify template
- Mutagenesis (introduce mutations via mismatched primers)
- Cloning (amplify insert for ligation)

**Taq vs. Proofreading Polymerases**

- **Taq:** Fast, no proofreading → ~1 error per 10⁵ bp; sufficient for most applications
- **Phusion/Q5:** Have 3'→5' proofreading exonuclease → error rate ~10⁻⁶/bp; use when accuracy matters (cloning, sequencing prep)

### Gel Electrophoresis

**Principle**

- DNA is negatively charged (phosphate backbone) → migrates toward + pole in electric field
- Agarose gel acts as molecular sieve: **smaller fragments migrate faster**
- Ethidium bromide (EtBr) or SYBR Green intercalates into DNA → fluorescent under UV

**Reading a Gel**

```
Wells (top)
  |   Ladder   Sample1  Sample2
  |   10 kb ──────────────────
  |    5 kb ──────────────────
  |    2 kb ──────────────────
  |    1 kb ──────────────────
  |  500 bp ──────────────────
  ↓ Migration direction (+)
```
- Compare band position to DNA ladder (size standards) to estimate fragment size
- Band intensity ∝ amount of DNA (useful for comparing quantities)

**Agarose % and Resolution**

| % Agarose | Best for |
|-----------|---------|
| 0.8% | Large fragments (2–20 kb) |
| 1–1.5% | Standard (200 bp–10 kb) |
| 2–3% | Small fragments (<500 bp) |

**Pulse-Field Gel Electrophoresis (PFGE)**

For very large DNA (chromosomes, >50 kb); alternating electric field allows separation.

### Restriction Enzymes

**Types**

- **Type II:** Cut within or near recognition sequence; produce defined fragments; used in cloning
- Recognition sequences are typically **palindromic** 4–8 bp sequences

**Cut Types**

| Enzyme | Sequence | Cut Type |
|--------|---------|---------|
| EcoRI | 5'-G↓AATTC-3' | 5' overhang (sticky ends) |
| BamHI | 5'-G↓GATCC-3' | 5' overhang |
| SmaI | 5'-CCC↓GGG-3' | Blunt end |
| PstI | 5'-CTGCA↓G-3' | 3' overhang |

**Restriction Mapping**

1. Digest DNA with enzyme A alone, enzyme B alone, and A+B double digest
2. Resolve fragments on gel; measure sizes
3. Deduce restriction site positions from additive fragment sizes

### DNA Sequencing

**Sanger Sequencing (Chain Termination)**

**Components:**
- Template ssDNA
- Primer
- DNA Pol (Klenow or Taq)
- dNTPs + small amounts of each **ddNTP** (dideoxynucleotide — lacks 3'-OH; terminates chain)

**Mechanism:**
1. Extension proceeds normally until a ddNTP is incorporated → chain terminates
2. Produces a nested set of fragments, each ending with a specific ddNTP
3. Modern: fluorescent ddNTPs (each base labeled a different color) → capillary electrophoresis → sequence read by laser

**Read length:** ~500–1,000 bp per reaction

**Next-Generation Sequencing (NGS) — Overview**

- **Illumina (by synthesis):** Library prep → cluster amplification on flow cell → sequencing by synthesis with reversible fluorescent terminators → 150–300 bp reads; massively parallel (billions of reads)
- **PacBio (SMRT):** Single-molecule real-time sequencing; long reads (10–20 kb); useful for resolving repeats
- **Oxford Nanopore:** Single-molecule sequencing through a pore; longest reads (>1 Mb); portable

### Southern Blotting

**Steps**

1. Digest genomic DNA with restriction enzyme
2. Separate by gel electrophoresis
3. Denature gel (NaOH) → ssDNA
4. **Transfer** DNA to nitrocellulose/nylon membrane (blotting)
5. **Hybridize** with labeled probe (complementary to gene of interest)
6. Wash off non-specific probe; detect by autoradiography or chemiluminescence

**Applications**

- Detect specific gene sequences in a complex genome
- RFLP (restriction fragment length polymorphism) analysis → genotyping
- Confirm gene knockouts/insertions

**Northern and Western Blotting**

| Blot | Molecule | Separated by | Probe/Detection |
|------|---------|-------------|----------------|
| Southern | DNA | Size (agarose gel) | DNA probe |
| Northern | RNA | Size (denaturing gel) | DNA/RNA probe |
| Western | Protein | Size (SDS-PAGE) | Antibody |

---

## ⚠️ Exam Traps

- ❌ **"Taq polymerase has proofreading activity"** — Taq lacks 3'→5' exonuclease; use high-fidelity polymerases for accurate amplification.
- ❌ **"Gel electrophoresis separates by charge"** — All DNA has the same charge-to-mass ratio; separation is by **size** through the gel matrix.
- ❌ **"Southern blotting detects protein"** — Southern = DNA; Northern = RNA; Western = protein.

---

## Practice Questions

1. Design a PCR experiment to detect whether a bacterial strain carries a specific antibiotic resistance gene. What would positive and negative controls look like on the gel?

2. A restriction digest with EcoRI gives bands of 4 kb, 2 kb, and 1 kb. With HindIII, bands are 5 kb and 2 kb. The double digest gives 3 kb, 2 kb, 1 kb, and 1 kb. Draw a restriction map consistent with these data.

3. Why does Sanger sequencing use ddNTPs rather than dNTPs for chain termination? What feature of ddNTPs causes termination?

4. In Southern blotting, why is it necessary to denature the DNA before transfer to the membrane?

5. You perform PCR with a thermostable polymerase that lacks 3'→5' exonuclease activity and get a product of the correct size but incorrect sequence. What likely happened, and how would you fix it?

---

## Related Concepts

- [[PCR]]
- [[Molecular Techniques]]
- [[Molecular Techniques]]
- [[Molecular Techniques]]
- [[DNA Replication]] — PCR mimics in vitro replication
- [[Mutations]] — PCR-based mutagenesis
