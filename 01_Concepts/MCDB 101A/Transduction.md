# Transduction

## Definition
Transduction is a mechanism of **horizontal gene transfer** in which **bacteriophage** carry bacterial DNA from a donor cell to a recipient cell. The phage acts as an accidental vehicle, packaging host DNA instead of (or in addition to) its own genome. There are two types: **generalized transduction** (any gene can be transferred) and **specialized transduction** (only specific genes flanking a phage integration site are transferred).

---

## Generalized Transduction

### Mechanism
1. Phage infects donor bacterium → enters lytic cycle
2. **Pac site recognition**: Some phages (e.g., P22 in Salmonella, P1 in E. coli) package DNA using a **pac site** on their own genome to initiate packaging
3. **Headful packaging**: Phage terminase recognizes pac site, cuts DNA, packages a "headful" (~105% of phage genome) into the capsid
4. **Accidental packaging**: Sometimes the pac site-like sequence is found near chromosomal DNA, or the chromosome is fragmented and packaged non-specifically → **any region** of the bacterial chromosome can be encapsidated
5. Transducing phage injects **bacterial DNA** into recipient cell
6. Injected DNA undergoes **homologous recombination** with the recipient chromosome → gene stably inherited
7. Frequency: ~10⁻⁸ per phage

### Key Features
- **Any gene** in the genome can be transduced (equally likely)
- Transducing particles contain **only donor DNA** (no phage genome) → cannot replicate
- Requires **recombination** for stable integration in recipient

### Cotransduction
- If two genes are close enough (~1–2 min = ~20–40 kb for P1), they can be **co-packaged** and co-transduced
- **Cotransduction frequency** is inversely proportional to distance
- Used to determine **gene order and relative distances**
- Strategy: Cross transducing phage (carrying gene A) × recipient lacking genes A and B → measure % of A⁺ transductants that are also B⁺

#### Three-Point Cotransduction for Gene Order
If selecting for A⁺ transductants and scoring B and C:
- Gene order determined by which flanking marker is cotransduced more frequently with the selected gene

---

## Specialized Transduction

### Mechanism
Specialized transduction arises from **imprecise excision** of a **prophage** (integrated phage genome).

#### Lambda Phage as the Model
1. Lambda phage integrates (lysogeny) at **attB** site on E. coli chromosome using **integrase** and **IHF**
2. The attB site flanks **gal** (galactose utilization genes) on the left and **bio** (biotin biosynthesis genes) on the right
3. During **induction** (prophage excision):
   - **Normal excision**: Integrase + Xis remove the prophage precisely → free lambda
   - **Imprecise excision** (~10⁻⁶): Phage DNA loops out asymmetrically, including adjacent bacterial DNA → **transducing phage** (λdgal or λdbio)
4. **λdgal**: Contains **gal** genes but is missing some phage genes → defective (d = defective)
5. **λdbio**: Contains **bio** genes

### High-Frequency Transducing (HFT) Lysates
- If a lambda lysate contains λdgal particles, co-infect a gal⁻ recipient with **λdgal + wild-type helper lambda**
- Helper lambda provides missing functions in *trans*
- **HFT lysate**: Very high proportion (~50%) of transducing particles
- All gal⁺ transductants carry the same λdgal → **only gal or bio genes** can be transduced by lambda

---

## Generalized vs. Specialized Transduction Comparison

| Feature | Generalized Transduction | Specialized Transduction |
|---------|------------------------|------------------------|
| Phage examples | P1 (E. coli), P22 (Salmonella) | Lambda (λ) phage |
| Mechanism | Accidental headful packaging | Imprecise prophage excision |
| Genes transferred | **Any gene** in genome | **Only genes flanking attB** (gal, bio for lambda) |
| Frequency | ~10⁻⁸ per phage | ~10⁻⁶ per phage (low-frequency) |
| Phage DNA in particle | Usually only bacterial DNA | Phage DNA + adjacent bacterial DNA |
| Integration requirement | Yes (homologous recombination) | Can integrate via att sites |
| HFT lysates | No | Yes (after co-infection with helper) |
| Transducing particle replicates? | No (no phage genes) | Only with helper phage |

---

## Using Cotransduction for Gene Mapping

### Principle
- Cotransduction frequency **decreases** with increasing distance between genes
- ~2 genes within ~1–2 min on E. coli map can be cotransduced with P1

### Three-Point Cross Logic
To determine order of three genes (A, B, C) where B is in the middle:
1. Select for **A⁺** transductants → score B and C
2. Compare cotransduction frequencies: A⁺B⁺ vs A⁺C⁺
3. The gene **closer** to A is cotransduced more frequently
4. If A-B-C order, then: A⁺C⁺ frequency < A⁺B⁺ frequency

---

## Key Exam Points
- **Generalized**: pac site + headful packaging → **any gene** transferred; P1/P22 phage
- **Specialized**: imprecise lambda excision → **only gal or bio**; λdgal/λdbio
- Cotransduction ↑ = closer gene distance
- HFT lysate = enriched λd particles + helper phage → high-frequency specialized transduction
- Transducing particles in generalized transduction: **no phage genes** → cannot replicate, cannot cause lysis
- Distinguish transduction (phage-mediated) from transformation (naked DNA) and conjugation (pilus-mediated)

---

## Related Concepts
- [[Conjugation]]
- [[Plasmids]]
- [[Recombination]]
- [[Deletion Mapping]]
- [[Bacteriophage Lambda]]

## Prerequisites
- Bacteriophage lytic and lysogenic cycles
- Homologous recombination
- Gene mapping principles

## Importance: HIGH YIELD
Generalized vs. specialized transduction distinction, pac site/headful mechanism, cotransduction mapping logic, and HFT lysates are all exam-relevant.
