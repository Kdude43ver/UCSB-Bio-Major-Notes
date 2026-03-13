# High-Yield Mechanisms — Quick Reference Card

**Purpose**: One-page summary of most likely exam mechanisms. Memorize these!

---

## 1. MMR (Mismatch Repair) — The Strand Discrimination Machine

**Problem**: DNA Pol III incorporates wrong nucleotide occasionally → mismatch (G-T, A-A, etc.)

**Solution**:
```
STEP 1: MutS recognizes mismatch
        ↓
STEP 2: MutL recruited; complex slides along DNA
        ↓
STEP 3: MutH binds to hemimethylated GATC
        (Parental = methylated; New = unmethylated)
        MutH nicks unmethylated strand (the new one)
        ↓
STEP 4: Exonuclease I degrades from nick → past mismatch (5'→3')
        ↓
STEP 5: DNA Pol III resynthesizes excised region
        ↓
STEP 6: DNA Ligase seals nick
        ↓
STEP 7: Dam methylase methylates new strand at GATC
```

**Key Insight**: Hemimethylation = transient marker of new strand

**Repair Accuracy**: Reduces error rate from 10^-10 to 10^-12

---

## 2. NER (Nucleotide Excision Repair) — The Distortion Detector

**Problem**: Thymine dimer (TT covalently bonded) blocks replication/transcription

**Solution**:
```
STEP 1: UvrA scans DNA (ATPase activity)
        ↓
STEP 2: UvrB detects distortion; remains bound
        ↓
STEP 3: UvrC arrives; makes TWO CUTS:
        - Cut 1: ~5 nt UPSTREAM of lesion
        - Cut 2: ~8 nt DOWNSTREAM of lesion
        Total excision: 12-13 nucleotides
        ↓
STEP 4: UvrD (helicase) unwinds and removes oligonucleotide (+ lesion)
        ↓
STEP 5: DNA Pol I fills gap (also has 5'→3' exonuclease to trim)
        ↓
STEP 6: DNA Ligase seals
```

**Key Insight**: Excision size is FIXED (12-13 nt), not lesion size

**Target Damage**: Any bulky distortion (TT dimer, bulky adducts)

---

## 3. BER (Base Excision Repair) — The Precision Knife

**Problem**: Single damaged base (8-oxoG, uracil, thymine glycol)

**Solution**:
```
STEP 1: DNA Glycosylase (base-specific)
        Recognizes damage; cleaves N-glycosidic bond
        Leaves AP (apurinic/apyrimidinic) site
        ↓
STEP 2: AP Endonuclease (APE1)
        Cuts backbone 5' to AP residue
        ↓
STEP 3: DNA Pol I (SHORT-PATCH, most common)
        Removes AP residue + adds 1 replacement nt
        OR
        DNA Pol δ (LONG-PATCH, complex lesions)
        Adds multiple nt; FEN1 removes 5' flap
        ↓
STEP 4: DNA Ligase seals
```

**Key Insight**: Lesion-specific glycosylases = BER's recognition specificity

**Common Lesions**:
- 8-oxoG (oxidative stress) → 8-oxoguanine glycosylase
- Uracil (deamination) → Uracil DNA glycosylase
- Thymine glycol (UV) → Thymine glycol glycosylase

---

## 4. DSB Repair via HR (Double-Strand Break via Homologous Recombination)

**Problem**: Both strands broken; cell death if unrepaired

**Solution**:

### RecBCD Pathway (Primary)

```
STEP 1: RecBCD complex binds broken DNA end
        RecB = 3'→5' helicase + nuclease
        RecC = Chi site sensor
        RecD = 5'→3' helicase
        ↓
STEP 2: RecBCD degrades dsDNA (unwind + nuclease activity)
        Direction: 3'→5'
        ↓
STEP 3: Upon hitting Chi site (5'-GCTGGTGG-3'):
        RecC signals → Nuclease SWITCHES
        Now generates 3' ssDNA tail (~10 kb)
        ↓ [THIS IS THE KEY TRANSFORMATION]
STEP 4: RecA loads on 3' ssDNA
        Forms nucleoprotein filament
        ↓
STEP 5: RecA-ssDNA scans homologous dsDNA
        Upon homology, invades → D-loop forms
        ↓
STEP 6: DNA Pol III extends invading 3' end
        Synthesizes new DNA using target as template
        ↓
STEP 7: RuvAB binds Holliday junction
        (Motor protein; stabilizes branch point)
        ↓
STEP 8: RuvC cleaves junction (two options):
        - Vertical cut → crossover (recombinant)
        - Horizontal cut → patch (non-crossover)
```

