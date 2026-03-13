# Light Reactions — Z-Scheme Pathway

**Course:** [[Course Dashboard]] | **Yield:** HIGH ⭐⭐⭐

---

## Pathway Overview

The Z-scheme traces the flow of electrons from water through two photosystems to produce NADPH, with ATP synthesized along the way via chemiosmosis. It takes place in the **thylakoid membranes** of chloroplasts.

---

## Step-by-Step Pathway

```
LIGHT
  ↓
H₂O ──[OEC]──→ 2H⁺ + ½O₂ + 2e⁻
                      ↓
              PSII (P680) ──excited──→ e⁻ ──→ Pheophytin
                                                    ↓
                                              Plastoquinone (PQ)
                                                    ↓
                                          Cyt b6f complex ──→ pumps H⁺ into lumen
                                                    ↓
                                            Plastocyanin (PC)
                                                    ↓
LIGHT                                       PSI (P700) ──excited──→ e⁻ ──→ A₀ → A₁ → FeSx
  ↓                                                                               ↓
  └────────────────────────────────────────────────────────────────────→ Ferredoxin (Fd)
                                                                                  ↓
                                                                      FNR (Ferredoxin-NADP⁺ reductase)
                                                                                  ↓
                                                                    NADP⁺ + H⁺ → NADPH

H⁺ GRADIENT (lumen high) ──→ ATP Synthase (CF₀CF₁) ──→ ADP + Pᵢ → ATP
```

---

## Key Components

| Component | Location | Function |
|-----------|----------|----------|
| OEC (Oxygen Evolving Complex) | PSII lumenal side | Splits H₂O → O₂ + H⁺ + e⁻; contains Mn cluster |
| P680 | PSII reaction center | Absorbs 680 nm photons; strongest known biological oxidant when oxidized |
| Pheophytin | PSII | First electron acceptor; chlorophyll without Mg²⁺ |
| Plastoquinone (PQ) | Mobile; thylakoid membrane | Carries 2e⁻ + 2H⁺; connects PSII to Cyt b6f |
| Cytochrome b6f | Thylakoid membrane | Proton pump; 4H⁺ per 2e⁻; analogous to Complex III in mitochondria |
| Plastocyanin (PC) | Lumen | Mobile Cu²⁺ protein; connects Cyt b6f to PSI |
| P700 | PSI reaction center | Absorbs 700 nm photons |
| Ferredoxin (Fd) | Stromal side | Transfers e⁻ to FNR |
| FNR | Stroma | Reduces NADP⁺ → NADPH |
| ATP synthase | Thylakoid membrane | H⁺ flow drives ATP synthesis |

---

## Energy Accounting (per 2 electrons, noncyclic)

| Product | Amount |
|---------|--------|
| O₂ released | ½ O₂ |
| NADPH produced | 1 |
| ATP produced | ~1.5 |

**To run Calvin cycle 3 times (fix 3 CO₂ → net 1 G3P):** need 9 ATP + 6 NADPH

---

## Cyclic vs. Noncyclic

| Mode | Electron source | Products |
|------|----------------|---------|
| Noncyclic (linear) | H₂O | O₂ + NADPH + ATP |
| Cyclic | PSI (electrons return via Fd → Cyt b6f) | ATP only (no NADPH, no O₂) |

---

## Related Concepts

- [[Light Reactions and Z-Scheme]]
- [[Calvin Cycle]]
- [[Photosynthesis]]
- [[C4 and CAM Photosynthesis]]
