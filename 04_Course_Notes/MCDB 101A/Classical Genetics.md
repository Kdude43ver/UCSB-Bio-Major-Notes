# Classical Genetics

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## 🎯 Learning Objectives

1. Explain the one gene–one enzyme hypothesis and how nutritional mutants tested it
2. Perform biosynthetic pathway analysis using epistasis
3. Use deletion mapping to localize mutations in a genetic locus
4. Apply complementation testing to determine whether two mutations affect the same gene

---

## 🧠 Core Concepts

### One Gene–One Enzyme (Beadle & Tatum, 1941)
Irradiated *Neurospora crassa* spores → nutritional mutants (auxotrophs) that couldn't grow on minimal medium. Each mutant blocked one enzymatic step → each step = one enzyme = one gene.

**Pathway rescue logic:**
```
A → B → C → D → Z
     ↑    ↑    ↑
   gene1 gene2 gene3
```
- Add Z → growth ✓
- Add C, D, Z → growth; add B → no growth → block is at step B→C (gene2)

**Epistasis:** The mutant accumulating the earliest precursor is epistatic — it masks phenotypes of downstream mutants.

| Term | Definition |
|------|-----------|
| Auxotroph | Mutant requiring a supplement to grow |
| Prototroph | Wild-type; grows on minimal medium |
| Epistasis | One gene masks the phenotype of another |
| Minimal medium | Inorganic salts + carbon source only |

---

### Deletion Mapping (Benzer's rII System)
Fine-structure mapping within a single gene (rII locus of phage T4).

**Setup:** rII⁺ → small plaques on *E. coli* K; rII⁻ → large plaques on B, no growth on K.

**Strategy:**
1. Cross point mutant × deletion mutant
2. Mutation **inside** deleted region → no recombinants → no rII⁺ plaques on K
3. Mutation **outside** deleted region → recombinants appear → rII⁺ plaques on K

---

### Complementation Testing — The cis-trans Test
Tests whether two mutations are in the **same gene** (same complementation group).

**Trans configuration:**
```
m1  +
--  --    ← two chromosomes
 +  m2
```
- Different genes → wild-type phenotype ✓
- Same gene → mutant phenotype ✗

| Result | Interpretation |
|--------|---------------|
| Trans → WT | m1 and m2 are in **different genes** |
| Trans → mutant | m1 and m2 are in the **same gene** |
| Intragenic complementation | Rare; multimeric protein; misleading |

**cis vs. trans:**
- Operators, promoters → **cis-acting** (affect only genes on same DNA molecule)
- Repressors, activators → **trans-acting** (act on any copy in the cell)

---

### Key Experiments

| Experiment | Organism | Finding |
|-----------|----------|---------|
| Beadle & Tatum (1941) | *Neurospora crassa* | One gene–one enzyme |
| Benzer (1950s) | Phage T4 rII | Deletion mapping; cistron defined by cis-trans test |

---

## ⚠️ Exam Traps

- ❌ **"Complementation = recombination"** — Complementation is a functional test in *trans*; no recombination occurs
- ❌ **"Epistatic gene is upstream in the genome"** — Upstream in the *pathway*, not necessarily the chromosome
- ❌ **"Failing to complement = identical mutations"** — Same gene, but could be different mutations within it
- ❌ **"Intragenic complementation proves different genes"** — Rare exception; multimeric proteins can complement within one gene

---

## Practice Questions

1. A mutant can grow with citrulline or arginine, but not with ornithine. In which biosynthetic step is the block? Explain.
2. A point mutant crosses with Del1 (covers A1–A3): no plaques; Del2 (B1–B5): plaques; Del3 (A2–B2): no plaques. Where is the point mutation?
3. Two *trp*⁻ mutants fail to complement in trans. What does this tell you? What additional test could confirm allelism?

---

## Related Concepts
- [[Complementation Testing]]
- [[Deletion Mapping]]
- [[DNA Replication]]
- [[Mutations]]