**Critical Feature**: Chi site recognition switches RecBCD from degradation to 3' tail generation

---

## 5. SOS Response — Emergency Mode

**Trigger**: Single-stranded DNA (from damage or stalled replication fork)

**Mechanism**:

```
STEP 1: RecA binds ssDNA → RecA* (activated)
        ↓
STEP 2: RecA* stimulates LexA autocleavage
        (LexA has intrinsic serine protease activity)
        ↓
STEP 3: LexA (repressor) levels drop
        ↓
STEP 4: ~40 SOS genes derepressed:
        - *umuDC* (error-prone Pol V)
        - *dinB* (error-prone Pol IV)
        - *recF*, *recO*, *recR* (recombination)
        - *uvrA*, *uvrB*, *uvrC* (NER) [wait, these are actually basal, not SOS]
        - *dnaB*, *dnaK* (replication/chaperones)
        ↓
STEP 5: Pol V bypasses lesions (low fidelity; ~10^-1 error rate)
        Cell survives replication that would otherwise stall
        ↓
STEP 6: Upon damage repair: ssDNA disappears
        RecA* → RecA (inactive)
        LexA synthesis resumes
        SOS genes repressed
```

**Strategic Trade-off**: Accept mutagenesis to survive (better than death)

---

## 6. Holliday Junction Resolution — The 4-Way Branch

**Structure**: Two homologous dsDNA molecules connected at a single point; strands cross

**Resolution** (by RuvC endonuclease):

```
        ─ A ──────── B ─
        │                │
        │    Junction    │
        │                │
        ─ a ──────── b ─

RuvC CUTS two homologous strands:

OPTION 1 (Horizontal cut):
Result = Patch (non-crossover)
No exchange of outer markers
A is still with B; a still with b

OPTION 2 (Vertical cut):
Result = Crossover (recombinant)
Exchange of outer markers
A ends with b; a ends with B
```

**Gene Conversion** (if mismatch in heteroduplex during branch migration):
- Heteroduplex contains mismatches (e.g., A-a at polymorphic site)
- Mismatch repair "corrects" one way (all A-A or all a-a)
- Results in non-Mendelian ratios (3:5 or 5:3 in meiosis, not 4:4)

---

## 7. Hfr Interrupted Mating — Time = Distance

**Key Idea**: Genes transfer in linear order; TIME of entry = DISTANCE

**Process**:

```
oriT (Origin of Transfer, integrated in Hfr)
   ↓
MATING INITIATES
   ↓
Chromosome transfers linearly:
- Gene A enters at 5 min
- Gene B enters at 12 min
- Gene C enters at 18 min
   ↓
MATING INTERRUPTED (e.g., by agitation at 15 min)
   ↓
MAPPING:
A to B = 12 - 5 = 7 map units
B to C = 18 - 12 = 6 map units
A to C = 18 - 5 = 13 map units
```

**Why useful**:
- Linear transfer = clear gene order
- No need for recombination frequency calculations
- Can map hundreds of genes in one mating

**Recombinant Selection**:
- Select for F- markers (e.g., *lac-*, *gal-*)
- Look for cells that received Hfr alleles + recombined them in

---

## 8. RecBCD Chi Site Recognition — The Molecular Switch

**Critical Moment**: When RecBCD encounters Chi site (5'-GCTGGTGG-3')

**BEFORE Chi**:
```
RecBCD helicase unwinds dsDNA
Nuclease activity (on RecB) degrades strand: 3'→5' direction
```

**AT Chi Site**:
```
RecC protein senses Chi sequence
Sends allosteric signal to RecB nuclease
NUCLEASE ACTIVITY SWITCHES
```

**AFTER Chi**:
```
RecBCD still unwinds (helicase still works)
BUT nuclease no longer degrades
Instead: generates 3' ssDNA tail
RecA can load on this tail
```

