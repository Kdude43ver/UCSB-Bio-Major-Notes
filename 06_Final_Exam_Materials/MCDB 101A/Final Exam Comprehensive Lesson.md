# Final Exam Comprehensive Lesson — Post-Midterm 2 Genetics

**Course:** MCDB 101A — Molecular Genetics I
**Coverage:** Lectures 11–17 (Mutations, DNA Repair, Recombination, Gene Transfer, Molecular Techniques)
**Level:** Junior Undergraduate
**Last Updated:** 2026-03-12

---

## Overview & Learning Objectives

This lesson covers the second half of MCDB 101A, spanning from spontaneous and induced mutations through advanced molecular techniques used to study and manipulate genes.

### By the end of this lesson, you should be able to:

1. **Mutations**: Explain the types, rates, and causes of mutations; distinguish between spontaneous and induced mutations
2. **DNA Repair**: Describe all major DNA repair pathways (MMR, NER, BER, DSB repair) and their mechanisms
3. **Recombination**: Explain homologous recombination models (Holliday, RecBCD) and site-specific recombination
4. **Gene Transfer**: Analyze bacterial conjugation, transduction, and transformation as mechanisms of horizontal gene transfer
5. **Molecular Techniques**: Apply restriction enzymes, PCR, Sanger sequencing, and other molecular tools to solve genetic problems
6. **SOS Response**: Understand the bacterial emergency response to DNA damage and its role in mutagenesis

---

## Module 1: Mutations (Lecture 11)

### 1.1 Definitions & Classification

**Mutation**: A heritable change in DNA sequence.

#### Types by Scope:
- **Point Mutations**: Single nucleotide substitutions
  - **Transitions**: Purine ↔ Purine (A ↔ G) or Pyrimidine ↔ Pyrimidine (C ↔ T)
  - **Transversions**: Purine ↔ Pyrimidine (less common, ~25% of random point mutations)
- **Insertions**: Addition of one or more nucleotides
- **Deletions**: Loss of one or more nucleotides
- **Inversions**: Reversal of a DNA segment
- **Duplications**: Repetition of a DNA segment

#### Types by Consequence:
- **Silent/Synonymous**: No change to amino acid sequence (wobble position mutations)
- **Missense**: Change in amino acid (may or may not affect protein)
- **Nonsense**: Creation of stop codon (premature termination)
- **Frameshift**: Insertion/deletion not divisible by 3 (changes all downstream codons)

### 1.2 Spontaneous vs. Induced Mutations

#### Spontaneous Mutation Rates
- **Typical Rate**: 10^-9 to 10^-10 per base pair per cell division in bacteria
- **Per Gene Rate**: ~10^-6 to 10^-8 per gene per generation
- **Causes**:
  - DNA replication errors (despite proofreading)
  - Spontaneous chemical changes (e.g., deamination, oxidation)
  - Errors in DNA repair

#### Sources of Spontaneous Mutations
1. **Replication Errors**: DNA polymerase occasionally incorporates wrong nucleotide despite 3'→5' exonuclease activity
2. **Spontaneous Lesions**:
   - **Deamination**: Cytosine → Uracil (recognized & repaired by BER), 5-methylcytosine → Thymine (often escapes repair)
   - **Oxidative Damage**: Reactive oxygen species (ROS) create 8-oxoguanine and other lesions
3. **Tautomeric Shifts**: Rare forms of bases allow aberrant pairing during replication

#### Induced Mutations
**Induced Mutation**: A change in DNA caused by external mutagen exposure.

**Chemical Mutagens**:
- **Alkylating Agents** (e.g., EMS, MMS): Add alkyl groups to guanine/adenine → mispairing
- **Intercalating Agents** (e.g., acridine, ethidium bromide): Insert between base pairs → frameshift mutations
- **Base Analogs** (e.g., 5-bromouracil, 2-aminopurine): Incorporated into DNA; exhibit abnormal pairing

**Physical Mutagens**:
- **UV Light**: Causes thymine dimers (TT → TT with covalent bond) → distorts DNA & blocks replication/transcription
- **Ionizing Radiation** (X-rays, gamma rays): Causes double-strand breaks and point mutations
- **Nitrous Acid (HNO₂)**: Deaminates amino groups on bases (A→hypoxanthine, C→uracil)

### 1.3 The Luria-Delbrück Fluctuation Test

**Experimental Question**: Are phage-resistant mutations pre-existing or induced by phage exposure?

**Method**:
1. Grow 10^7 bacteria (wild-type, *lac*+ or phage-sensitive)
2. **Fluctuation Cultures**: Inoculate many small separate flasks with ~100 bacteria each; grow to ~10^8 cells
3. **One Large Culture**: Grow one culture to 10^8 cells in one vessel
4. Plate all cultures on medium with phage

**Results**:
- **Fluctuation (separate) cultures**: High variance in number of resistant colonies—some cultures have "jackpot" (many resistant colonies), others have none
- **Large culture**: Consistent, low number of resistant colonies

**Conclusion**: High variance in fluctuation cultures proves mutations arose **randomly before selection** (independent of phage exposure). If mutations were induced by phage, all cultures would show similar variance.

**Mathematical Basis**: If resistant mutants are pre-existing and arise during growth at constant rate μ, the variance among cultures is much higher than the mean (indicating Poisson fluctuations). If induced by selection, variance ≈ mean.

