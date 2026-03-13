# Conjugation

## Definition
Conjugation is a mechanism of **horizontal gene transfer** in bacteria that requires **direct cell-to-cell contact** via a pilus. The F (fertility) factor — a plasmid carrying genes for its own transfer — drives conjugation in *E. coli*. It is the only form of bacterial gene transfer that can move large segments of chromosomal DNA.

---

## The F (Fertility) Factor

### Structure
- ~100 kb circular plasmid
- **tra genes**: ~25 genes encoding the mating pilus and conjugation machinery (tra operon)
- **oriT**: Origin of transfer — where rolling circle replication initiates during conjugation
- **oriV**: Origin of vegetative replication (autonomous replication of F plasmid)
- **IS elements** (IS2, IS3, IS10, Tn1000/γδ): Insertion sequences enabling integration into chromosome via homologous recombination

### Donor Cell Types
| Cell Type | F Factor Status | Transfer During Mating |
|-----------|----------------|----------------------|
| **F⁺** | F plasmid (autonomous) | Transfers F plasmid to F⁻ |
| **Hfr** | F integrated into chromosome | Transfers chromosomal DNA |
| **F'** | F plasmid carrying chromosomal DNA | Transfers chromosomal genes at high frequency |

---

## F⁺ × F⁻ Mating

1. F⁺ cell produces **conjugative pilus** (encoded by *traA*)
2. Pilus extends, contacts F⁻ cell → forms **mating junction**
3. **Relaxase (TraI)** nicks the F plasmid at **oriT**
4. **Rolling circle replication**: one strand of F is transferred 5'→3' through the mating junction
5. F⁻ recipient synthesizes complementary strand → becomes **F⁺**
6. **Outcome**: F⁻ becomes F⁺; **no chromosomal genes transferred**

---

## Hfr × F⁻ Mating

### How Hfr Strains Form
- F factor integrates into the **bacterial chromosome** via **IS-mediated recombination** between IS elements on F and identical IS elements on the chromosome
- Integration is **reversible** (rare excision events can regenerate F⁺ or F' cells)

### Transfer Mechanism
1. **Relaxase** nicks at **oriT** within integrated F
2. Rolling circle replication transfers chromosome starting from oriT → chromosomal DNA enters F⁻ cell in linear fashion
3. Genes are transferred in order of their position on the chromosome, starting from **oriT**
4. **F⁻ rarely becomes F⁺**: the F sequence is split — leading F genes transfer first; the remaining F tail enters last (~100 min for entire chromosome)
5. **Mating is usually interrupted** before the full chromosome transfers → F⁻ recipient gets chromosomal DNA but rarely the complete F factor → remains F⁻

### Recombination in Recipient
- Transferred ssDNA is converted to dsDNA in recipient
- **Homologous recombination** integrates donor chromosomal segment into F⁻ chromosome
- Results in **merodiploid** (partially diploid) for transferred region

---

## Interrupted Mating & Time-of-Entry Mapping

### Experiment (Jacob & Wollman, ~1955)
1. Mix Hfr × F⁻ at time 0
2. At various time points, **agitate** (Waring blender) to interrupt mating
3. Plate on selective media to detect which donor markers appeared in recipients
4. Plot: marker appearance vs. time → **time-of-entry map**

### Principles
- Genes enter in order of their distance from oriT
- 1 minute ≈ ~20 kb (approximately)
- E. coli chromosome ≈ 100 min map
- **Gene order** = sequence of appearance; **distance** = time difference between appearances

### Example
If genes A, B, C appear at 5, 10, 20 min respectively → gene order: oriT—A—B—C; distances: A–B = 5 min, B–C = 10 min

---

## F' (F-prime) Factors and Sexduction

### Formation
- **Imprecise excision** of integrated F factor → loop out includes adjacent chromosomal DNA
- Results in F' plasmid carrying chromosomal genes + missing some F genes (occasionally)

### Sexduction (F-duction)
- F' cell mates with F⁻ → transfers chromosomal genes at **very high frequency** (nearly 100%)
- Recipient becomes **merodiploid** for genes on F'
- Used to construct **partial diploids** for **complementation analysis** (cis-trans tests)

---

## Plasmid Types Transferred by Conjugation

| Plasmid | Relevant Genes Transferred | Significance |
|---------|--------------------------|--------------|
| F factor | F⁺ genes; sometimes chromosomal | Gene mapping; generating merodiploids |
| R factors (resistance plasmids) | Antibiotic resistance genes | **Clinical significance**: spreads multidrug resistance |
| Col plasmids | Colicin genes | Bacteriocin production |
| Ti plasmid (Agrobacterium) | T-DNA → plant cells | Genetic engineering of plants |

---

## Comparison: Conjugation vs. Other Gene Transfer

| Feature | Conjugation | Transformation | Transduction |
|---------|-------------|---------------|-------------|
| Mechanism | Cell contact, pilus | Naked DNA uptake | Bacteriophage |
| DNA size transferred | Large (entire chromosome possible) | Small (plasmids or fragments) | ~1 phage genome (~50 kb) |
| Requires live donor | Yes | No | No |
| F factor needed | Yes (donor) | No | No |
| Frequency | Moderate | Low–moderate | Low (~10⁻⁸) |

---

## Key Exam Points
- **F⁺ × F⁻**: F plasmid transferred; recipient becomes F⁺; no chromosomal genes transferred
- **Hfr × F⁻**: Chromosomal DNA transferred beginning at oriT; F⁻ **rarely** becomes F⁺ (F tail enters last)
- Gene order on chromosome = order of entry in interrupted mating experiments
- **1 minute ≈ ~20 kb** in E. coli conjugation mapping
- F' formed by **imprecise excision** of Hfr; used for complementation analysis
- IS elements mediate F integration into chromosome → Hfr formation
- **R factors** spread antibiotic resistance via conjugation — major clinical concern

---

## Related Concepts
- [[Plasmids]]
- [[Transduction]]
- [[Recombination]]
- [[Transcriptional Regulation]]

## Prerequisites
- Bacterial chromosome structure
- Plasmid biology
- Recombination basics
- Genetic mapping principles

## Importance: HIGH YIELD
F⁺/Hfr/F' distinctions, interrupted mating logic, time-of-entry mapping, and F' complementation are all heavily tested topics.
