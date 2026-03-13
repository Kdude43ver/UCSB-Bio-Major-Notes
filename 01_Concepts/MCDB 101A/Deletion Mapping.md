# Deletion Mapping

## Definition
Deletion mapping is a genetic technique that uses **deletion mutants** (strains missing a defined segment of DNA) to rapidly assign point mutations to specific regions of a gene. Because deletions cannot revert to wild-type by a single mutational event, recombination between a deletion and a point mutant can only produce wild-type recombinants if the point mutation falls **outside** the deleted region.

---

## Why Deletions Cannot Revert
A deletion removes one or more base pairs entirely. There is no intact sequence for back-mutation to restore. This means:
- A deletion strain will always be mutant phenotype (e.g., rII⁻)
- Crossing two deletion mutants only gives wild-type recombinants if the deletions **do not overlap**

---

## The rII System (Benzer, T4 Phage)
Seymour Benzer used the **rII locus** of bacteriophage T4 to fine-structure map a gene at single base-pair resolution.

### Why rII?
- **Wild-type (r⁺)** phage form **small, turbid** plaques on both E. coli B and E. coli K
- **rII mutants** form **large, clear** plaques on E. coli B, but **cannot grow** on E. coli K (λ lysogen)
- This differential host range provides an extremely sensitive selection for rare wild-type recombinants

### rII Gene Structure
- rII locus has two adjacent genes: **rIIA** and **rIIB**
- Deletions of defined segments were mapped to create a reference deletion map
- Each deletion was assigned to a region (e.g., A1, A2, B1, B2, etc.)

---

## Logic of Deletion Mapping

### Deletion × Point Mutant Cross
1. Cross deletion strain × point mutant strain on E. coli B (permissive host)
2. Plate on E. coli K (selective host)
3. **Wild-type recombinants appear** → point mutation is **outside** the deleted region
4. **No wild-type recombinants** → point mutation is **within** the deleted region

### Deletion × Deletion Cross
- Cross two deletion mutants
- If recombination can produce a chromosome with a segment covered by **neither** deletion → wild-type recombinants possible (deletions **do not overlap**)
- If deletions overlap → no wild-type recombinants possible

### Summary Table
| Cross Result | Interpretation |
|-------------|----------------|
| + (recombinants seen) | Deletions/mutations **do not overlap** |
| 0 (no recombinants) | Deletions/mutations **overlap** |

---

## Two-Step Mapping Strategy

**Step 1**: Cross point mutant against a **panel of large deletions** covering different regions of the gene → narrows mutation to a segment in ~5 crosses

**Step 2**: Cross point mutant against **smaller deletions** within that segment → localizes to sub-segment

This "Rule of Two" approach localizes any point mutation with far fewer crosses than pairwise point-by-point mapping.

---

## Reading a Deletion Map Matrix

A matrix shows crosses between multiple deletions or point mutants:
- Rows = one set of mutants; Columns = another
- + = recombinants observed (no overlap)
- 0 = no recombinants (overlap or same region)

Use the pattern of 0s to define minimal overlapping regions → assign mutants to intervals.

---

## Cis-Trans Test (Complementation) vs. Deletion Mapping

| Feature | Deletion Mapping | Cis-Trans / Complementation |
|---------|-----------------|---------------------------|
| Purpose | Localize mutations within a gene | Determine if mutations are in same or different genes |
| Measures | Recombination frequency | Functional complementation |
| Requires | Recombination | Diploid or merodiploid |
| Deletions used | Yes | Not required |

Deletion mapping is **intragenic** (maps position within one gene); complementation tests **intergenic** (tests if two mutations are in the same gene).

---

## Key Exam Points
- Deletions **cannot revert** — critical premise of the entire technique
- 0 recombinants = overlap; + recombinants = no overlap
- rII system: grows on E. coli B (permissive), cannot grow on E. coli K (selective)
- Two-step strategy: large deletions first → narrow to segment → fine-map with small deletions
- Deletion mapping = **recombination-based** (not complementation)
- Distinguish from **cis-trans test**: deletion mapping maps position; cis-trans tests gene identity

---

## Related Concepts
- [[Recombination]]
- [[Mutations]]
- [[Transduction]]
- [[Bacteriophage Lambda]]

## Prerequisites
- Recombination basics
- Bacteriophage life cycle
- Concept of genetic mapping

## Importance: HIGH YIELD
Benzer/rII system, the logic of 0 vs. + results, and distinguishing deletion mapping from complementation are all high-frequency exam topics.