### 1.4 Mutation Rate Estimation

**Notation**:
- μ = mutation rate per cell per generation (or per base pair per replication)
- N = number of cells at time of plating
- r = number of resistant mutants observed

**Relationship**: E(r) = μN

**Example Calculation**:
If 10 separate cultures of ~10^8 cells show mutation counts of (0, 0, 0, 0, 0, 0, 2, 0, 0, 56):
- Mean = 5.8, Variance ≈ 248 (high variance indicates pre-existing mutations)
- Jackpot culture (56) likely arose from a single mutation early in growth, which then proliferated

---

## Module 2: DNA Repair (Lectures 12–13)

DNA damage is constant; cells employ multiple repair mechanisms, each specialized for specific damage types.

### 2.1 Overview of Repair Pathways

| Pathway | Damage Type | Key Enzymes | Mechanism |
|---------|------------|------------|-----------|
| **MMR** | Replication errors, mismatches | MutS, MutL, MutH | Recognize hemimethylated mismatch; nick new strand; degrade & resynthsize |
| **NER** | Thymine dimers, bulky adducts | UvrA, UvrB, UvrC, UvrD | Excise 12–13 nt segment containing lesion |
| **BER** | Oxidized bases, uracil, 8-oxoG | DNA glycosylase, APE1, Pol I | Remove damaged base; cleave at AP site; fill & ligate |
| **DSB Repair** | Double-strand breaks | RecBCD, RecA, RuvAB, RuvC | Homologous recombination (HR) or non-homologous end joining (NHEJ) |

### 2.2 Mismatch Repair (MMR) — The Proofreading System

**Role**: Removes replication errors not caught by polymerase exonuclease (3'→5' proofreading).

**System in *E. coli***:
- **MutS**: Recognizes mismatched base pairs (e.g., G-T, A-A)
- **MutL**: Recruited by MutS; coordinates the repair process
- **MutH**: Endonuclease that nicks the new (unmethylated) strand

**Mechanism**:

1. **Recognition**: MutS dimer scans DNA; upon mismatch detection, undergoes conformational change
2. **Coupling**: MutS recruits MutL; complex slides along DNA
3. **Strand Discrimination** (Key!): *E. coli* methylates **GATC** sequences at adenine using Dam methylase
   - Parental strand: methylated (adenine is methylated)
   - New strand: temporarily hemimethylated (unmethylated adenine)
   - MutH recognizes hemimethylated GATC and nicks the unmethylated (new) strand
4. **Degradation**: Exonuclease I degrades the nicked new strand in the 5'→3' direction (toward mismatch)
5. **Resynthesis**: DNA Pol III replaces the excised segment; DNA ligase seals
6. **Methylation**: Dam methylase methylates the new GATC sequence

**Eukaryotic MMR**: Uses **PCNA** (processivity factor) instead of methylation to recognize new strand; MLH1/MLH3/MSH complexes instead of Mut proteins.

**Clinical Significance**: Mutations in human mismatch repair genes (MLH1, MSH2, MSH6) → Lynch syndrome (hereditary non-polyposis colorectal cancer).

### 2.3 Nucleotide Excision Repair (NER) — The Versatile System

**Role**: Removes large, distorting DNA lesions that don't fit standard base-pairing (thymine dimers, bulky adducts).

**Key Substrate**: Thymine dimer from UV exposure.

**Mechanism in *E. coli***:

1. **Recognition**: UvrA (ATPase) + UvrB dimer scan DNA; UvrB identifies distortion
2. **Dual Incision**: UvrBC complex makes incisions:
   - 5 nucleotides upstream of lesion (UvrC)
   - 8 nucleotides downstream of lesion (UvrC)
   - **Total removed**: 12–13 nucleotides
3. **Displacement**: UvrD (DNA helicase II) unwinds and removes the oligonucleotide segment
4. **Resynthesis**: DNA Pol I fills the 12–13 nt gap (has 5'→3' exonuclease for removal + polymerase for synthesis)
5. **Ligation**: DNA ligase seals the nick

**Eukaryotic NER** (Transcription-Coupled Repair, TCR):
- TFIIH complex recognizes stalled RNA polymerase at lesion
- XPA, XPB, XPD, XPE, XPF nucleases perform dual incision
- Similar 25–32 nt excision

**SOS Response Coupling**: In bacteria, extensive UV damage triggers SOS response → error-prone polymerases (Pol V) → increased mutation rate.

### 2.4 Base Excision Repair (BER) — The Surgical System

**Role**: Removes damaged bases (8-oxoguanine, uracil, thymine glycol) and abasic sites.

**Mechanism**:

1. **Base Removal**: DNA glycosylase scans DNA; recognizes damaged base via enzyme's active site specificity
   - Examples: UracilDNA glycosylase (removes U), 8-oxoguanine glycosylase (removes 8-oxoG)
   - Catalyzes N-glycosidic bond cleavage → creates apurinic/apyrimidinic (AP) site
2. **AP Site Cleavage**: AP endonuclease (APE1) cuts backbone 5' to AP site
3. **Gap Filling**:
   - **Short-patch BER**: DNA Pol I removes AP residue + adds 1 nt; DNA ligase seals
   - **Long-patch BER**: DNA Pol δ adds multiple nucleotides; flap endonuclease removes 5' flap
