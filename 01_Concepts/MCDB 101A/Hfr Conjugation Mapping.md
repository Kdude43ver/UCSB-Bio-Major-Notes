# Hfr Conjugation and Gene Mapping

**Topic Area:** Bacterial Genetics
**Lecture:** [[Gene Transfer]]
**Exam:** Final
**Importance:** HIGH YIELD ⭐⭐⭐

---

## One-Line Definition
Hfr (high-frequency recombination) strains have the F plasmid integrated into the chromosome; during conjugation they transfer chromosomal genes **in a defined linear order** starting from oriT, allowing gene order and distance to be mapped by interrupted mating.

---

## How Hfr Forms
F plasmid integrates into the chromosome via RecA-dependent recombination at IS elements → F is now part of the chromosome → transfer begins at oriT within the integrated F.

---

## Transfer Mechanics
- **Rolling circle replication** at oriT: one strand is nicked; 5' end enters recipient
- Chromosomal genes enter the recipient in order from oriT, carried by the replicating strand
- Complete transfer (~100 min) is rare → genes near the distal end of F are almost never transferred → **recipient stays F⁻**

---

## Interrupted Mating
1. Mix Hfr × F⁻ strains
2. At timed intervals, separate pairs (blender)
3. Plate on selective media for each donor marker
4. **Time of entry = chromosomal position** relative to oriT

**1 min of transfer ≈ 47 kb**

### Example Entry Order
```
oriT → thr (8') → leu (9') → azi (11') → ton (11.5') → lac (25') → ...
```
→ Gene order: thr–leu–azi–ton–lac

---

## Key Rules (from NLM)
- Recipient is **almost always F⁻** after Hfr mating — F trailing end is transferred last
- Transferred DNA must integrate by **homologous recombination** (RecA-dependent); requires an **even number of crossovers** — odd number is lethal (breaks the circular chromosome)
- Transfer polarity: orientation of integrated F determines which genes go first (clockwise vs. counterclockwise)

---

## Building the Complete Map
Use multiple Hfr strains with F integrated at different positions/orientations → combine entry time data → assemble complete circular map of *E. coli* chromosome (100 min total)

---

## Comparison: F⁺ vs. Hfr × F⁻

| Feature | F⁺ × F⁻ | Hfr × F⁻ |
|---------|---------|---------|
| What transfers efficiently | F plasmid itself | Chromosomal genes |
| Recipient becomes | F⁺ (almost always) | F⁻ (almost always) |
| Chromosomal gene transfer | Rare | High frequency (Hfr = high frequency recombinant) |

---

## Connections
- [[Conjugation]]
- [[Transduction]] — alternative mapping method using cotransduction frequencies
- [[Recombination]] — transferred DNA integrates by HR
- [[Gene Transfer]]
