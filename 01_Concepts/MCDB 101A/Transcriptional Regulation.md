# Transcriptional Regulation

## Definition
Transcriptional regulation is the control of **when, how much, and under what conditions** a gene is transcribed. Bacteria regulate transcription primarily in response to nutrient availability and environmental conditions, allowing efficient use of cellular resources.

---

## Regulatory Logic: Key Distinctions

### Positive vs. Negative Regulation
| Type | Regulator | Default State | Activated by |
|------|-----------|---------------|-------------|
| **Negative** | Repressor | ON (basal transcription) | Inducer removes repressor from operator |
| **Positive** | Activator | OFF (no transcription) | Activator binds and recruits RNA Pol |

### Inducible vs. Repressible Systems
- **Inducible**: Gene is OFF by default; inducer molecule turns it ON (e.g., lac operon)
- **Repressible**: Gene is ON by default; corepressor turns it OFF (e.g., trp operon)

### Cis vs. Trans Elements
- **Cis-acting**: DNA sequences that regulate the gene on the **same chromosome** (operator, promoter) — cannot be complemented
- **Trans-acting**: Diffusible protein factors that can act on **either chromosome** in a diploid (repressors, activators) — can be complemented

---

## The Lac Operon (Negative + Positive Regulation)

### Structure
`lacI — P — O — lacZ — lacY — lacA`
- **lacI**: Constitutively expressed repressor gene (upstream, separate promoter)
- **P**: Promoter; **O**: Operator (overlaps promoter/TSS)
- **lacZ**: β-galactosidase (cleaves lactose)
- **lacY**: Lactose permease (imports lactose)
- **lacA**: Transacetylase (minor role)

### Negative Regulation — LacI Repressor
- **LacI** repressor binds the **operator** (O) → blocks RNA polymerase → no transcription
- **Allolactose** (isomer of lactose; made by trace β-galactosidase) = **inducer**
- Allolactose binds LacI → conformational change → LacI releases operator → transcription
- IPTG (isopropyl-β-D-thiogalactoside): gratuitous inducer used in lab (not metabolized)

### Positive Regulation — CAP (Catabolite Activator Protein / CRP)
- **Glucose effect (catabolite repression)**: When glucose is present, cAMP is LOW → CAP cannot activate lac operon
- When **glucose is absent**, adenylate cyclase is active → cAMP is HIGH → cAMP binds CAP → CAP-cAMP complex binds **CAP site** (upstream of −35) → recruits RNA Pol → strong transcription
- **Dual requirement**: lac operon is maximally expressed only when **lactose is present AND glucose is absent**

### Lac Operon Expression Summary
| Lactose | Glucose | cAMP | Repressor State | Transcription |
|---------|---------|------|----------------|---------------|
| − | + | Low | Bound (repressed) | None |
| + | + | Low | Released | Low |
| − | − | High | Bound (repressed) | None |
| + | − | High | Released | High (maximal) |

---

## Lac Operon Mutant Analysis

| Mutant | Phenotype | Cis/Trans | Explanation |
|--------|-----------|-----------|-------------|
| **I⁻** | Constitutive | Trans | No repressor → always ON |
| **Iˢ (super-repressor)** | Non-inducible | Trans | Cannot bind allolactose → always repressed |
| **O^c (operator constitutive)** | Constitutive | **Cis** | Repressor cannot bind O → always ON for genes downstream |
| **P⁻** | No expression | Cis | RNA Pol cannot bind |

**Key rule**: O^c is dominant over O⁺ **in cis** (affects only genes on same DNA molecule). I⁻ is recessive to I⁺ in trans (wild-type repressor from I⁺ can diffuse and repress O on both chromosomes). Iˢ is dominant (mutant repressor blocks both operators).

---

## The Trp Operon (Negative Regulation — Repressible)

### Structure
`trpR — [trpE trpD trpC trpB trpA]`
- Encodes enzymes for tryptophan biosynthesis
- **ON by default** (needed when Trp is absent)

### TrpR Repressor
- **Aporepressor (TrpR)**: Inactive alone — cannot bind operator
- **Corepressor (Trp)**: Tryptophan binds TrpR → active repressor → binds trp operator → represses transcription
- When Trp is absent: TrpR cannot bind → operon is expressed
- When Trp is high: TrpR-Trp complex binds → operon is off

---

## Attenuation (trp Operon)
A second level of regulation beyond repression:

### Mechanism
1. The **leader sequence** (trpL) upstream of trpE encodes a short leader peptide with **two Trp codons** (Trp-Trp)
2. A special **attenuator** region can form alternative mRNA secondary structures:
   - **Terminator hairpin** (3:4 stem-loop + U-run): causes premature transcription termination
   - **Anti-terminator hairpin** (2:3 stem-loop): prevents terminator formation → transcription continues

### Decision Logic (Coupling of transcription and translation)
| Trp level | Ribosome behavior | mRNA structure | Outcome |
|-----------|-------------------|----------------|---------|
| High Trp | Ribosome translates quickly through Trp codons; reaches region 2 before 3:4 forms | 3:4 terminator forms | **Termination (~90%)** |
| Low Trp | Ribosome stalls at Trp codons (no charged tRNA-Trp); region 1:2 pairs; frees 3 | 2:3 anti-terminator forms | **Read-through** |

Attenuation is a **translational sensor** for amino acid availability, layered on top of repressor regulation.

---

## Key Exam Points
- **Lac operon** = inducible, negatively regulated by LacI, positively regulated by CAP-cAMP
- **Glucose OFF + Lactose ON** = maximal lac expression
- O^c is cis-dominant; I⁻ is recessive; Iˢ is trans-dominant
- **trp operon** = repressible; TrpR alone is inactive (aporepressor); Trp is corepressor
- Attenuation: ribosome stalling at Trp codons → anti-terminator → read-through
- CAP-cAMP site is **upstream of the promoter** (positive activator)
- Operator is **downstream of promoter** (overlaps TSS in lac)

---

## Related Concepts
- [[Transcription]]
- [[Translation]]
- [[Mutations]]
- [[Transcriptional Regulation]]

## Prerequisites
- Transcription mechanism
- Protein-DNA interactions
- RNA secondary structure

## Importance: HIGH YIELD
Lac operon mutant analysis, CAP-cAMP glucose effect, cis/trans logic, and trp attenuation are all heavily tested on exams.