4. **Ligation**: DNA ligase seals final nick

**Base Damage Examples**:
- **8-oxoguanine**: Oxidized guanine; mimics thymine in pairing (G:C → G:T→A:T after replication)
- **Uracil**: Spontaneous cytosine deamination or incorporation of dUMP; recognized by uracil glycosylase
- **Thymine Glycol**: UV-induced; recognized by thymine glycol glycosylase

### 2.5 Double-Strand Break (DSB) Repair

**Challenge**: Complete breaks in both strands are lethal if not repaired; two main pathways in bacteria.

#### Homologous Recombination (HR) — Accurate Repair

**Requirement**: Homologous DNA template (sister chromatid or homolog).

**RecBCD Pathway** (primary in *E. coli*):

1. **Recognition**: RecBCD complex binds broken end; contains:
   - RecB: helicase + nuclease
   - RecC: recognizes Chi sites
   - RecD: helicase

2. **Degradation & Chi Recognition**:
   - RecBCD degrades dsDNA (helicase activity unwinds, nuclease activity degrades in 3'→5' direction)
   - Upon encountering **Chi site** (5'-GCTGGTGG-3'), RecC signals change:
     - Nuclease activity **switches** to generate 3' single-stranded tail (~10 kb)
     - This 3' ssDNA is perfect substrate for RecA loading

3. **RecA Loading**:
   - RecA coats the 3' ssDNA tail (ATP-dependent)
   - Forms nucleoprotein filament
   - Promotes homology search in double-stranded DNA

4. **Strand Invasion**:
   - RecA-ssDNA filament scans dsDNA
   - Upon finding homology, invades target dsDNA
   - Creates **D-loop** (displacement loop): 3' end of invading strand primes DNA synthesis

5. **Resolution**:
   - DNA Pol III extends invading 3' end, synthesizing new DNA strand
   - RuvAB complex recognizes Holliday junction; RuvAB binds (motor protein activity)
   - **RuvC** endonuclease cleaves Holliday junction at two homologous sites
   - Cleavage generates either **crossover** (recombinant) or **patch** (non-crossover) products

**RecFOR Pathway** (secondary; for small gaps):
- RecF, RecO, RecR facilitate RecA loading on ssDNA gaps
- Less efficient at DSBs; primarily handles gaps left after replication

#### Non-Homologous End Joining (NHEJ) — Error-Prone Repair

- Direct ligation of broken ends without template
- Error-prone; can result in small deletions
- More prevalent in eukaryotes (uses Ku70/Ku80 complex); rare in *E. coli*

### 2.6 The SOS Response

**Trigger**: Single-stranded DNA (ssDNA) from unrepaired damage or stalled replication forks.

**Mechanism**:

1. **ssDNA Detection**: RecA protein binds ssDNA; undergoes conformational change to RecA*

2. **LexA Autocleavage**: RecA* stimulates RecA-mediated self-cleavage of **LexA** repressor (protease activity)
   - LexA normally represses ~40 SOS genes (*recA*, *lexA*, *umuDC*, *sulA*, etc.)

3. **Gene Derepression**: As LexA levels drop, SOS genes are transcribed:
   - **DNA repair genes**: *uvrABC*, *recF*, *recN*, *polB* (Pol II)
   - **Error-prone polymerases**: *umuDC* (Pol V) & *dinB* (Pol IV) — bypass lesions but with low fidelity
   - **Mutagenic recombination**: *recF*, *recR*, *recO*

4. **Transient Mutagenesis**: Error-prone polymerases tolerate lesions (especially thymine dimers), allowing replication to continue but introducing mutations

5. **Recovery**: Upon repair of damage, ssDNA decreases → RecA* reverts → LexA is synthesized → SOS genes are repressed

**Key Point**: SOS response is a "bet-the-farm" strategy—cells accept increased mutation rate to survive otherwise lethal damage.

---

## Module 3: Homologous Recombination & Genetic Mapping (Lecture 14)

### 3.1 The Holliday Model

**Historical Context**: Robin Holliday (1964) proposed a symmetrical model for meiotic recombination; later applied to mitotic recombination.

**Key Structures**:

**Holliday Junction**: Four-way DNA junction where two homologous dsDNA molecules are connected at a point of strand exchange.

```
        ─ A ─
        │   │
    ─ a ┤   ├ b ─
        │   │
        ─ B ─
```

### 3.2 Steps of Homologous Recombination (Holliday Model)

1. **Strand Breakage & Invasion**:
   - Single-strand nick (or DSB) in one strand of each molecule
   - Invading strand displaces complement, creating D-loop

2. **Branch Migration**:
   - Holliday junction moves along DNA (resolution point migrates)
   - Can involve hundreds or thousands of base pairs
   - Allows heteroduplex DNA formation (mismatched base pairs at crossover point)

3. **Mismatch Repair During Branch Migration**:
   - Heteroduplex regions may contain mismatches from polymorphisms
   - Mismatch repair can create **gene conversion**—non-reciprocal transfer of genetic information

4. **Resolution** (Holliday Cleavage):
   - Two homologous strands of the Holliday junction are cleaved by resolvase (RuvC)
   - Can cleave horizontally (vs. vertically) through junction:
     - **Horizontal cleavage** (one pair of opposite strands) → **non-crossover** (patch) product
     - **Vertical cleavage** (other pair of opposite strands) → **crossover** product

