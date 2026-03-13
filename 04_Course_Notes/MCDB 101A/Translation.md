# Translation

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## 🎯 Learning Objectives

1. Interpret the genetic code and identify synonymous codons
2. Explain the wobble hypothesis and its consequences for codon-anticodon pairing
3. Describe the structure and function of the ribosome, including A, P, and E sites
4. Explain the mechanism of translation initiation, elongation, and termination in prokaryotes
5. Describe how aminoacyl-tRNA synthetases ensure accuracy of translation

---

## 🧠 Core Concepts

### The Genetic Code

**Properties**

- **Triplet code:** 3 nucleotides = 1 codon → 4³ = 64 possible codons for 20 amino acids
- **Degenerate (redundant):** Multiple codons can encode the same amino acid (synonymous codons)
- **Non-overlapping:** Each nucleotide belongs to only one codon
- **Comma-free:** Continuously read without punctuation (reading frame set by start codon)
- **Nearly universal:** Essentially the same in all organisms (minor exceptions in mitochondria)

**Special Codons**

| Codon | Amino Acid / Function |
|-------|----------------------|
| AUG | Methionine / START codon |
| UAA | Stop (Ochre) |
| UAG | Stop (Amber) |
| UGA | Stop (Opal/Umber) |

**Degeneracy Pattern**
- Most degeneracy is at the **3rd (wobble) position**
- Met (M) and Trp (W) are encoded by only one codon each

### The Wobble Hypothesis (Crick, 1966)

**Concept**

The first two positions of the codon pair strictly with the anticodon (standard Watson-Crick pairing). The **third position** of the codon can pair non-standard ("wobble") with the first position of the anticodon.

**Wobble Pairing Rules**

| Anticodon position 1 (5' end of anticodon) | Can pair with codon position 3 |
|---------------------------------------------|-------------------------------|
| G | C or U |
| C | G only |
| A | U only |
| U | A or G |
| **Inosine (I)** | C, U, or A (most flexible) |

**Consequence**
- Fewer tRNAs than codons are needed (~45 tRNAs decode 61 sense codons)
- tRNAs with inosine at the wobble position are especially flexible

### Aminoacyl-tRNA Synthetases

**"Second Genetic Code"**

- 20 aaRS enzymes (one per amino acid); highly specific
- Each charges the correct tRNA with the correct amino acid

**Mechanism (2-step)**

1. Amino acid + ATP → aminoacyl-adenylate + PPi (activation)
2. Aminoacyl-adenylate + tRNA → aminoacyl-tRNA + AMP

**Proofreading (Editing Activity)**

- Some aaRS have an **editing active site** separate from the synthetic site
- If a wrong amino acid is attached, it's hydrolyzed before it reaches the ribosome
- Example: IleRS occasionally charges Ile-tRNA^Ile with valine → editing site removes Val
- "Double sieve" mechanism: synthetic site excludes amino acids larger than the cognate; editing site excludes the cognate and amino acids smaller

### Ribosome Structure

**Prokaryotic Ribosome (70S)**

| Subunit | Components | Sedimentation |
|---------|-----------|---------------|
| Small (30S) | 16S rRNA + ~21 proteins | Decoding center |
| Large (50S) | 23S + 5S rRNA + ~31 proteins | Peptidyl transferase center (PTC) |

**Ribosomal RNA is catalytic:** PTC is composed of 23S rRNA, not protein (ribozyme).

**A, P, E Sites**

| Site | Full Name | Function |
|------|-----------|---------|
| A site | Aminoacyl site | Incoming aminoacyl-tRNA binds |
| P site | Peptidyl site | tRNA carrying growing peptide chain |
| E site | Exit site | Discharged tRNA exits the ribosome |

### Prokaryotic Translation Initiation

**Shine-Dalgarno Sequence**

- Purine-rich sequence on mRNA (~6–10 nt upstream of AUG): consensus **AGGAGG**
- Complementary to 3' end of 16S rRNA (**anti-SD sequence**: CCUCC)
- Base pairing positions the AUG start codon in the P site

**Initiation Steps**

1. **30S + mRNA + fMet-tRNA^fMet + IF1 + IF2 + IF3 → 30S initiation complex (30S IC)**
   - IF3: prevents premature 50S joining
   - IF2 (GTPase): brings fMet-tRNA^fMet to P site
   - IF1: blocks A site
2. IF3 released; 50S joins → **70S initiation complex**
3. IF1 and IF2 released (GTP hydrolysis); elongation begins

### Elongation Cycle

1. **Decoding (A site):** EF-Tu·GTP delivers aminoacyl-tRNA to A site; GTP hydrolysis after correct codon:anticodon match; EF-Tu·GDP released
2. **Peptide bond formation:** PTC catalyzes transfer of peptide from P-site tRNA to α-amino group of A-site amino acid; A site now has peptidyl-tRNA (one aa longer); P site has uncharged tRNA
3. **Translocation:** EF-G·GTP catalyzes movement of ribosome 3 nt in 3' direction; A-site peptidyl-tRNA → P site; P-site tRNA → E site; new A site exposed; EF-G·GDP released

### Termination

1. Stop codon in A site recognized by **Release Factor (RF1 or RF2)**
   - RF1: reads UAA, UAG
   - RF2: reads UAA, UGA
2. RF + GTP hydrolyzes ester bond linking peptide to tRNA → peptide released
3. **RF3** (GTPase) promotes RF1/RF2 dissociation
4. **RRF (ribosome recycling factor) + EF-G:** disassembles 70S → free subunits for next round

---

## ⚠️ Exam Traps

- ❌ **"The A site is where the growing chain is"** — The **P site** holds the peptidyl-tRNA with the growing chain; A site receives the **incoming** aminoacyl-tRNA.
- ❌ **"Ribozymes are only found in eukaryotes"** — The PTC in the 50S ribosomal subunit is a ribozyme in both prokaryotes and eukaryotes.
- ❌ **"Wobble applies to all three codon positions"** — Wobble is specifically at the **third position** of the codon / **first position** of the anticodon.

---

## Practice Questions

1. A tRNA has the anticodon 3'-IAG-5'. What codons can this tRNA recognize? (Remember: anticodon is read 3'→5', codon 5'→3')

2. A mutation changes the AUG start codon of an mRNA to AUA. What happens to protein synthesis from this transcript in prokaryotes?

3. If the wobble position of the anticodon has guanosine, which codons can be decoded?

4. Why is fMet-tRNA^fMet used only for initiation and not elongation in bacteria?

5. What would be the consequence of a mutation that prevents SD:anti-SD pairing on translation efficiency?

---

## Related Concepts

- [[Genetic Code]]
- [[Translation]]
- [[Translation]]
- [[Translation]]
- [[Transcription]] — mRNA template for translation
- [[Lac Operon]] — translational coupling in operons
