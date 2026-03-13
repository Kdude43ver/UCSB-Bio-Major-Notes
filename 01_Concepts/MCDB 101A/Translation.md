# Translation

## Definition
Translation is the process where genetic information encoded in mRNA is decoded to generate a linear sequence of amino acids forming a protein. It is the final step of the **Central Dogma** (DNA → RNA → Protein). In rapidly growing bacteria, up to 80% of a cell's energy is dedicated to protein synthesis.

---

## The Genetic Code

- **Codons**: 3-nucleotide units in mRNA specifying an amino acid or stop signal
- **64 codons total** encode only 20 amino acids → the code is **degenerate** (redundant)
- **AUG**: Universal start codon; encodes methionine (fMet in bacteria)
- **Stop codons**: UAA, UAG, UGA (no tRNA recognizes these — release factors bind instead)
- **Code properties**: Non-overlapping, read in fixed 5'→3' frame, nearly universal

### Wobble Hypothesis (Crick)
- The **3' base of the codon** pairs with the **5' base of the anticodon** (wobble position)
- Wobble base pairs: G:U, I:A, I:C, I:U (inosine = I, a modified adenine in tRNA)
- One tRNA can recognize multiple synonymous codons → fewer tRNAs than codons needed

---

## Ribosome Structure

| Feature | Prokaryotic | Eukaryotic |
|---------|-------------|------------|
| Total size | 70S | 80S |
| Small subunit | 30S (16S rRNA + ~21 proteins) | 40S (18S rRNA) |
| Large subunit | 50S (23S + 5S rRNA + ~31 proteins) | 60S (28S + 5.8S + 5S rRNA) |
| Decoding center | 30S | 40S |
| Peptidyl transferase center | 50S (catalytic RNA = ribozyme!) | 60S |

### tRNA Binding Sites (A, P, E)
- **A (Aminoacyl) site**: Accepts incoming aminoacyl-tRNA
- **P (Peptidyl) site**: Holds tRNA carrying the growing polypeptide
- **E (Exit) site**: Holds deacylated tRNA before release

---

## Mechanism: Three Stages

### 1. Initiation (Bacteria)
1. **30S subunit** binds mRNA at the **Shine-Dalgarno (SD) sequence** (~5–10 nt upstream of AUG; complementary to 3' end of 16S rRNA)
2. **fMet-tRNA^fMet** (charged with formyl-methionine) binds AUG in P site, assisted by **IF2** (GTP-dependent)
3. Initiation factors: IF1 (blocks A site), IF2 (fMet-tRNA delivery), IF3 (prevents premature 50S joining)
4. **50S subunit** joins → **70S initiation complex** formed; IFs released; GTP hydrolyzed

### 2. Elongation
**Cycle repeated for each amino acid:**
1. **Decoding (A site)**: EF-Tu·GTP·aminoacyl-tRNA delivers aa-tRNA to A site; codon-anticodon pairing checked; GTP hydrolyzed → EF-Tu·GDP released
2. **Peptide bond formation**: Peptidyl transferase (ribozyme activity of 23S rRNA) catalyzes transfer of peptide from P-site tRNA to A-site amino acid
3. **Translocation**: EF-G·GTP catalyzes movement of ribosome 3' by one codon; A-site tRNA moves to P site; P-site tRNA moves to E site; deacylated tRNA exits

### 3. Termination
- Stop codon (UAA, UAG, UGA) enters A site
- **Release factors**: RF1 (recognizes UAA, UAG), RF2 (recognizes UAA, UGA), RF3 (GTP-dependent)
- RF binds A site → peptidyl transferase hydrolyzes peptide-tRNA bond → polypeptide released
- **Ribosome recycling factor (RRF)** + EF-G disassemble 70S ribosome

---

## Polyribosomes (Polysomes)
- Multiple ribosomes translate same mRNA simultaneously
- In bacteria: **coupled to transcription** — ribosomes load onto mRNA as it is being synthesized
- Increases protein output per mRNA molecule

---

## Key Differences: Prokaryotes vs. Eukaryotes

| Feature | Prokaryotes | Eukaryotes |
|---------|-------------|------------|
| Ribosome | 70S | 80S |
| Start codon tRNA | fMet-tRNA^fMet | Met-tRNA^Met |
| mRNA recognition | Shine-Dalgarno sequence | 5' cap recognition (eIF4E) |
| Initiation factors | IF1, IF2, IF3 | eIF1–eIF6 (many more) |
| Coupled transcription | Yes | No |
| Antibiotic targets | 30S (streptomycin, tetracycline), 50S (chloramphenicol, erythromycin) | Different targets |

---

## Key Exam Points
- **SD sequence** in bacteria: pairs with 16S rRNA 3' end to position AUG in P site
- **fMet** is the initiator amino acid in bacteria (formylated methionine)
- Wobble: 5' anticodon base is wobble position; inosine (I) is most flexible
- Peptide bond formation = **ribozyme** (23S rRNA catalyzes, not protein)
- Stop codons have **no tRNA** — release factors (proteins) recognize them
- 70S = 30S + 50S (Svedberg units are NOT additive in the usual sense)
- EF-Tu delivers aa-tRNA; EF-G drives translocation — both require GTP

---

## Related Concepts
- [[Transcription]]
- [[Transcriptional Regulation]]
- [[Mutations]]
- [[Genetic Code]]

## Prerequisites
- DNA/RNA structure
- Central Dogma
- Protein structure basics

## Importance: HIGH YIELD
Start codon/SD sequence, ribosome subunit structure, A/P/E sites, and initiation steps are frequently tested.
