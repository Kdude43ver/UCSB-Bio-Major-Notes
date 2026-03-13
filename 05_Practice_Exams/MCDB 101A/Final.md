# Practice Exam — Final

**Course:** MCDB 101A — Molecular Genetics I
**Coverage:** Lectures 11–17 (Mutations, DNA Repair, Recombination, Gene Transfer, Techniques)
**Format:** 10 Multiple Choice Questions
**Source:** Generated from course materials via NotebookLM

---

## Instructions

Select the single best answer for each question. After completing all questions, check your answers in the [[#Answer Key]] section below. Review explanations for any question you miss.

---

## Questions

**1.** Which of the following best describes the primary conclusion of the **Luria-Delbrück fluctuation test**?

A. Mutations in bacteria occur as a direct adaptive response to environmental stress, such as phage infection.
B. Mutations arise spontaneously and randomly before selection is applied.
C. The rate of mutation is constant across all individual bacterial cultures.
D. Bacterial resistance is inherited through the acquisition of protein fragments from the environment.

---

**2.** In a bacterial infection experiment where the multiplicity of infection (m) is exactly 1 (1×10⁶ bacteria infected with 1×10⁶ phage), approximately what percentage of the bacteria will remain **uninfected** based on the Poisson distribution?

A. 0%
B. 13%
C. 37%
D. 63%

---

**3.** In *E. coli* **Mismatch Repair (MMR)**, how does the **MutH** protein distinguish the newly synthesized daughter strand from the parental template strand?

A. It recognizes acetyl groups on the newly formed histones.
B. It identifies the daughter strand by the presence of a 3' overhang.
C. It binds to hemimethylated GATC sequences and nicks the unmethylated strand.
D. It only recognizes the strand that contains uracil instead of thymine.

---

**4.** During **Nucleotide Excision Repair (NER)** in *E. coli*, which protein is responsible for **displacing** the damaged DNA segment after nicks have been made by the UvrBC complex?

A. UvrA
B. UvrD
C. DNA Polymerase I
D. DNA Ligase

---

**5.** Which bacterial protein is responsible for **cleaving** the Holliday junction structure to finish recombination?

A. RecA
B. RuvAB
C. RuvC
D. RecBCD

---

**6.** In the **Double-Strand Break (DSB) Repair** model, what is the first step performed by the **RecBCD** complex after binding to a broken DNA end?

A. Synthesis of a new DNA strand to bridge the break.
B. Degradation of the DNA until it reaches a Chi site.
C. Immediate loading of RuvC to resolve the break.
D. Direct ligation of the broken ends.

---

**7.** During bacterial **conjugation** involving an **Hfr strain**, what is the primary factor used to determine the **relative order and distance** of genes on the chromosome?

A. The number of plaques formed on a restrictive host.
B. The density of the DNA in a cesium chloride gradient.
C. The time of entry of specific markers into the recipient cell.
D. The frequency of spontaneous reversion of auxotrophic mutations.

---

**8.** Restriction endonucleases like **EcoRI** typically recognize and cut DNA at sequences that are:

A. Long stretches of repetitive A-T base pairs.
B. Randomly distributed throughout the genome every 100 bp.
C. Palindromic, reading the same 5'→3' on both strands.
D. Only found at the ends of linear chromosomes (telomeres).

---

**9.** In **Sanger sequencing**, why does the addition of a **dideoxynucleoside triphosphate (ddNTP)** stop DNA synthesis?

A. It lacks a 5' phosphate group necessary for energy.
B. It inhibits the helicase from unwinding the DNA template.
C. It lacks a 3'-OH group, preventing the addition of the next nucleotide.
D. It causes the DNA polymerase to fall off the sliding clamp.

---

**10.** What molecular signal directly activates **RecA** to initiate the **SOS response** in bacteria?

A. The presence of double-stranded DNA breaks.
B. Binding to single-stranded DNA (ssDNA) resulting from DNA damage.
C. High levels of ATP in the cytoplasm.
D. Direct contact with ionizing radiation.

---

## Answer Key

| Q | Answer | Explanation |
|---|--------|-------------|
| 1 | **B** | Luria and Delbrück showed that phage-resistant mutations arose spontaneously before phage exposure, as evidenced by the high variance (jackpot cultures) across replicate experiments. |
| 2 | **C** | Poisson formula: P(0) = e^(−m) = e^(−1) ≈ 0.368, or **~37%** of bacteria remain uninfected. |
| 3 | **C** | *E. coli* Dam methylase methylates A in GATC sequences. Right after replication, only the parental strand is methylated (hemimethylated). MutH nicks the unmethylated (new) strand. |
| 4 | **B** | **UvrD** (helicase II) unwinds and displaces the 12–13 nt damaged fragment after UvrBC makes the dual incisions. DNA Pol I then fills the gap. |
| 5 | **C** | **RuvC** is a resolvase/endonuclease that nicks two homologous strands of the Holliday junction to produce either splice (crossover) or patch (non-crossover) products. |
| 6 | **B** | RecBCD binds at the DSB end and degrades DNA (helicase + nuclease) until it encounters a **Chi site** (5'-GCTGGTGG-3'), where nuclease activity switches to generate a 3' ssDNA tail for RecA loading. |
| 7 | **C** | In Hfr mapping, genes are transferred linearly from oriT. The **time at which each marker first appears** in the recipient determines gene order and relative distance (interrupted mating). |
| 8 | **C** | Restriction enzymes typically recognize short (4–8 bp) **palindromic sequences** and cut within or near those sequences, producing sticky or blunt ends. |
| 9 | **C** | ddNTPs lack the **3'-OH group**. Without a free 3'-OH, the next phosphodiester bond cannot form, causing chain termination at every position where a ddNTP is incorporated. |
| 10 | **B** | **Single-stranded DNA** (from stalled replication forks or unrepaired damage) recruits RecA to form a nucleoprotein filament. Activated RecA then stimulates autoproteolysis of LexA, derepressing SOS genes. |

---

## Related Notes

- [[Mutations]]
- [[DNA Repair]]
- [[Recombination]]
- [[Gene Transfer]]
- [[Molecular Techniques]]
- [[Luria-Delbrück Fluctuation Test]]
- [[Mismatch Repair]]
- [[Nucleotide Excision Repair]]
- [[Holliday Junction]]
- [[Hfr Conjugation Mapping]]
- [[PCR]]
