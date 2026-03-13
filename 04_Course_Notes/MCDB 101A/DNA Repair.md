# DNA Repair

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## 🎯 Learning Objectives

1. Compare the three major repair pathways: NER, MMR, and BER in terms of damage recognized, enzymes, and mechanism
2. Describe the prokaryotic NER mechanism (UvrABC system) step by step
3. Explain how MutSHL achieves strand discrimination in MMR
4. Describe base excision repair: glycosylase, AP endonuclease, gap-filling, and ligation
5. Explain the SOS response and its role in repair vs. mutagenesis

---

## 🧠 Core Concepts

### Overview of DNA Repair Pathways

| Pathway | Damage Repaired | Strand Specificity | Key Enzymes (E. coli) |
|---------|---------------|-------------------|-----------------------|
| **Nucleotide Excision Repair (NER)** | Bulky adducts, pyrimidine dimers, helix-distorting lesions | Both strands recognized; damaged strand excised | UvrA, UvrB, UvrC, UvrD, Pol I, Ligase |
| **Mismatch Repair (MMR)** | Replication mismatches, small loops | Newly synthesized strand excised | MutS, MutL, MutH, UvrD, exonucleases, Pol III, Ligase |
| **Base Excision Repair (BER)** | Small base modifications (oxidation, deamination, alkylation) | Damaged strand excised | DNA glycosylase, AP endonuclease, Pol I (or Pol β), Ligase |

### Nucleotide Excision Repair (NER) — UvrABC System

**Substrates**

- UV-induced pyrimidine dimers (CPD: cyclobutane pyrimidine dimers; 6-4 PP: pyrimidine-pyrimidone photoproducts)
- Bulky chemical adducts (benzo[a]pyrene-dG, cisplatin crosslinks)
- Any lesion that significantly distorts the double helix

**Mechanism**

1. **UvrA₂B complex** forms in solution; UvrA recognizes helix distortion via DNA bending
2. **UvrB** (helicase-like) is loaded at the damage site; UvrA₂ dissociates
3. **UvrC** binds UvrB-DNA complex; UvrC makes two incisions:
   - 8th phosphodiester bond 3' to the lesion (UvrC 3' endonuclease)
   - 4th–5th phosphodiester bond 5' to the lesion (UvrC 5' endonuclease)
   - Excises a **12–13 nt oligonucleotide** containing the lesion
4. **UvrD (helicase II)** displaces the 12–13 nt fragment along with UvrC
5. **DNA Pol I** fills the gap (5'→3'); **DNA Ligase** seals the nick

**Eukaryotic NER**

- **Global genome NER (GG-NER):** XPC-RAD23B recognizes helix distortion genome-wide
- **Transcription-coupled NER (TC-NER):** Stalled RNAP triggers repair of transcribed strand preferentially
- Human syndrome: **Xeroderma pigmentosum (XP)** — defective NER; UV sensitivity; skin cancer

### Mismatch Repair (MMR) — MutSHL System

**Substrates**

- Replication errors: base-base mismatches, small insertion/deletion loops (from slippage)
- Must remove **new strand** (the one with the error), not the parental strand

**Strand Discrimination — GATC Methylation**

- *E. coli* methylates adenine in **GATC** sequences (by Dam methyltransferase)
- Immediately after replication, **parental strand is methylated; new strand is transiently unmethylated**
- MutH uses this to distinguish strands: cuts the **unmethylated strand** at the nearest GATC site

**Mechanism**

1. **MutS** recognizes the mismatch → binds and bends DNA
2. **MutL** is recruited; acts as a molecular matchmaker
3. **MutH** binds hemimethylated GATC site (can be >1 kb from mismatch); cuts the unmethylated (new) strand
4. **UvrD** (helicase) unwinds DNA from the nick toward the mismatch
5. **Single-strand exonucleases** degrade the new strand beyond the mismatch
6. **Pol III + SSB** fills the gap; **Ligase** seals

**Human MMR**

- MutS homologs: **MSH2-MSH6** (base mismatches), **MSH2-MSH3** (small loops)
- MutL homologs: **MLH1-PMS2**
- No MutH equivalent; strand discrimination by PCNA/strand discontinuities
- Defects: **Hereditary Nonpolyposis Colorectal Cancer (HNPCC/Lynch Syndrome)**; microsatellite instability (MSI)

