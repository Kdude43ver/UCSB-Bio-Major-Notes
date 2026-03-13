# DNA Structure

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## 🎯 Learning Objectives

1. Describe the key features of the Watson-Crick double helix model
2. Apply Chargaff's rules to determine base composition from a given strand
3. Define linking number (L), twist (T), and writhe (W) and use the equation L = T + W
4. Explain thermal denaturation and its dependence on GC content

---

## 🧠 Core Concepts

### The Double Helix — Watson & Crick (1953)

**Structural Features**

| Feature | Value/Description |
|---------|-----------------|
| Helix type | Right-handed (B-form under physiological conditions) |
| Base pairs per turn | 10.5 |
| Rise per base pair | 3.4 Å |
| Diameter | 20 Å (2 nm) |
| Grooves | Major groove (wider, protein binding) and minor groove |
| Strand orientation | Antiparallel (5'→3' on one strand, 3'→5' on other) |

**Key Evidence**
- **X-ray crystallography (Franklin & Wilkins):** 3.4 Å repeat within helix, 34 Å per full turn
- **Chargaff's rules:** [A] = [T], [G] = [C] in double-stranded DNA
- **Density gradient analysis (Meselson-Stahl):** DNA is a defined molecule amenable to density-based separation

**Base Pairing**
- **A–T:** 2 hydrogen bonds
- **G–C:** 3 hydrogen bonds (GC-rich DNA is more stable)

### Chargaff's Rules

**Statement**

In any double-stranded DNA:
- [A] = [T]
- [G] = [C]
- [A] + [G] = [T] + [C] (purines = pyrimidines)
- [A] + [T] + [G] + [C] = 100%

**Application**

Given: one strand is 30% A, 20% G, 25% C, 25% T
- Complementary strand: 30% T, 20% C, 25% G, 25% A
- Whole molecule: [A] = [T] = (30+25)/2 = 27.5%, [G] = [C] = (20+25)/2 = 22.5%

### DNA Topology: L = T + W

**Definitions**

| Symbol | Name | Definition |
|--------|------|-----------|
| **L** | Linking number | Number of times one strand crosses the other; topological invariant |
| **T** | Twist | Number of helical turns in the DNA |
| **W** | Writhe | Number of times the helix axis crosses itself in 3D space |

**The Equation**

$$L = T + W$$

- **Relaxed circular DNA:** W = 0, so L = T
- **Negatively supercoiled:** L < T₀ (underwound; W < 0) — common in cells
- **Positively supercoiled:** L > T₀ (overwound; W > 0) — forms ahead of replication fork

**Topoisomerases**

| Enzyme | Mechanism | Effect |
|--------|-----------|--------|
| Topoisomerase I | Cuts one strand, rotates, reseals | Changes L by ±1 per cycle |
| Topoisomerase II (Gyrase) | Cuts both strands, passes another segment, reseals | Changes L by ±2; introduces negative supercoils (ATP-dependent) |

**DNA Gyrase** (bacterial): introduces negative supercoils; target of fluoroquinolone antibiotics (ciprofloxacin).

### Thermal Denaturation (DNA Melting)

**Tm (Melting Temperature)**

The temperature at which 50% of DNA is single-stranded.

**Determinants of Tm:**
1. **GC content:** Each G-C pair has 3 H-bonds vs. 2 for A-T → GC-rich DNA has higher Tm
2. **Salt concentration:** Higher [Na⁺] stabilizes DNA (shields phosphate repulsion) → higher Tm
3. **DNA length:** Longer DNA has higher Tm
4. **Formamide/urea:** Denaturants lower Tm

**Formula (approximate):**

$$T_m \approx 69.3 + 0.41 \times (\% GC)°C$$

**Hyperchromic Effect**

As DNA melts, absorbance at 260 nm increases (~40%) — stacked bases absorb less than unstacked bases. This is used to monitor denaturation spectrophotometrically.

### DNA Forms

| Form | Conditions | Features |
|------|-----------|---------|
| B-DNA | Aqueous, physiological | Major form; right-handed; 10.5 bp/turn |
| A-DNA | Low humidity | Right-handed; 11 bp/turn; shorter, wider |
| Z-DNA | High salt, GC-rich alternating sequences | Left-handed; 12 bp/turn |

---

## ⚠️ Exam Traps

- ❌ **"Chargaff's rules apply to all DNA"** — They apply to double-stranded DNA only. Single-stranded DNA or RNA can have [A] ≠ [T].
- ❌ **"Linking number can be changed by stretching DNA"** — L is a topological invariant; only strand nicking changes it.
- ❌ **"A-T pairs are always destabilizing"** — While A-T has fewer H-bonds, stacking energy also matters significantly.
- ❌ **"Gyrase is a type I topoisomerase"** — Gyrase is a type II topoisomerase that uses ATP.

---

## Practice Questions

1. A double-stranded DNA molecule is 42% G + C. What percentage is A? What is the approximate Tm?

2. A relaxed circular DNA has L₀ = 400. After treatment with gyrase, L = 390. What type of supercoiling was introduced? What is the writhe now?

3. Why does RNA form less stable duplexes than DNA of the same sequence and length? (Hint: consider 2'-OH and base stacking.)

4. You are given a single-stranded DNA with the sequence 5'-ATGCGGTAT-3'. What is the sequence of the complementary strand? What are the %A, %T, %G, %C in the double-stranded form?

---

## Related Concepts

- [[DNA Topology]]
- [[DNA Structure]]
- [[DNA Replication]] — must unwind supercoiled DNA
- [[DNA Topology]]
