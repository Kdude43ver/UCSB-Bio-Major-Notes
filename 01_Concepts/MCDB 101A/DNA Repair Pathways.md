# DNA Repair Pathways

## Overview
Cells employ multiple repair systems to correct DNA damage. Each pathway targets specific lesion types and uses distinct mechanisms. The four major pathways in bacteria are: **Mismatch Repair (MMR)**, **Nucleotide Excision Repair (NER)**, **Base Excision Repair (BER)**, and **SOS/Translesion Synthesis (TLS)**.

---

## 1. Mismatch Repair (MMR)

### Function
Corrects **replication errors**: mismatched base pairs and small insertion/deletion loops that escape DNA Pol III proofreading.

### The Key Problem: Which Strand is the Error?
After replication, both strands have the same sequence but **only the parental strand** is correctly methylated. MMR uses methylation to identify the template.

### Dam Methylation System
- **Dam methylase** methylates adenine in **GATC sequences** (N⁶-methyladenine)
- Newly synthesized daughter strand is **transiently unmethylated** → **hemimethylated** DNA
- MMR uses hemimethylation to identify the **new (error-containing) strand**

### Mechanism (E. coli)
1. **MutS** recognizes and binds the mismatch
2. **MutL** (ATPase) acts as a mediator; recruits MutH
3. **MutH** binds nearby **hemimethylated GATC** site; cleaves the **unmethylated (new) strand**
4. **UvrD helicase** unwinds from nick to mismatch
5. **Exonucleases** degrade the unmethylated strand up to and past the mismatch
6. **DNA Pol III** fills the gap
7. **DNA Ligase** seals the nick

### Key Points
- MutH is the strand discrimination factor — only cuts unmethylated strand
- Gap can be 100s to 1000s of bp long
- Pol III (not Pol I) fills the MMR gap

---

## 2. Nucleotide Excision Repair (NER)

### Function
Repairs **bulky helix-distorting lesions**: pyrimidine dimers (UV damage), large chemical adducts, intrastrand crosslinks.

### Mechanism (E. coli — UvrABC System)
1. **UvrA₂B** complex scans DNA; **UvrA** recognizes distortion
2. **UvrA** dissociates; **UvrB** remains bound at lesion; **UvrC** is recruited
3. **UvrB cuts 3'** side of lesion (4–5 nt from damage)
4. **UvrC cuts 5'** side of lesion (~8 nt from damage)
5. **~12–13 nt oligonucleotide** containing the lesion is excised
6. **UvrD helicase** removes the fragment
7. **DNA Pol I** fills the gap
8. **DNA Ligase** seals

### Key Points
- Cuts BOTH sides of the lesion (dual incision) → removes oligonucleotide
- Excision fragment: ~12–13 nt (bacteria) / ~25–30 nt (eukaryotes)
- UvrA = damage recognition; UvrB = verification + marks site; UvrC = dual incision
- **Pol I** (not Pol III) fills the NER gap

---

## 3. Base Excision Repair (BER)

### Function
Repairs **small, non-helix-distorting base modifications**: oxidized bases (8-oxoguanine), deaminated bases (uracil from C deamination), alkylated bases (3-methyladenine), abasic (AP) sites.

### Mechanism
1. **DNA Glycosylase** recognizes and cleaves the **N-glycosidic bond** → removes damaged base → creates **AP (abasic) site**
   - UNG (uracil-DNA glycosylase): removes uracil (from C deamination)
   - OGG1 / MutM (Fpg): removes 8-oxoguanine
   - AlkA / Tag: removes 3-methyladenine
2. **AP Endonuclease** cleaves the phosphodiester backbone **5' of the AP site** → nick with 3'-OH and 5'-dRP (deoxyribose phosphate)
3. **dRP Lyase** (activity of Pol I or Pol β) removes the 5'-dRP group
4. **DNA Pol I** fills the 1-nt gap
5. **DNA Ligase** seals the nick