### Base Excision Repair (BER)

**Substrates**

- Small, non-helix-distorting base modifications:
  - 8-oxoguanine (oxidation; pairs with A → G:C→T:A transversions if unrepaired)
  - Uracil in DNA (deamination of cytosine; → C:G→T:A if unrepaired)
  - Alkylated bases (3-methyladenine, 7-methylguanine)
  - Abasic (AP) sites

**Mechanism**

1. **DNA glycosylase** recognizes and cleaves the N-glycosidic bond → releases the damaged base → leaves an **abasic (AP) site**
   - Monofunctional: cuts only N-glycosidic bond
   - Bifunctional: cuts N-glycosidic bond AND 3' phosphodiester bond (β-lyase activity)
2. **AP endonuclease (APE1)** cuts 5' to the AP site → 5' deoxyribose phosphate (dRP) residue
3. **Pol I (short patch) or Pol β (eukaryotes)** incorporates 1 nt; removes dRP flap (dRPase activity)
4. **DNA Ligase** seals nick

**Key Glycosylases**

| Glycosylase | Substrate |
|-------------|---------|
| UNG (Uracil DNA Glycosylase) | Uracil (from C deamination) |
| MutM (Fpg) | 8-oxoguanine, ring-opened purines |
| MutY | Adenine mispaired with 8-oxoG |
| AlkA | Alkylated bases (3-mA, 7-mG) |
| Nth (Endonuclease III) | Thymine glycol, other oxidized pyrimidines |

### SOS Response — Damage-Induced Mutagenesis

**Trigger**

Extensive single-stranded DNA (from stalled replication forks or UV damage) → **RecA** polymerizes on ssDNA → activated RecA co-protease stimulates autocleavage of **LexA** repressor → SOS genes induced.

**SOS Genes and Products**

| Gene | Product | Function |
|------|---------|---------|
| *recA* | RecA | ssDNA binding, recombination |
| *lexA* | LexA | SOS repressor (auto-regulated) |
| *uvrA, uvrB* | NER components | Repair of UV damage |
| *sulA* | SulA | Cell division inhibitor (buys time for repair) |
| *umuC, umuD* | UmuC, UmuD | Components of **DNA Pol V (translesion synthesis)** |
| *dinB* | UmuC homolog | **DNA Pol IV** — translesion synthesis |

**Translesion Synthesis (TLS)**

- Pol V (UmuC₂D'): bypass synthesis past unrepaired lesions
- **Error-prone** — inserts incorrect nucleotides (5'-A across from CPD dimers)
- This is the basis of **SOS mutagenesis** — survival at the cost of increased mutation rate

---

## ⚠️ Exam Traps

- ❌ **"NER only repairs UV damage"** — NER repairs any bulky, helix-distorting lesion (crosslinks, adducts, not just pyrimidine dimers).
- ❌ **"MMR removes the parental strand"** — MMR specifically removes the **new** strand (identified by absence of methylation).
- ❌ **"BER and NER both excise oligonucleotides"** — BER removes just the **base** (and 1–2 nucleotides); NER removes a **12–13 nt oligonucleotide**.
- ❌ **"Translesion synthesis is error-free"** — TLS is inherently error-prone; it sacrifices accuracy for survival.

---

## Practice Questions

1. A mutation eliminates the N-glycosidic bond cleavage activity of UNG. What specific mutations would accumulate at elevated rates? At what positions (CpG?)?

2. Explain how MutH determines which strand to degrade in MMR. What would happen in a *dam*⁻ mutant where neither strand is methylated?

3. Compare the size of the repair patch in NER vs. BER. What determines the size difference?

4. A bacterium is exposed to a high dose of UV light. Describe the sequence of events from lesion formation to resumption of replication, including the roles of UvrABC, SOS, and Pol V.

5. Patients with mutations in *MSH2* frequently develop colorectal cancer. Why does a single inactivating mutation in *MSH2* (heterozygous) not immediately cause cancer, but inheriting two inactivated alleles (or losing heterozygosity) does?

---

## Related Concepts

- [[Nucleotide Excision Repair]]
- [[Mismatch Repair]]
- [[Base Excision Repair]]
- [[Mutations]] — the lesions these pathways repair
- [[DNA Replication]] — MMR requires access to replication fork
- [[Bacteriophage Lambda]] — SOS induction activates λ lytic cycle
