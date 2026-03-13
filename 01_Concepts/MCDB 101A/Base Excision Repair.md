# Base Excision Repair (BER)

## Definition
Base Excision Repair (BER) is a DNA repair pathway that corrects **small, non-helix-distorting base lesions** by removing and replacing individual damaged bases. It handles the most common types of spontaneous DNA damage — oxidation, deamination, and alkylation of bases — estimated at tens of thousands of lesions per cell per day.

---

## Damage Types Repaired by BER

| Lesion | Cause | Glycosylase |
|--------|-------|-------------|
| **Uracil** (from cytosine deamination) | Spontaneous hydrolysis; bisulfite | UNG (Uracil-DNA Glycosylase) |
| **8-oxoguanine** (8-oxoG) | Reactive oxygen species (ROS) | MutM/Fpg (bacteria); OGG1 (eukaryotes) |
| **3-methyladenine** | Alkylating agents | AlkA (bacteria); AAG (eukaryotes) |
| **Hypoxanthine** (from adenine deamination) | Spontaneous | Hypoxanthine-DNA glycosylase |
| **Thymine glycol** | UV/radiation | Endonuclease III / Nth |
| **AP (abasic) sites** | Spontaneous depurination/depyrimidination | AP endonuclease processes directly |

---

## Mechanism: Step-by-Step

### Step 1: Base Recognition and Removal (DNA Glycosylase)
- **DNA glycosylase** scans the minor groove, flips the damaged base out of the helix (**base flipping**)
- Cleaves the **N-glycosidic bond** between the damaged base and the deoxyribose sugar
- Leaves behind an **AP (apurinic/apyrimidinic) site** — a sugar-phosphate backbone with no base

### Step 2: AP Site Processing (AP Endonuclease)
- **AP endonuclease (APE1 in humans; Xth/Nfo in bacteria)** recognizes the AP site
- Cleaves the **phosphodiester backbone 5' of the AP site**
- Creates a **3'-OH** (for polymerase) and a **5'-deoxyribose phosphate (5'-dRP)** group

> ⚠️ Critical: AP site ≠ nick. The backbone is still intact at the AP site until AP endonuclease acts.

### Step 3: 5'-dRP Removal
- The **5'-dRP sugar remnant** must be removed before gap-filling
- In bacteria: **DNA Pol I** has an associated **dRP lyase** activity (β-elimination)
- In eukaryotes: **Pol β** has intrinsic dRP lyase activity

### Step 4: Gap Filling (DNA Polymerase)
- **DNA Pol I** (bacteria) or **Pol β** (eukaryotes) fills the 1-nucleotide gap using the intact complementary strand as template
- Inserts the correct base opposite the undamaged template

### Step 5: Ligation (DNA Ligase)
- **DNA ligase** seals the remaining nick
- Bacteria: requires NAD⁺; Eukaryotes: requires ATP

---

## Short-Patch vs. Long-Patch BER

| Feature | Short-Patch BER | Long-Patch BER |
|---------|----------------|----------------|
| Nucleotides replaced | 1 nt | 2–10 nt |
| Mechanism | Direct gap fill + ligate | Strand displacement synthesis; flap created |
| Flap removal | Not needed | FEN1 (flap endonuclease) removes displaced flap |
| Main polymerase (euk.) | Pol β | Pol δ/ε + PCNA |
| Frequency | More common | Less common |

---

## Key Glycosylases

### UNG (Uracil-DNA Glycosylase)
- Removes **uracil** from DNA — the most important BER glycosylase
- Uracil arises from **deamination of cytosine** (most common spontaneous mutation)
- If unrepaired: U pairs with A → C:G → T:A transition
- UNG is constitutively active and highly conserved

### MutM / Fpg (8-oxoguanine glycosylase, bacteria)
- Removes **8-oxoguanine** — caused by reactive oxygen species
- 8-oxoG normally pairs with C (correct), but can mispair with A → G:C → T:A transversion
- **MutY** (ADP-glycosylase) removes A from A:8-oxoG mispairs as a backup

### AlkA
- Removes **3-methyladenine** and other alkylated bases
- Induced as part of the adaptive response to alkylating agents

---

## BER vs. Other Repair Pathways

| Feature | BER | NER | MMR |
|---------|-----|-----|-----|
| Lesion type | Small base modifications, AP sites | Bulky helix-distorting adducts | Mismatches, insertion loops |
| Initiation | Glycosylase removes base | UvrABC dual incision | MutS recognizes mismatch |
| First step | Base removal → AP site | Backbone cuts flanking lesion | No base removal |
| Excision size | 1 base (AP site formed) | 12–13 nt (bacteria) | Hundreds–thousands nt |
| Gap polymerase | Pol I (bacteria) | Pol I | Pol III |
| Strand discrimination | N/A (damaged base removed) | N/A | Dam methylation (MutH) |

---

## Key Exam Points
- **BER removes one base at a time** via glycosylase; NER removes an oligonucleotide
- **AP site**: no base, but backbone intact — **AP endonuclease** must nick 5' of AP site
- **UNG** prevents C→U→T mutations; most important glycosylase to know
- **Pol I** handles gap filling in bacterial BER (and NER); **Pol III** is for MMR
- Short-patch = 1 nt replacement; long-patch = 2–10 nt
- 8-oxoG = oxidative damage; MutM removes it; if not repaired → G:C → T:A transversion
- BER is **constitutive** (not induced like SOS)
- Distinguish from **direct reversal**: photolyase (UV dimers) and AlkB (methylation) don't create an AP site

---

## Related Concepts
- [[DNA Repair Pathways]]
- [[Mutations]]
- [[Okazaki Fragments]]
- [[DNA Repair]]

## Prerequisites
- DNA structure and base pairing
- DNA polymerase mechanisms
- Types of DNA damage

## Importance: HIGH YIELD
AP site processing, glycosylase specificity, BER vs. NER distinction, and Pol I's role are all exam-tested concepts.
