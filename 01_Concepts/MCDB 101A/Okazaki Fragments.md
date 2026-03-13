# Okazaki Fragments

## Definition
Okazaki fragments are short, discontinuously synthesized DNA segments produced on the **lagging strand** during DNA replication. They are named after Reiji and Tsuneko Okazaki, who discovered them in the 1960s. Their existence solves the fundamental problem of how a polymerase that can only synthesize 5'→3' replicates a template running 3'→5' at the replication fork.

---

## The Antiparallel Problem

DNA is antiparallel: the two strands run in opposite directions. DNA polymerase can only add nucleotides to a 3'-OH end (5'→3' synthesis). At a replication fork moving in one direction:

- **Leading strand**: Template runs 3'→5' relative to fork movement → synthesized **continuously** 5'→3' toward the fork
- **Lagging strand**: Template runs 5'→3' relative to fork movement → must be synthesized **discontinuously** in short fragments moving **away** from the fork

---

## Synthesis of Okazaki Fragments (Bacteria)

### Step 1: Primer Synthesis
- **Primase (DnaG)** synthesizes a short **RNA primer** (~10–12 nt) on the lagging strand template
- Primase associates with the **DnaB helicase** at the replication fork
- A new primer must be synthesized for each Okazaki fragment

### Step 2: Extension
- **DNA Pol III holoenzyme** extends the RNA primer, synthesizing DNA 5'→3'
- Synthesis continues until it reaches the 5' end of the previous Okazaki fragment

### Step 3: Primer Removal
- **DNA Pol I** uses its **5'→3' exonuclease** activity to remove the RNA primer while simultaneously filling the gap with DNA (**nick translation**)
- This is the KEY role of DNA Pol I's 5'→3' exonuclease — unique among E. coli polymerases

### Step 4: Ligation
- **DNA ligase** seals the nick between the newly synthesized DNA and the adjacent Okazaki fragment
- Requires NAD⁺ (bacteria) or ATP (eukaryotes/phage) as cofactor

---

## Fragment Sizes

| Organism | Fragment Size | Primer Size |
|----------|--------------|-------------|
| Bacteria (E. coli) | 1,000–2,000 nt | ~10–12 nt RNA |
| Eukaryotes | 100–400 nt | ~10 nt RNA |

Eukaryotic fragments are shorter because of nucleosome interference and more complex regulation.

---

## Supporting Proteins

| Protein | Function |
|---------|----------|
| DnaB helicase | Unwinds double-stranded DNA at fork |
| SSB (Single-Strand Binding Protein) | Stabilizes single-stranded template; prevents secondary structures |
| DnaG (Primase) | Synthesizes RNA primers |
| DNA Pol III | Main replicative polymerase; extends primers |
| DNA Pol I | Removes primers (5'→3' exonuclease); fills gaps |
| DNA Ligase | Seals nicks between fragments |

---

## Leading vs. Lagging Strand Summary

| Feature | Leading Strand | Lagging Strand |
|---------|---------------|----------------|
| Template orientation | 3'→5' (toward fork) | 5'→3' (away from fork) |
| Synthesis direction | Toward fork | Away from fork |
| Continuity | Continuous | Discontinuous (Okazaki fragments) |
| Primers needed | One (at origin) | One per fragment |
| Pol I involvement | Minimal | Removes each primer |

---

## Key Exam Points
- **Only the lagging strand** makes Okazaki fragments; leading strand is synthesized continuously
- **DNA Pol I** removes RNA primers via its **5'→3' exonuclease** (not 3'→5' proofreading)
- **DNA Pol III** does the bulk extension of each fragment
- **DNA ligase** seals the final nick — without it, fragments remain separate
- SSB stabilizes the template; without SSB, hairpins form and block polymerase
- In bacteria, Okazaki fragments are 1–2 kb; eukaryotes ~100–400 nt
- **Primase is required** because DNA Pol III cannot start a new strand de novo

---

## Related Concepts
- [[DNA Replication]]
- [[DNA Repair Pathways]]
- [[Mutations]]

## Prerequisites
- DNA structure and antiparallel nature
- DNA polymerase properties
- Replication fork proteins

## Importance: HIGH YIELD
Primer removal by Pol I's 5'→3' exonuclease, the role of DNA ligase, and the distinction between leading/lagging strands are classic exam questions.
