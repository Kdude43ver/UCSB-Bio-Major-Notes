# Mismatch Repair (MMR)

**Topic Area:** DNA Repair
**Lecture:** [[DNA Repair]]
**Exam:** Final
**Importance:** HIGH YIELD ⭐⭐⭐

---

## One-Line Definition
Mismatch repair removes replication errors (base mismatches and small indel loops) from the **newly synthesized strand**, identified by its transient lack of Dam methylation at GATC sites.

---

## Key Players

| Protein | Function |
|---------|---------|
| **MutS** | Recognizes mismatch or small insertion/deletion loop; bends DNA |
| **MutL** | Molecular matchmaker; bridges MutS and MutH |
| **MutH** | Endonuclease; cuts the **unmethylated strand** at hemimethylated GATC |
| **UvrD** (helicase II) | Unwinds DNA from MutH nick toward the mismatch |
| Single-strand exonucleases | Degrade the new strand past the mismatch |
| **DNA Pol III + SSB** | Fills in the gap |
| **DNA Ligase** | Seals the nick |

---

## Strand Discrimination — The Dam Methylation System

- *E. coli* Dam methylase adds methyl groups to **adenine in GATC** sequences
- Immediately after replication: parental strand = **methylated**; new strand = **unmethylated** (transiently)
- MutH cuts the **unmethylated strand** at the nearest GATC → only the new (potentially erroneous) strand is degraded
- The GATC site can be **>1 kb** from the mismatch — MutL mediates the long-range communication

---

## Mechanism Steps
1. MutS binds mismatch → bends DNA
2. MutL recruited
3. MutH finds nearest hemimethylated GATC → nicks unmethylated strand
4. UvrD unwinds from nick toward mismatch
5. Exonucleases degrade new strand beyond mismatch
6. Pol III + SSB fills gap; Ligase seals

---

## Error Rate Impact
- Without MMR (proofreading only): ~10⁻⁷ errors/bp
- With MMR: ~10⁻⁹–10⁻¹⁰ errors/bp

---

## Human Homologs and Disease
| E. coli | Human | Disease if defective |
|---------|-------|---------------------|
| MutS | MSH2-MSH6 (base-base), MSH2-MSH3 (small loops) | Lynch syndrome (HNPCC) |
| MutL | MLH1-PMS2 | Lynch syndrome |
| MutH | No direct homolog | (strand discrimination via PCNA/nick) |

**Microsatellite instability (MSI)** is a hallmark of MMR-deficient tumors.

---

## Common Exam Traps (from NLM)
- MMR removes the **new strand**, not the parental strand
- MutH is unique to bacteria — eukaryotes use PCNA and strand discontinuities for strand discrimination
- The GATC site can be far from the mismatch; MutL enables this long-range interaction

---

## Connections
- [[DNA Replication]] — MMR corrects errors that escape Pol III proofreading
- [[Nucleotide Excision Repair]] — different substrate; NER handles bulky lesions
- [[Luria-Delbrück Fluctuation Test]] — MMR defects increase overall mutation rate
- [[DNA Repair]]
