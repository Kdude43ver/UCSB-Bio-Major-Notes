# Bacteriophage Lambda (λ)

**Topic Area:** Gene Regulation / Phage Biology
**Lecture:** [[Bacteriophage Lambda]]
**Exam:** Midterm 2
**Importance:** HIGH YIELD ⭐⭐⭐

---

## One-Line Definition
Bacteriophage λ is a temperate phage that chooses between **lysis** (replication and cell death) and **lysogeny** (integration and dormancy) via a genetic switch governed by competition between the cI repressor and Cro protein.

---

## The Switch: cI vs. Cro

| Protein | Binds OR sites in order | Effect |
|---------|------------------------|--------|
| **cI** (repressor) | OR1 > OR2 > OR3 | Represses PR/PL; **activates PRM** (autoregulation) → lysogeny |
| **Cro** | OR3 > OR2 > OR1 | Represses **PRM** → prevents cI maintenance → lysis |

### Promoter Logic
| Promoter | What it makes | Repressed by | Activated by |
|---------|--------------|-------------|-------------|
| PR | Cro, replication proteins | cI (at OR1) | Default |
| PL | N, other early genes | cI | Default |
| **PRM** | cI (maintenance) | Cro (at OR3) | cI (at OR2) |
| PRE | cI (establishment, high) | — | cII |

---

## Decision: Lysis vs. Lysogeny

**cII protein is the key arbiter:**
- **High cII** (slow-growing cells, low HflB protease) → activates PRE → high cI → cI fills OR1+OR2 → lysogeny
- **Low cII** (fast-growing cells, high HflB) → insufficient cI → PR active → Cro made → Cro fills OR3 → PRM off → lysis

---

## Lysogeny Maintenance
- Moderate cI occupies OR1+OR2: PR repressed, PRM activated (positive autoregulation)
- Self-reinforcing loop maintains low-level cI expression indefinitely

## Induction (SOS Response)
UV → DNA damage → RecA activated as co-protease → cI autocleavage → cI falls off OR → PR/PL derepressed → lytic cycle

---

## Analogy
The λ switch is like a bistable light switch: cI keeps the "lysogeny" state ON by holding its own switch up (positive autoregulation at OR2). DNA damage kicks the switch — RecA is the finger that flips it to lysis.

---

## Connections
- [[Transcriptional Regulation]] — compare Lac operon logic
- [[Recombination]] — λ integrase (site-specific recombination)
- [[DNA Repair]] — SOS induction triggers λ lytic cycle
- [[Bacteriophage Lambda]]