### Key Points
- BER starts with base removal (glycosylase); NER starts with backbone incision on BOTH sides
- AP site ≠ a nick — AP site must be processed by AP endonuclease before gap can be filled
- Short-patch BER: 1 nt replaced (most common)
- Long-patch BER: 2–10 nt replaced via strand displacement + flap cleavage

---

## 4. SOS Response / Translesion Synthesis (TLS)

### Function
**Not true repair** — SOS is a **damage tolerance** pathway. It allows replication to continue past unrepaired lesions that block DNA Pol III, at the cost of introducing mutations.

### Induction Mechanism
1. **DNA damage** (or replication blocks) → accumulation of **ssDNA**
2. **RecA** binds ssDNA → forms **RecA filament** → acts as **co-protease**
3. RecA filament stimulates **LexA autoproteolysis** (self-cleavage)
4. LexA normally represses >40 SOS genes → its destruction **induces** the SOS regulon
5. SOS genes expressed include: **UmuC, UmuD** (components of Pol V), **sulA** (cell division inhibitor), **recA**, **uvrA**, **uvrB**

### Translesion Synthesis
- **UmuD** undergoes RecA-mediated autoproteolysis → **UmuD'**
- **UmuD'₂C = DNA Pol V** — error-prone polymerase
- Pol V inserts nucleotides across from damaged bases that block Pol III (e.g., abasic sites, pyrimidine dimers)
- **Highly error-prone** → introduces mutations (hence: mutagenic repair)
- **SOS mutagenesis** = mutation frequency increases after DNA damage

### Key Points
- SOS is **induced** (not constitutive) — requires damage signal
- RecA co-protease activity is DISTINCT from its recombination activity
- LexA is the **repressor** of SOS genes; its destruction = SOS induction
- **Pol V is mutagenic** — inserts wrong bases across lesions
- SOS allows survival but at cost of increased mutation rate

---

## Comparison Table

| Feature | MMR | NER | BER | SOS/TLS |
|---------|-----|-----|-----|---------|
| **Damage recognized** | Mismatches, small indels | Bulky adducts, pyrimidine dimers | Oxidized/deaminated/alkylated bases, AP sites | Any lesion blocking Pol III |
| **Recognition proteins** | MutS | UvrA₂B | DNA Glycosylase | RecA (ssDNA) |
| **Strand discrimination** | Dam methylation (MutH) | N/A (excises both strands flanking lesion) | N/A (removes damaged base only) | N/A |
| **Excision size** | 100s–1000s nt | 12–13 nt | 1 base (AP site) | None (polymerase bypass) |
| **Gap-filling polymerase** | DNA Pol III | DNA Pol I | DNA Pol I | DNA Pol V (UmuD'₂C) |
| **Error-prone?** | No (high fidelity) | No | No | **Yes** (mutagenic) |
| **Constitutive/Inducible** | Constitutive | Constitutive | Constitutive | **Inducible** (SOS) |

---

## Key Exam Traps
1. **Pol I vs. Pol III**: MMR uses Pol III; NER and BER use Pol I
2. **AP site ≠ nick**: AP endonuclease must cut the backbone before a gap forms
3. **SOS is NOT repair** — it is damage tolerance; mistakes are made
4. **Direct reversal** (e.g., photolyase, AlkB) ≠ excision repair — no strand incision needed
5. **MutH** cuts the **unmethylated** strand — the NEW strand
6. **UvrABC** makes dual incision flanking the lesion; UvrD removes the fragment
7. RecA's role in SOS (co-protease) is **different** from its role in recombination (strand exchange)
8. **UmuD must be cleaved** to UmuD' before Pol V (UmuD'₂C) is active

---

## Related Concepts
- [[Base Excision Repair]]
- [[Mutations]]
- [[Okazaki Fragments]]
- [[Recombination]]
- [[Transduction]]

## Prerequisites
- DNA structure and replication
- DNA polymerase properties
- Bacterial gene regulation

## Importance: HIGH YIELD
All four pathways, their protein components, damage types, and key distinctions are extremely high-yield for exams. The comparison table is essential to memorize.
