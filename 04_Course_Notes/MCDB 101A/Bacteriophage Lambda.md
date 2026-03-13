# Bacteriophage Lambda

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## 🎯 Learning Objectives

1. Describe the two lifecycle options of λ phage and the molecular factors that determine the choice
2. Explain the roles of cI, Cro, and N protein in the lysis/lysogeny switch
3. Describe the λ promoter architecture and how cI and Cro bind OR
4. Explain how cI maintenance (lysogeny) is self-reinforcing
5. Explain how UV irradiation induces the lytic cycle from a lysogen

---

## 🧠 Core Concepts

### λ Phage Overview

**Two Lifecycle Fates**

| Fate | Condition | Outcome |
|------|---------|---------|
| **Lysogeny** | Low MOI, slow growing cells, low proteases | λ DNA integrates into host chromosome; cI repressor silences lytic genes; prophage replicates with host |
| **Lytic** | High MOI, rapid host growth, DNA damage | Phage DNA replicates; structural proteins made; cell lyses; ~100 new phages released |

**Phage Genome Features**

- ~48.5 kb linear dsDNA; cohesive (cos) ends allow circularization after injection
- Integrates at **attB** site (bacterial) × **attP** (phage) → attL + attR flanking prophage
- Integration catalyzed by **λ Integrase (Int)** + **IHF**

### Key Regulatory Proteins

| Protein | Gene | Function | Binding |
|---------|------|---------|---------|
| **cI (λ repressor)** | cI | Represses lytic genes; maintains lysogeny | OR1 > OR2 > OR3; OL |
| **Cro** | cro | Represses lysogenic genes; promotes lysis | OR3 > OR2 > OR1 (opposite of cI) |
| **N** | N | Antiterminator; allows early gene transcription | nut sites (with Nus proteins) |
| **Q** | Q | Antiterminator; allows late gene transcription | qut site |
| **cII** | cII | Activates PRE promoter; stabilized by cIII | Activates cI and int transcription |
| **cIII** | cIII | Protects cII from host proteases (HflB/FtsH) |  |

### OR Region — The Genetic Switch

**Architecture**

The right operator (OR) contains three 17-bp operator sites:

```
←PRM    PR→
  OR3  OR2  OR1  (right to left: OR1 closest to PR)
```

| Site | Preferred by | Effect when bound |
|------|-------------|------------------|
| OR1 | cI first | Represses PR (blocks Cro and lytic genes) |
| OR2 | cI second | Represses PR; cI at OR2 also **activates PRM** (positive autoregulation) |
| OR3 | Cro first | Represses PRM (blocks cI transcription) |

**cI Binding Behavior**

- cI binds cooperatively: OR1 binding promotes OR2 binding
- OR1+OR2 bound by cI → PR repressed; PRM activated → **stable lysogeny**
- If cI falls below threshold → PR derepressed → Cro made → Cro binds OR3 → PRM repressed → irreversible shift to lysis

**Cro Binding Behavior**

- Cro binds OR3 first, then OR2, then OR1
- OR3 bound → PRM repressed → no cI made
- Eventually OR1 bound → PR also repressed (autoregulation of lytic cycle)

### Promoter Architecture

| Promoter | Direction | Activated by | Repressed by | Products |
|---------|-----------|-------------|-------------|---------|
| **PL** | Leftward | — | cI | N, other leftward early genes |
| **PR** | Rightward | — | cI | Cro, cII, O, P (replication) |
| **PRM** | Rightward (maintenance) | cI at OR2 | Cro at OR3 | cI (maintenance transcript) |
| **PRE** | Rightward | cII | — | cI (establishment transcript, higher level) |
| **PI** | — | cII | — | Int (integration) |

**Key logic:**
- After infection, **cII** levels determine fate:
  - High cII (stressed cells, low HflB activity) → activate PRE → high cI → lysogeny
  - Low cII (rapidly growing cells, high HflB protease) → cI not established → lysis

### Establishment vs. Maintenance of Lysogeny

**Establishment (immediately after infection)**

1. N protein (antiterminator) allows early gene read-through from PL and PR
2. cII protein accumulates; activates PRE (establishment promoter)
3. High cI from PRE → binds OR1+OR2 → represses PR → silences lytic genes
4. Int protein (made from PI) integrates λ DNA at attB × attP

**Maintenance (stable lysogen)**

1. Once OR1+OR2 are occupied by cI → PRM is activated
2. Low-level cI made from PRM → replenishes any degraded repressor
3. Self-reinforcing loop: cI maintains its own expression by activating PRM

### Induction — From Lysogen to Lytic

**Trigger: SOS Response (UV irradiation)**

1. UV creates DNA damage → RecA is activated as a coprotease
2. Activated RecA stimulates autocleavage of cI LexA-like linker
3. cI repressor cleaved → dissociates from OR1, OR2
4. PR and PL derepressed → lytic cycle begins

**RecA** also cleaves LexA repressor (inducing SOS genes) — parallel systems.

### OR Logic Summary

| [cI] | OR occupancy | PRM | PR | Outcome |
|------|-------------|-----|-----|---------|
| High | OR1+OR2+OR3 | OFF | OFF | Unstable lysogeny (too much repressor) |
| Moderate | OR1+OR2 | **ON** | OFF | **Stable lysogeny** |
| Low | None or only OR1 | OFF | ON | Cro made → lysis |

---

## ⚠️ Exam Traps

- ❌ **"cI simply turns off all λ genes"** — cI represses PR and PL but **activates** PRM by binding OR2.
- ❌ **"Cro is a repressor of lytic genes"** — Cro primarily represses **PRM** (lysogenic maintenance), promoting lysis.
- ❌ **"UV light directly destroys cI"** — UV causes DNA damage → RecA activation → cI autocleavage; UV doesn't directly attack the protein.

---

## Practice Questions

1. A mutation prevents cI from binding OR2 but not OR1. Predict the effect on: (a) repression of the lytic cycle, (b) maintenance of lysogeny. Explain using the promoter architecture.

2. Why is Cro considered an "anti-repressor" rather than an activator in the context of λ lysogeny?

3. cII protein is rapidly degraded by the HflB protease in rapidly growing cells. Explain how this tips the decision toward lysis.

4. A λ lysogen is exposed to UV irradiation. Describe the sequence of molecular events leading to prophage induction, including the roles of RecA and cI.

5. What would happen if a cI mutation abolished the ability to dimerize? (Hint: consider cooperative binding to OR1+OR2)

---

## Related Concepts

- [[Bacteriophage Lambda]]
- [[Bacteriophage Lambda]]
- [[Bacteriophage Lambda]]
- [[Transcriptional Regulation]] — compare operon logic
- [[DNA Repair]] — SOS response activates during induction
- [[Recombination]] — λ integrase uses site-specific recombination