### 3.3 Double-Strand Break (DSB) Model — Modern Mechanism

The Holliday model describes the chemical events; the DSB repair model explains *how* the process is initiated in *E. coli*.

**Key insight**: Most recombination initiates from a **double-strand break**, not a single nick.

**RecBCD Pathway** (already covered in Section 2.5):
- RecBCD processes broken end → generates 3' ssDNA tail
- RecA loads on 3' ssDNA
- RecA-ssDNA filament performs homology search
- Invades homologous dsDNA
- RuvAB + RuvC resolve junctions

### 3.4 Gene Conversion & Holliday Junction Resolution

**Gene Conversion**: Non-reciprocal recombination; one strand's sequence is "corrected" to match the other.

**Mechanism**:
- During branch migration, heteroduplex DNA forms (e.g., A-T mismatch on one side, T-A on other)
- Mismatch repair machinery (MutS, MutL) recognizes mismatch
- Can repair in either direction:
  - If repairs to A:T on one side, T:A (original) on other → gene conversion (1:1 instead of 1:1)
  - Typically biased toward one allele (creates non-Mendelian segregation ratios)

**Observable Phenotype**: In meiosis, asci may show 4:4 (normal) or 3:5, 5:3 (gene conversion) ratios for markers near crossover point.

### 3.5 Mapping by Recombination Frequency

**Principle**: Recombination frequency is proportional to distance between genes.

