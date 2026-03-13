# Lac Operon

**Topic Area:** Gene Regulation
**Lecture:** [[Transcriptional Regulation]]
**Exam:** Midterm 2
**Importance:** HIGH YIELD ⭐⭐⭐

---

## One-Line Definition
The *lac* operon is a set of three genes (*lacZYA*) in *E. coli* controlled by both **negative regulation** (Lac repressor) and **positive regulation** (CRP-cAMP), allowing the cell to use lactose only when glucose is absent.

---

## Key Components

| Component | Type | Function |
|-----------|------|---------|
| *lacI* | Gene (separate) | Encodes Lac repressor tetramer |
| Lac repressor | Trans-acting protein | Binds operator → blocks RNAP |
| O1 (operator) | cis-acting DNA | Repressor binding site; overlaps TSS |
| *lacZ* | Structural gene | β-galactosidase; cleaves lactose |
| *lacY* | Structural gene | Lac permease; imports lactose |
| *lacA* | Structural gene | Transacetylase (minor role) |
| CRP site | cis-acting DNA | CRP-cAMP binding at −61 |
| Allolactose | Small molecule | True inducer; relieves repressor |
| cAMP | Small molecule | Activates CRP when glucose is low |

---

## Regulation Logic

### Negative Control (Repressor)
- **No lactose:** Repressor bound to O1 → operon OFF
- **Lactose present:** Allolactose (made by basal β-gal) binds repressor → conformational change → repressor off DNA → operon ON

### Positive Control (CRP-cAMP)
- **Glucose present:** Low cAMP → CRP inactive → operon low
- **Glucose absent:** High cAMP → CRP-cAMP binds at −61 → recruits RNAP α-CTD → operon high

### Full Expression Table
| Glucose | Lactose | Expression |
|---------|---------|-----------|
| + | − | Off |
| + | + | Low |
| − | − | Off |
| **−** | **+** | **Maximum** |

---

## Mutant Analysis (High Yield)

| Mutant | Effect | cis or trans? | Dominance |
|--------|--------|--------------|-----------|
| *lacI*⁻ | No repressor → constitutive ON | Trans | Recessive |
| *lacI*^s | Repressor can't bind allolactose → always OFF | Trans | Dominant |
| *lacO*^c | Operator can't bind repressor → constitutive ON | **Cis** | Cis-dominant |
| *lacZ*⁻ | No β-galactosidase | Trans | Recessive |

---

## Analogy
The Lac operon is like a vending machine that only dispenses lactose-metabolizing enzymes when lactose is present **and** glucose is absent. The repressor is a physical lock; CRP-cAMP is an amplifier that cranks up the signal when the better fuel (glucose) runs out.

---

## Connections
- [[Catabolite Repression]] — CRP-cAMP positive control
- [[Transcription Attenuation]] — alternative regulatory mechanism (Trp operon)
- [[Bacteriophage Lambda]] — another genetic switch using repressor logic
- [[Transcriptional Regulation]]