**Why Important**: Creates optimal substrate for RecA (3' ssDNA)

**Alternative**: If no Chi site found, RecBCD just degrades both strands (→ no recombination, degradation pathway)

---

## 9. PCR Primer Design — Tm Matters

**Three Requirements**:

1. **Primer Length**: 18-25 nt (typical)
   - Too short → non-specific
   - Too long → harder to synthesize, may misfold

2. **Melting Temperature (Tm)**:
   - Rough: Tm = 4(G+C) + 2(A+T)
   - Accurate: various algorithms (e.g., Nearest-neighbor)
   - Typical range: 50-65°C
   - **EQUAL TM BOTH PRIMERS**: Ideal ±2°C difference
   - Use **lower of the two Tm values minus 2-5°C** for annealing temperature

3. **Specificity**:
   - Avoid self-complementarity (hairpin)
   - Avoid primer-dimer (forward + reverse binding to each other)
   - Check against genome for off-target binding
   - Avoid highly repetitive sequences

**Annealing Temperature** = Tm(lower primer) - 2-5°C

**Why this works**:
- Higher than annealing temp: denaturation ensures separation
- At annealing temp: primers find targets (Tm determines efficiency)
- Lower than Tm: specificity improves

---

## 10. Sanger Sequencing — ddNTP Chain Termination

**Key Chemistry**: ddNTP lacks 3'-OH group

```
dNTP:                      ddNTP:
    O                           O
    ║                           ║
─P─O─ (5' phosphate)     ─P─O─ (5' phosphate)
    │                           │
   sugar                        sugar
    │                           │
   3'─OH ← allows next       3'─H ← NO OH
   nucleotide addition        chain termination!
```

**Reaction**:

```
STEP 1: Denature template to ssDNA
        ↓
STEP 2: Anneal primer immediately 5' to target region
        ↓
STEP 3: Mix with:
        - Polymerase (Klenow or modern)
        - dNTPs (high, ~100 µM)
        - ddNTPs (low, ~1 µM, each labeled with different fluorescent dye)
        - Buffer
        ↓
STEP 4: Polymerase extends from primer
        At each position: 99% chance dNTP (continue)
                        1% chance ddNTP (terminate)
        ↓
STEP 5: Result = population of DNA fragments
        Each terminated by ddA, ddC, ddG, or ddT
        Sizes: primer+1, primer+2, primer+3, ... primer+n
```

**Separation**:
- Capillary electrophoresis (or gel)
- Separate by size
- Smallest fragments = closest to primer = read first
- Read sequence 5'→3' (direction of synthesis)

**Detection**:
- Fluorescence detector
- Each fragment's label read as it passes
- Automated base calling

**Accuracy**: ~99.9% per base
**Read Length**: 500-1000 bp (limited by template secondary structure, polymerase speed)

---

## Quick Study Tips

### For Each Mechanism, Know:
1. **What problem does it solve?** (What damage type?)
2. **Key enzymes** (name + function)
3. **Step-by-step process** (what happens when?)
4. **Strand discrimination** (how does cell know which one is damaged?)
5. **Outcome** (what's left after repair?)

### Comparison Strategy:
Create table comparing:
- MMR vs. NER vs. BER vs. DSB
- Damage recognized, enzymes used, excision size, accuracy, consequence of failure

### Visualization:
- Draw each pathway
- Label enzyme names above arrows
- Mark critical steps (e.g., Chi recognition)
- Use color: blue = recognition, yellow = cutting, green = synthesis, red = ligation

### Test Yourself:
- Explain each mechanism WITHOUT looking at notes
- Explain what happens if a key enzyme is mutated
- Predict which pathway repairs specific damage types
- Distinguish between similar mechanisms (e.g., NER vs. BER)

---

## Exam Day Checklist

Before exam:
- [ ] Memorize all enzyme names + abbreviations
- [ ] Know key numbers (12-13 nt NER, 5' of lesion, Chi site sequence)
- [ ] Practice drawing mechanisms
- [ ] Understand WHY each step happens (not just WHAT happens)

During exam:
- [ ] Read question carefully (asks for mechanism, comparison, prediction?)
- [ ] Take 1 min to outline answer before writing
- [ ] Draw diagrams if helpful (arrows, enzyme names, DNA sequences)
- [ ] Explain, don't just list steps
- [ ] Check: Did I answer the actual question asked?

---

**File Location**: `/sessions/practical-happy-hopper/mnt/Obsidian Vault/04_Course_Notes/MCDB 101A/High-Yield Mechanisms Quick Reference.md`

**Last Updated**: 2026-03-12