**Derivation**:
- Two linked genes: A-B at distance d (centiMorgans = cM)
- Probability of odd number of crossovers between them = d/100 (if measured in %); in map units (Morgans), equals d directly
- **Recombination frequency (RF)** = (# recombinants / total progeny) × 100%

**Example**:
- Cross: A B / a b (coupling) × a b / a b (testcross)
- Progeny: 450 A B : 430 a b (parental) : 35 A b : 40 a B (recombinant)
- RF = (35 + 40) / 955 × 100% = 7.85% ≈ 8 map units apart

**Three-Point Cross**:
- Three linked genes (A, B, C)
- Identifies which gene is in middle by analyzing double-crossover class (rarest)
- Allows determination of coefficient of coincidence (COC) and interference

---

## Module 4: Gene Transfer in Bacteria (Lecture 15)

**Definition**: Horizontal gene transfer (HGT)—acquisition of DNA from another organism, not inherited from parent.

### 4.1 Transformation

**Definition**: Uptake of naked DNA from environment.

**Competence**: Ability to take up exogenous DNA.
- **Natural competence**: Some bacteria (e.g., *Streptococcus*, *Vibrio*, *Bacillus*) naturally competent
- **Artificial competence**: CaCl₂-treatment or electroporation makes cells competent

**Mechanism**:
1. DNA binds to competence proteins (ComE, ComD, etc.) on cell surface
2. Single strand is imported; complementary strand remains in medium
3. Single-stranded DNA is protected from nucleases
4. ssDNA enters chromosome via RecA-mediated recombination OR replicates as plasmid

**Efficiency**: Usually low (~0.1%–1% of treated cells take up DNA).

**Griffith Experiment (1928)**:
- *S. pneumoniae*: Smooth (S, virulent) vs. Rough (R, avirulent)
- Heat-killed S + live R → mice died; S recovered from lungs
- Conclusion: "Transforming principle" (later identified as DNA) transferred virulence

### 4.2 Transduction

**Definition**: Bacterial DNA transfer via bacteriophage vector.

#### Generalized Transduction

**Mechanism**:
1. Phage DNA replicates in host cell; phage head packaging machinery accidentally packages adjacent bacterial DNA (instead of phage DNA)
2. Phage particle with **only** bacterial DNA (no phage genes) is released
3. Upon infection of new cell, bacterial DNA is injected but cannot replicate (no phage replication genes)
4. Bacterial DNA can recombine into chromosome or circularize as plasmid

**Frequency**: ~1 per 10^6 phage particles; depends on DNA fragment size vs. phage head capacity.

**Characteristics**:
- Any bacterial genes can be transduced with equal probability
- **Abortive transduction**: Transduced DNA doesn't integrate, so unstable (diluted out)
- **Stable transduction**: Integration via homologous recombination

#### Specialized Transduction

**Context**: Temperate phage (e.g., lambda) integrating into chromosome.

**Mechanism**:
1. Lambda integrates at specific site (*attB*) between *gal* and *bio* genes
2. Upon induction, rare aberrant excision occurs:
   - Excises at normal *att* site on one side, but at abnormal site on other
   - Takes adjacent bacterial genes (*gal* or *bio*) but leaves behind some phage genes
   - Result: **defective phage** carrying *gal* or *bio*
3. This defective phage can only replicate in presence of helper phage (wild-type)

**Characteristics**:
- Only genes adjacent to integration site are transduced
- Phage particle carries **both** phage and bacterial DNA
- Requires helper phage for replication

**Example**: *λdgal* (lambda defective in *gal*) carries *gal* genes; cannot replicate alone.

### 4.3 Conjugation

**Definition**: Direct transfer of DNA between two bacteria via pilus.

#### F Plasmid & Hfr Strains

**F Plasmid** (Fertility):
- ~100 kb plasmid; encodes:
  - **tra genes**: Transfer machinery (pilus, coupling proteins, ATPases)
  - **ori**: Origin of replication
  - **oriT**: Origin of transfer

**Mating Types**:
- **F+ (Donor)**: Contains F plasmid; produces pilus
- **F- (Recipient)**: Lacks F plasmid; has no pilus
- **Hfr (High frequency recombination)**: F plasmid integrated into chromosome

**F+ × F- Mating**:
1. F+ extends pilus; connects to F- cell
2. Mating pair stabilizes via DNA transfer channel
3. Rolling circle replication at **oriT**: single strand nicks and unwinds
4. Complementary strand synthesized in donor; nicked strand transferred to recipient
5. Recipient synthesizes complementary strand
6. Both cells are now F+ (plasmid replicates autonomously)
7. Transfer usually completes in ~100 minutes

**Hfr × F- Mating** (Interrupted Mating):
1. Hfr initiates chromosome transfer from integrated **oriT** site
2. Chromosome transfers linearly: specific genes enter recipient in predictable order
3. Mating usually interrupted before complete transfer (~12 minutes for first markers)
4. Recipients become **F- merodiploids** (partial diploids) for transferred genes

**Hfr Mapping**:
- **Time of entry (TOE)**: Time at which a marker first appears in recipient
- **Gene order**: Determined by TOE sequence
- **Distance**: TOE intervals indicate relative distance
- Example: If gene A appears at 5 min, gene B at 8 min, they are 3 min apart (~3% recombination frequency on Hfr chromosome)

**Recombination in Recipient**:
- Transconjugant DNA recombines with recipient chromosome via homologous recombination
- Meiotic selection: selection for recipient chromosome marker + Hfr marker confirms recombination

### 4.4 Fertility Factors & Episomes

**F' (F-prime)**: F plasmid that has excised from Hfr, carrying adjacent bacterial genes.
- Example: F' (*lac*+) carries *lac* operon genes; very useful for complementation testing

**Episome**: DNA that can exist as plasmid OR integrate into chromosome.
- F plasmid is an episome
- Lambda phage is an episome

---

## Module 5: Molecular Techniques (Lecture 16)

### 5.1 Restriction Enzymes (Restriction Endonucleases)

**Definition**: Endonucleases that recognize and cleave DNA at specific sequences.

**Discovery**: Bacteria use restriction enzymes as defense against foreign DNA (restriction-modification system); methylation protects own DNA.

**Recognition Sequences**:
- **Palindromic**: Same sequence read 5'→3' on both strands
  - Example: EcoRI recognizes 5'-GAATTC-3' / 3'-CTTAAG-5'
  - Creates **sticky ends** (cohesive ends): 5' overhangs of 4 nt
  - Example: 5'-G        AATTC-3' / 3'-CTTAA        G-5'

- **Non-Palindromic**: Recognition site is asymmetric; rare

**Common Restriction Enzymes**:
| Enzyme | Source | Recognition | Cut Pattern |
|--------|--------|-------------|-------------|
| EcoRI | *E. coli* RY13 | GAATTC | G^AATTC (sticky) |
| PstI | *Providencia stuartii* | CTGCAG | CTGCA^G (sticky) |
| BamHI | *Bacillus amyloliquefaciens* | GGATCC | G^GATCC (sticky) |
| PvuII | *Proteus vulgaris* | CAG^CTG | CAG^CTG (blunt) |
| HaeIII | *Haemophilus aegyptius* | GG^CC | GG^CC (blunt) |

**Cutting Patterns**:
- **Sticky Ends** (cohesive, overhangs): 4–8 nt single-stranded overhangs; useful for ligation
- **Blunt Ends**: No overhangs; harder to ligate but can be force-ligated

### 5.2 Restriction Mapping

**Goal**: Determine order and distance of restriction sites on a DNA molecule.

**Method**:
1. Digest DNA with single restriction enzyme → cut at all recognition sites → produces fragments
2. Run on gel, measure fragment sizes
3. Digest with combinations of enzymes → compare patterns
4. Build map from overlapping fragments

**Example**:
- Digest with EcoRI alone: fragments of 2 kb, 3 kb, 4 kb (total 9 kb)
- Digest with BamHI alone: fragments of 1 kb, 5 kb, 3 kb
- Digest with EcoRI + BamHI: fragments of 1 kb, 1 kb, 2 kb, 2 kb, 3 kb
- **Map**: Determine arrangement by analyzing all three digests

### 5.3 DNA Cloning & Plasmids

**Recombinant DNA**: DNA formed by joining sequences from different sources.

**Process**:
1. Isolate vector (plasmid or phage) and insert DNA
2. Digest both with same restriction enzyme (creates compatible sticky ends)
3. Ligate insert DNA into vector using DNA ligase (seals nicks in sugar-phosphate backbone)
4. Introduce into bacterial host:
   - **Transformation**: CaCl₂ or electroporation
   - **Transduction**: Via phage
   - **Conjugation**: Via Hfr or F plasmid
5. Select recombinant clones (e.g., antibiotic selection, blue-white screening)

**Plasmid Features**:
- **ori** (origin of replication): Controls copy number (low, medium, high)
- **Selectable marker**: Antibiotic resistance gene (ampicillin, tetracycline, etc.)
- **cloning site**: Multiple restriction sites for inserting foreign DNA

**Blue-White Screening** (*lacZ*):
- Vector carries *lacZ* gene (encodes β-galactosidase)
- Cloning site within *lacZ*
- Bacteria grown on medium + X-gal (substrate)
- White colonies: *lacZ* disrupted (has insert)
- Blue colonies: *lacZ* intact (no insert)

### 5.4 PCR (Polymerase Chain Reaction)

**Invention**: Kary Mullis, 1983. Revolutionized molecular biology; won 1993 Nobel Prize.

**Goal**: Exponentially amplify specific DNA target (~10^9-fold in 25–30 cycles).

**Requirements**:
- Template DNA (even one copy)
- Two primers (oligonucleotides) flanking target, designed to anneal to opposite strands
- dNTPs (deoxyribonucleoside triphosphates)
- Thermostable DNA polymerase (usually *Taq* from *Thermus aquaticus*)
- Thermal cycler (switches between temperatures)

**Three-Step Cycle** (repeated 25–35 times):

1. **Denaturation** (94–95°C, 30 sec): dsDNA melts → ssDNA
2. **Annealing** (50–65°C, 30 sec): Primers bind to complementary sequences on template strands
3. **Extension** (72°C, varies): *Taq* polymerase extends from primer 3' end along template strand (3'→5' direction), synthesizing new strand

**After n Cycles**: DNA amount ≈ 2^n × initial amount

**Primer Design**:
- Typically 18–25 nucleotides
- Tm (melting temperature) usually 50–65°C
- Tm = 4(G+C) + 2(A+T) [rough formula]; more accurate methods available
- Primers should be specific (not self-complementary or primer-dimer)

**Applications**:
- Gene amplification (for cloning, analysis)
- Diagnosis (e.g., pathogen detection)
- Copy number variation (qPCR)
- Mutation screening

**qPCR (Real-Time PCR)**:
- Monitors amplification in real-time via fluorescence
- Allows quantification (instead of just end-point detection)
- Uses fluorescent reporters (SYBR Green, TaqMan probes)

### 5.5 DNA Sequencing

#### Sanger Sequencing (Chain-Termination Method)

**Principle**: Mix dNTPs with rare ddNTPs (dideoxyribonucleoside triphosphates); ddNTPs lack 3'-OH group, terminating synthesis when incorporated.

**Procedure**:
1. Denature template DNA to ssDNA
2. Anneal primer (immediately 5' to region of interest)
3. Add DNA polymerase + dNTPs + ~1% ddNTP (usually fluorescently labeled)
4. Polymerase extends from primer, incorporating dNTPs normally
5. Randomly, ddNTP incorporated → chain terminates
6. After reaction: mixture of DNA fragments of different lengths (each ends with a ddNTP)

**Separation**:
- Fragments separated by capillary electrophoresis (or gel) by size
- Each fragment's terminal ddNTP carries unique fluorescent label
- Detector reads label as each fragment passes: sequence read 5'→3'

**Accuracy & Read Length**:
- Highly accurate (~99.9%)
- Read length: typically 500–1000 bp per reaction (2-dye systems up to 800 bp)

**Chain Termination Mechanism**:
- ddATP, ddCTP, ddGTP, ddTTP each labeled with different fluorescent dye
- At each position in template, all four ddNTPs compete with dNTPs
- Probability of incorporation: ~1% (ddNTP) to 99% (dNTP)
- Creates population of fragments terminating at every position

#### Next-Generation Sequencing (NGS)

Briefly mentioned for context (not primary focus):
- **Illumina**: Cluster generation (bridge amplification), dye-terminator chemistry
- **Ion Torrent**: pH-based detection of nucleotide incorporation
- Much higher throughput (millions of reads) vs. Sanger's thousands

### 5.6 Applications of Molecular Techniques

**Forensics & Paternity**:
- PCR amplification of short tandem repeats (STRs)
- Sizing fragments by electrophoresis
- Comparison to known samples

**Disease Diagnosis**:
- qPCR detection of pathogen DNA/RNA
- Mutation screening in disease genes

**Transgenic Organisms**:
- Introduce foreign DNA into organisms
- Via microinjection (animals), electroporation (plants), *Agrobacterium* (plants)

**Gene Therapy**:
- Introduce functional gene copy to rescue genetic deficiency

---

## Module 6: Integration & Exam Strategy

### 6.1 Concept Map: Post-Midterm 2 Content

```
MUTATIONS (spontaneous, induced)
    ↓
    └─→ Drive evolution via selection
    └─→ Detected by: Luria-Delbrück test

DNA DAMAGE (from mutations, replication errors, environment)
    ↓
    └─→ SOS Response (emergency repair + mutagenesis)
    ├─→ MMR (replication errors)
    ├─→ NER (thymine dimers, bulky lesions)
    ├─→ BER (oxidative damage, deamination)
    └─→ DSB Repair (double-strand breaks)
        ├─→ RecBCD pathway
        ├─→ RecA-mediated recombination
        └─→ RuvAB + RuvC resolution

HOMOLOGOUS RECOMBINATION
    ├─→ Holliday junctions
    ├─→ Gene conversion (non-reciprocal)
    └─→ Mapping by recombination frequency

HORIZONTAL GENE TRANSFER
    ├─→ Transformation (naked DNA)
    ├─→ Transduction (phage-mediated)
    │   ├─→ Generalized (any genes)
    │   └─→ Specialized (specific genes near integration)
    └─→ Conjugation (pilus, direct transfer)
        ├─→ F+ → F- (F plasmid spread)
        └─→ Hfr → F- (chromosome transfer, interrupted mating mapping)

MOLECULAR TECHNIQUES
    ├─→ Restriction enzymes (palindromic recognition, sticky vs. blunt ends)
    ├─→ Restriction mapping (overlapping fragments)
    ├─→ PCR (exponential amplification, Tm, primer design)
    └─→ Sanger sequencing (ddNTP chain termination, fluorescent detection)
```

### 6.2 High-Yield Topics for Final Exam

Based on exam structure analysis:

**HIGH YIELD**:
1. **MMR Mechanism** — Likely tested as mechanism or problem-solving
   - Dam methylation → hemimethylation → MutH recognition of new strand
2. **RecBCD + Chi Site** — Critical for understanding DSB repair
   - Nuclease switches from degrading to generating 3' ssDNA upon Chi recognition
3. **Hfr Mapping (Time of Entry)** — Frequently tested; practical application
   - Can predict order and distance from timed mating interruptions
4. **PCR Fundamentals** — Cycles, Tm, primer design
   - Real-world applications (diagnostics, cloning)
5. **Sanger Sequencing Mechanism** — Why ddNTPs cause termination (lack 3'-OH)
6. **Holliday Junction Resolution** — Two cleavage options (crossover vs. patch)

**MEDIUM YIELD**:
1. NER pathway (recognition, dual incision, displacement)
2. Luria-Delbrück fluctuation test (variance analysis)
3. Lambda specialized transduction (defective phage)
4. Restriction enzyme recognition and sticky ends

**LOWER YIELD** (but still tested):
1. BER pathway (glycosylase-specific)
2. SOS response genes (*umuDC*, error-prone polymerases)
3. Blue-white screening
4. Poisson distribution application (MOI calculations)

### 6.3 Common Misconceptions & How to Avoid Them

1. **"MMR uses methylation in all organisms"**
   - FALSE: Only *E. coli* and some bacteria. Eukaryotes use PCNA & strand discontinuities.

2. **"Restriction enzymes cut all DNA at recognition sites"**
   - FALSE: Methylated sites (host DNA) are often protected; cutting depends on methylation status.

3. **"PCR cycle count determines final DNA amount exactly"**
   - INCOMPLETE: Assumes 100% efficiency per cycle (unrealistic); plateau effect at high cycles.

4. **"RecA only loads on double-stranded DNA"**
   - FALSE: RecA specifically binds **single-stranded DNA** (via RecBCD-generated 3' tail or naked ssDNA).

5. **"Transduction always gives stable inheritance"**
   - FALSE: Abortive transduction (non-integrated) is unstable; only integrated transductants are stable.

6. **"Hfr strains transfer F plasmid to recipients"**
   - FALSE: Hfr transfers **chromosome only** (F plasmid is integrated); F+ conjugation transfers F plasmid.

---

## Module 7: Practice Problem Set

### 7.1 Conceptual Questions

**Q1: DNA Damage & Repair**
A bacterial cell has a mutation in the *uvrB* gene (NER). What type(s) of DNA damage would accumulate if the cell were exposed to UV light? Why?

**Answer**:
- Thymine dimers would accumulate because NER is specifically responsible for removing UV-induced lesions.
- Without functional UvrB, the UvrBC complex cannot recognize or incise the damage.
- The cell might attempt SOS response (which can lead to error-prone repair) but would likely die due to unrepaired TT dimers blocking replication/transcription.

---

**Q2: Recombination Mapping**
An Hfr strain (*gal*+ *lac*+ *trp*+) is mated with an F- strain (*gal*- *lac*- *trp*-). Interrupted mating shows: *gal*+ enters at 5 min, *lac*+ at 12 min, *trp*+ at 18 min. Draw a genetic map.

**Answer**:
```
oriT ──5 min── gal+ ──7 min── lac+ ──6 min── trp+
```
- Distance: *gal* to *lac* = 7 min; *lac* to *trp* = 6 min
- Time of entry indicates transfer order and relative distance

---

**Q3: MMR Problem**
In a newly synthesized DNA strand, a G:C mismatch occurs opposite the parental A:T. Explain how *E. coli* MMR would resolve this, including the role of Dam methylation.

**Answer**:
1. Parental strand is methylated at GATC sites (adenine methylated by Dam methylase)
2. Newly synthesized strand is transiently hemimethylated (unmethylated adenine)
3. MutS recognizes G:C mismatch (actually G:T before correction)
4. MutH nicks unmethylated (new) strand at hemimethylated GATC
5. Exonuclease I degrades new strand from nick toward/past mismatch
6. DNA Pol III resynthesizes; DNA ligase seals
7. Dam methylase now methylates new strand at GATC

---

### 7.2 Molecular Technique Problems

**Q4: PCR Design**
You want to amplify a 500 bp region of a gene using PCR. The region starts at position 1000 and ends at position 1500 of a known sequence.

**Primers** (designed to flank the region):
- Forward primer: 5'-ATGCGATTACGATCC-3' (Tm = 58°C)
- Reverse primer: 5'-GGATCCGTACGTAAA-3' (Tm = 60°C)

(a) What is the length of the expected PCR product?
(b) What annealing temperature would you use?
(c) How many cycles would you need to amplify the region 10^5-fold?

**Answers**:
(a) 500 bp (the distance between primer binding sites)
(b) 56–58°C (typically use Tm of lower-Tm primer minus 2–5°C; lower than highest Tm)
(c) 2^n = 10^5 → n log(2) = 5 log(10) → n ≈ 16.6, so **17 cycles** to guarantee >10^5 amplification

---

**Q5: Restriction Mapping**
A 10 kb plasmid is digested with three restriction enzymes:
- EcoRI alone: 4 kb, 6 kb
- BamHI alone: 3 kb, 7 kb
- EcoRI + BamHI: 2 kb, 2 kb, 1 kb, 5 kb

Draw a restriction map, indicating EcoRI and BamHI sites.

**Answer**:
Work through overlaps:
- EcoRI cuts at positions 4 and 10 (or 0 and 4; circular plasmid)
- BamHI cuts at positions 3 and 10 (or 0 and 3)
- Double digest fragments: 0–2 (2 kb), 2–3 (1 kb), 3–5 (2 kb), 5–10 (5 kb)

One possible map:
```
    EcoRI (at 4)
       |
0 ──── B ──── E ──── 10
  BamHI|
   (at 3)

Fragment sizes (EcoRI): 0-4 (4 kb), 4-10 (6 kb) ✓
Fragment sizes (BamHI): 0-3 (3 kb), 3-10 (7 kb) ✓
Fragment sizes (double): 0-2, 2-3, 3-4, 4-10 → but that's not right...
```
(Correct map would require careful alignment; the key is overlapping fragments to determine enzyme positions.)

---

### 7.3 Integration Problem

**Q6: SOS Response Pathway**
A bacterial culture is exposed to UV light. Describe the molecular steps from DNA damage to expression of error-prone polymerase genes (*umuDC*), and explain why this is an adaptive response.

**Answer**:

1. **UV Damage**: TT dimers form in DNA
2. **Replication Stalling**: DNA polymerase III stalls at dimer; replication fork collapses
3. **ssDNA Generation**: Exonucleases degrade stalled fork region, generating ssDNA
4. **RecA Activation**: RecA binds ssDNA → RecA* (conformationally active)
5. **LexA Autocleavage**: RecA* stimulates LexA autoproteolytic cleavage
6. **Derepression**: As LexA (repressor) levels drop, SOS genes transcribed:
   - *umuDC* (Pol V), other error-prone polymerases
   - DNA repair genes (*recF*, *uvrA*, etc.)
7. **Error-Prone Synthesis**: Pol V bypasses lesions (e.g., TT dimers) but incorporates wrong bases
8. **Outcome**:
   - Cell survives replication (normally would stall & die)
   - Cost: increased mutation rate (mutations are not fatal in short term)
   - Adaptive because: transient burst of mutagenesis allows survival; upon repair, SOS shuts off

---

## Summary of Learning Objectives Revisited

By completing this lesson, you should now:

✓ **Explain mutations** — types, rates, spontaneous vs. induced, Luria-Delbrück test
✓ **Describe DNA repair** — MMR (Dam methylation, MutH), NER (dual incision), BER (glycosylases), DSB (RecBCD, RecA, RuvAB/C), SOS response
✓ **Understand recombination** — Holliday junctions, branch migration, gene conversion, RuvC resolution
✓ **Apply mapping** — recombination frequency, Hfr interrupted mating, time of entry mapping
✓ **Explain horizontal gene transfer** — transformation, generalized/specialized transduction, conjugation, F+, Hfr, F'
✓ **Use molecular techniques** — restriction enzymes, PCR, Sanger sequencing, restriction mapping

---

## Next Steps & Resources

**For Reinforcement**:
1. Review concept files in [[01_Concepts/MCDB 101A/]] — specialized deep-dives on each topic
2. Practice problems: [[05_Practice_Exams/MCDB 101A/Final]]
3. Related pathway notes: [[02_Pathways/]] for visual representations

**For Exam Preparation**:
1. Focus on high-yield topics (Module 6.2)
2. Redo any problems you missed
3. Be ready to explain mechanisms step-by-step (not just memorize)
4. Understand the "why" behind each repair pathway choice

**Wikilink Connections**:
- [[04_Course_Notes/MCDB 101A/Mutations]] — detailed mutation biology
- [[DNA Repair Pathways]] — comprehensive repair system overview
- [[04_Course_Notes/MCDB 101A/Recombination]] — homologous recombination mechanisms
- [[Gene Transfer]] — bacterial horizontal gene transfer
- [[Molecular Techniques]] — practical lab methods
- [[04_Course_Notes/MCDB 101A/Transcriptional Regulation]] — backlink to Midterm 2 content (needed context)
- [[Lac Operon]] — important for understanding regulation (Midterm 2)

---

**File Location**: `/sessions/practical-happy-hopper/mnt/Obsidian Vault/04_Course_Notes/MCDB 101A/Final Exam Comprehensive Lesson.md`

**Source**: NotebookLM Genetics AI Tutor (ID: 0211f2a5-00e1-4cfd-ba2a-10dfead80259) + Claude Biology Learning Engine
