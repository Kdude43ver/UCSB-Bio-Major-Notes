# Phototransduction Pathway

**Course:** [[Course Dashboard]] | **Yield:** MEDIUM ⭐⭐

---

## Pathway Overview

Phototransduction converts absorbed photons into a graded electrical signal in photoreceptor cells. The pathway in rod cells is a signal-amplifying G-protein cascade that causes hyperpolarization upon light exposure.

---

## Step-by-Step: Dark vs. Light

### DARK STATE (no photons)

```
11-cis retinal + opsin = Rhodopsin (inactive)
        ↓
cGMP phosphodiesterase (PDE) → INACTIVE
        ↓
[cGMP] HIGH in cytoplasm
        ↓
cGMP-gated channels OPEN
        ↓
Na⁺ and Ca²⁺ flow IN → DEPOLARIZED membrane (~−40 mV)
        ↓
Glutamate continuously released at synaptic terminal
```

### LIGHT STATE (photon absorbed)

```
PHOTON
        ↓
11-cis retinal → all-trans retinal (isomerization)
        ↓
Rhodopsin (R) → R* (activated metarhodopsin II)
        ↓
R* activates TRANSDUCIN (Gₜ, αβγ heterotrimer)
Gₜ-GDP + R* → Gₜ-GTP (α subunit released)
        ↓
Gₜ-α-GTP activates PHOSPHODIESTERASE (PDE)
        ↓
PDE hydrolyzes cGMP → 5'-GMP
        ↓
[cGMP] DROPS
        ↓
cGMP-gated channels CLOSE
        ↓
Na⁺/Ca²⁺ entry stops
        ↓
HYPERPOLARIZATION (membrane → ~−70 mV)
        ↓
Glutamate release STOPS (hyperpolarized terminal)
        ↓
Bipolar cell → responds → signal to retinal ganglion cell → optic nerve → brain
```

---

## Signal Amplification

- 1 photon activates ~1 rhodopsin
- 1 R* activates ~500 transducins
- 500 transducins activate 500 PDE enzymes
- Each PDE hydrolyzes ~1000 cGMP/sec
- **Result:** 1 photon → ~10⁶ cGMP hydrolyzed → large channel closure

---

## Recovery Mechanisms

| Step | Molecule | Action |
|------|----------|--------|
| Rhodopsin inactivation | Rhodopsin kinase → phosphorylates R* | Reduces transducin activation |
| | Arrestin binds phospho-R* | Fully blocks transducin |
| Transducin inactivation | Intrinsic GTPase (accelerated by RGS9) | GTP → GDP → Gₜ inactive |
| cGMP restoration | Guanylyl cyclase (activated by low Ca²⁺) | Resynthesizes cGMP |
| Retinal regeneration | RPE cells: retinal re-isomerized | 11-cis retinal returned to opsin |

---

## Related Concepts

- [[Phototransduction]]
- [[Sensory Systems]]
- [[Action Potential]]
- [[Nervous System]]
