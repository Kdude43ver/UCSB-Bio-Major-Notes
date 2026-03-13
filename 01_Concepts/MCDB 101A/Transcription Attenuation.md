# Transcription Attenuation

**Topic Area:** Gene Regulation
**Lecture:** [[Transcriptional Regulation]]
**Exam:** Midterm 2
**Importance:** HIGH YIELD ⭐⭐

---

## One-Line Definition
Transcription attenuation is a mechanism of gene regulation in which the ribosome's progress along a leader peptide coding sequence controls whether RNAP terminates prematurely or reads through into structural genes — coupling translation to transcription as a biosensor for amino acid availability.

---

## The Trp Operon Attenuator

### Setup
- Leader region (*trpL*) encodes a 14 aa peptide with **two Trp residues** at positions 10–11
- The leader mRNA has 4 segments (1, 2, 3, 4) that can form alternative secondary structures:
  - **3:4 hairpin** = terminator (Rho-independent terminator, U-rich run)
  - **2:3 hairpin** = antiterminator (prevents 3:4 from forming)

### High [Trp] — Transcription OFF
1. Charged Trp-tRNA abundant → ribosome translates leader without stalling
2. Ribosome covers segment 1 (and part of 2)
3. Segment 2 unavailable → **3:4 terminator hairpin forms**
4. RNAP terminates in the attenuator → *trpEDCBA* not transcribed

### Low [Trp] — Transcription ON
1. Uncharged tRNA^Trp abundant → ribosome **stalls at Trp codons** in segment 1
2. Segment 2 is free → **2:3 antiterminator hairpin forms**
3. 3:4 cannot form → RNAP reads through → Trp biosynthesis genes expressed

---

## Key Requirements
- **Coupled transcription-translation** (prokaryotes only — ribosome must be on nascent mRNA while RNAP is transcribing downstream)
- Eukaryotes cannot use attenuation because mRNA must exit the nucleus before translation

---

## Comparison: Attenuation vs. Repressor-Based Regulation

| Feature | Attenuation (Trp operon) | Repressor control (also Trp operon) |
|---------|------------------------|-------------------------------------|
| Mechanism | Premature transcription termination | Blocks initiation |
| Sensor | Ribosome stalling at Trp codons | Trp-bound TrpR repressor binds operator |
| Speed | Rapid (cotranscriptional) | Moderate |
| Works in euk? | No | Yes |

The Trp operon uses **both** mechanisms — additive repression when Trp is abundant.

---

## Common Exam Traps
- Attenuation is **premature termination**, not repression of initiation
- The 2:3 antiterminator is what **prevents** the terminator from forming — it is not itself a terminator
- Attenuation requires prokaryotic coupled transcription-translation; eukaryotes cannot use this mechanism

---

## Connections
- [[Lac Operon]] — different mechanism (repressor-based), same operon logic
- [[Transcription]] — Rho-independent terminator is used here (hairpin + U-run)
- [[Translation]] — ribosome position is the regulatory input
- [[Transcriptional Regulation]]
