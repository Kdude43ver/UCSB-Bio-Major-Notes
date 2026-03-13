# Transcription

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## 🎯 Learning Objectives

1. Describe the structure and function of prokaryotic RNA polymerase holoenzyme
2. Explain the roles of σ factor in promoter recognition and open complex formation
3. Compare prokaryotic and eukaryotic promoter elements
4. Describe the three stages of prokaryotic transcription: initiation, elongation, termination
5. Explain eukaryotic mRNA processing: 5' cap, 3' poly-A tail, and splicing

---

## 🧠 Core Concepts

### Prokaryotic RNA Polymerase

**Holoenzyme Composition**

| Subunit | Gene | Function |
|---------|------|---------|
| α (x2) | rpoA | Assembly platform; interacts with regulatory factors (UP elements) |
| β | rpoB | Catalytic subunit; contains active site; binds NTPs |
| β' | rpoC | Clamps onto DNA template; binds DNA non-specifically |
| ω | rpoZ | Assembly/stability |
| **σ (sigma)** | rpoD (σ⁷⁰ in E. coli) | Promoter recognition; dissociates after initiation |

- **Core enzyme:** αα ββ' ω (catalytically active but cannot find promoters)
- **Holoenzyme:** Core + σ (can recognize and bind promoters)

### Prokaryotic Promoter Elements

**σ⁷⁰ (Housekeeping) Promoter**

| Element | Position | Consensus | Function |
|---------|---------|-----------|---------|
| –10 box | –10 from TSS | TATAAT (Pribnow box) | Strand separation for open complex |
| –35 box | –35 from TSS | TTGACA | Initial holoenzyme recognition |
| UP element | –40 to –60 | AT-rich | Enhances transcription; binds α CTD |
| Spacer | Between –10 and –35 | 17 ± 1 bp optimal | Correct spacing required for dual recognition |

**Promoter Strength**

Determined by:
1. Similarity to consensus at –10 and –35
2. Correct spacer length (17 bp optimal)
3. Presence of UP element
4. Base stacking/stability at –10 (easier melting if AT-rich)

### Stages of Prokaryotic Transcription

**Initiation**

1. **Closed complex (RPc):** Holoenzyme binds promoter dsDNA; no melting
2. **Open complex (RPo):** ~14 bp around –10 melted; transcription bubble formed
3. **Abortive initiation:** RNAP makes short (<10 nt) transcripts and releases them; multiple cycles
4. **Promoter clearance:** After ~10 nt, σ released; elongation complex (TEC) moves processively

**Elongation**

- RNAP moves 5'→3', reads template 3'→5'
- Nascent RNA grows 5'→3'; complementary and antiparallel to template
- ~40–80 nt/second in bacteria
- Elongation complex is highly stable and processive

**Termination**

**Intrinsic (Rho-independent) Termination:**
1. G-C rich inverted repeat in RNA → hairpin forms in nascent RNA just outside exit channel
2. Followed by U-rich sequence (run of ~6–8 Us)
3. Hairpin stalls RNAP; weak rU–dA base pairs at 3' end dissociate
4. Transcript is released

**Rho-dependent Termination:**
1. Rho factor (hexameric helicase-like ATPase) binds rut site (Rho utilization site) on nascent RNA
2. Rho translocates 5'→3' on RNA behind the RNAP
3. Rho catches stalled RNAP (at pause sites); uses helicase activity to displace transcript from template
4. Requires ATP

### Sigma Factors and Alternative Promoters

| Sigma Factor | MW | Recognizes | Condition |
|-------------|-----|-----------|---------|
| σ⁷⁰ | 70 kDa | –35/–10 housekeeping promoters | Log phase growth |
| σ³² | 32 kDa | Heat shock gene promoters | Heat stress |
| σ⁵⁴ | 54 kDa | –24/–12 motifs | Nitrogen limitation |
| σ²⁸ | 28 kDa | Flagellar gene promoters | Motility |

Multiple σ factors allow a single RNAP to regulate different gene sets by swapping σ.

### Eukaryotic Transcription (Overview)

**RNA Polymerases**

| RNAP | Products |
|------|---------|
| RNAP I | 28S, 18S, 5.8S rRNA |
| RNAP II | mRNA, snRNA, miRNA |
| RNAP III | tRNA, 5S rRNA, snRNA |

### mRNA Processing (RNAP II products)

**5' Capping**
- Added to the 5' end of the pre-mRNA co-transcriptionally
- Structure: 7-methylguanosine connected via 5'–5' triphosphate linkage
- Functions: protects from 5' exonucleases; enhances translation initiation; aids nuclear export

**3' Polyadenylation**
- AAUAAA signal in pre-mRNA recognized by CPSF
- Endonuclease cleaves ~10–30 nt downstream
- Poly-A polymerase adds ~200 A residues
- Functions: protects from 3' degradation; aids translation; enables nuclear export

**Splicing**
- Introns removed by the **spliceosome** (snRNPs: U1, U2, U4/U6, U5)
- Splice sites: 5' GU (donor) and AG 3' (acceptor); branch point A (YNYURAY)
- Two-step transesterification:
  1. 2'-OH of branch point A attacks 5' splice site → lariat intermediate
  2. 3'-OH of exon 1 attacks 3' splice site → exons joined, lariat released
- Alternative splicing: one pre-mRNA → multiple proteins (e.g., Drosophila *dsx*, *tra*)

---

## ⚠️ Exam Traps

- ❌ **"σ factor is part of the elongation complex"** — σ dissociates after promoter clearance (~10 nt).
- ❌ **"Rho termination requires a hairpin"** — Hairpin is intrinsic termination; Rho uses ATPase helicase activity instead.
- ❌ **"Eukaryotic RNAP II directly binds the TATA box"** — TATA box is recognized by TBP (part of TFIID); RNAP II is recruited by general transcription factors.

---

## Practice Questions

1. A mutation changes the –10 box of a promoter from TATAAT to TAGAAT. Predict the effect on transcription. Explain why.

2. What is the difference between Rho-independent and Rho-dependent termination? Which requires ATP?

3. A eukaryotic mRNA lacks a 5' cap. What are the predicted functional consequences in the cytoplasm?

4. Compare the roles of σ⁷⁰ and σ³² in *E. coli*. Why is it advantageous to regulate transcription at the level of σ factor?

5. The consensus at the –35 box for σ⁷⁰ is TTGACA. A promoter variant has TTGCCA. Would you expect increased or decreased transcription? Why?

---

## Related Concepts

- [[Transcription]]
- [[Transcription]]
- [[Translation]]
- [[Translation]] — uses the mRNA product
- [[Lac Operon]] — transcriptional regulation
- [[Transcription Attenuation]]
