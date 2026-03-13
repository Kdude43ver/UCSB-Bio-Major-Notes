# Plasmids

## Definition
Plasmids are **extrachromosomal, circular, double-stranded DNA molecules** that replicate **autonomously** (independently of the bacterial chromosome). They typically encode genes that provide a **selective advantage** under specific conditions (antibiotic resistance, toxin production, metabolic pathways). Plasmids are not generally essential for normal growth but are maintained because they confer fitness benefits.

---

## Key Properties of Plasmids

| Property | Description |
|----------|-------------|
| **Size** | 1 kb – >200 kb (most: 2–100 kb) |
| **Replication** | Autonomous; independent of chromosomal replication |
| **Origin of Replication (oriV)** | Required for autonomous replication; determines copy number and host range |
| **Copy number** | Low copy (1–5 per cell) or high copy (20–700 per cell) |
| **Maintenance** | Requires partitioning (par) system for stable inheritance at low copy numbers |
| **Transfer** | Many plasmids can be transferred by conjugation (if they have oriT + tra genes) |

---

## Replication Control and Copy Number

### High-Copy Plasmids (e.g., ColE1, pUC19)
- Replicate many times per cell cycle
- Use RNA I / RNA II regulatory mechanism (antisense RNA inhibits primer RNA processing)
- Do not require active partitioning — randomly distributed to daughters (sufficient copies to guarantee both get at least one)

### Low-Copy Plasmids (e.g., F factor, P1 prophage)
- Replicate once per cell cycle (like chromosome)
- Require **par (partitioning) genes** to ensure one copy to each daughter cell
- Par system includes centromere-like sequence + ATPase-driven segregation machinery

---

## Plasmid Classification

### By Function / Phenotype Conferred

| Plasmid Type | Genes Carried | Example |
|-------------|--------------|---------|
| **F (Fertility) plasmid** | tra genes (conjugation), oriT | F factor in E. coli |
| **R factors** | Antibiotic resistance genes (aac, tet, kan, amp, etc.) | pBR322, R100 |
| **Col plasmids** | Colicin (bacteriocin) genes | ColE1 |
| **Virulence plasmids** | Toxins, adhesins | pO157 (E. coli O157); Ti plasmid (Agrobacterium) |
| **Metabolic plasmids** | Degradation pathways | TOL plasmid (toluene catabolism) |

### By Mobility
- **Conjugative plasmids**: Encode their own transfer machinery (tra genes + oriT); can transfer without help
- **Mobilizable plasmids**: Have oriT but lack complete tra; can be mobilized by a conjugative plasmid in the same cell
- **Non-mobilizable**: Lack oriT; cannot be transferred by conjugation

---

## The F Factor (Detailed)

See [[Conjugation]] for full conjugation details. Key structural features:
- **oriV**: Vegetative replication origin
- **oriT**: Transfer origin (nicked by TraI relaxase to initiate rolling circle replication)
- **tra operon**: ~25 genes encoding pilus biosynthesis, mating pair stabilization, DNA transfer
- **IS elements** (IS2, IS3, IS10, Tn1000/γδ): Enable integration into chromosome via homologous recombination with IS elements on chromosome → **Hfr formation**

### F Factor States
- **F⁺**: Autonomous plasmid → transfers F to F⁻ cells
- **Hfr**: Integrated → transfers chromosomal DNA
- **F'**: F + chromosomal genes (from imprecise excision) → used for complementation analysis

---

## Antibiotic Resistance Plasmids (R Factors)

### Importance
- R factors carry genes for **antibiotic resistance enzymes**: β-lactamases (cleave penicillin ring), acetyltransferases (inactivate aminoglycosides), efflux pumps, methylases (ribosome modification)
- Transfer between bacteria via **conjugation** → major driver of the antibiotic resistance crisis
- R factors can carry **multiple resistance genes** on integrons or transposons
- Can transfer between species (broad host range plasmids)

### Examples
| Resistance Gene | Antibiotic | Mechanism |
|----------------|-----------|-----------|
| bla (TEM β-lactamase) | Ampicillin | Hydrolyzes β-lactam ring |
| tet | Tetracycline | Efflux pump |
| kan | Kanamycin | Aminoglycoside acetyltransferase |
| cat | Chloramphenicol | Acetyltransferase |

---

## Incompatibility Groups

- Two plasmids of the **same incompatibility (Inc) group** cannot stably coexist in the same cell
- Reason: They share the same replication control system → compete for replication/partitioning → one is randomly lost
- Different Inc groups → stable coexistence (different replication origins, different partition systems)
- Plasmids are classified: IncF, IncI, IncP, IncQ, IncW, etc.

---

## Plasmids as Cloning Vectors

Essential features of a cloning vector:
1. **Origin of replication (ori)** — autonomous replication in host
2. **Selectable marker** — antibiotic resistance (ampR, kanR) for selecting transformed cells
3. **Multiple Cloning Site (MCS)** — unique restriction sites for inserting foreign DNA
4. **Small size** — efficient transformation and handling

### Examples
| Vector | Size | Features |
|--------|------|---------|
| pBR322 | 4.4 kb | ampR, tetR; classic vector |
| pUC19 | 2.7 kb | ampR, lacZα (blue-white selection); MCS |
| pBAD | Variable | Arabinose-inducible expression |

---

## Key Exam Points
- Plasmids replicate **autonomously** via their own ori (oriV)
- F factor: tra genes + oriT for transfer; IS elements for chromosomal integration
- **Incompatibility**: same-Inc plasmids cannot coexist → lost by segregation
- R factors spread antibiotic resistance by conjugation — clinically critical
- Low-copy plasmids require **par genes** for stable segregation; high-copy plasmids do not
- oriT = transfer origin (conjugation); oriV = vegetative origin (autonomous replication)
- F' plasmid used to create **merodiploids** for complementation analysis

---

## Related Concepts
- [[Conjugation]]
- [[Transduction]]
- [[Recombination]]
- [[Transcriptional Regulation]]

## Prerequisites
- Bacterial DNA replication
- Conjugation mechanism
- Restriction enzymes and cloning basics

## Importance: HIGH YIELD
F factor biology, plasmid incompatibility, R factor resistance mechanisms, and the distinction between oriT and oriV are exam-tested.
