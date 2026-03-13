# Pathway: Calvin Cycle (Dark Reactions)

**Type:** Biochemical cycle | **System:** Photosynthesis | **Module:** [[Photosynthesis]]

---

## Full Pathway

```
INPUTS: CO₂ (from air), ATP (from light reactions), NADPH (from light reactions)

STAGE 1: CARBON FIXATION
       ↓
CO₂ + RuBP (5C) ──[RuBisCo]──▶ 2× 3-PGA (3C)
                                  (3-phosphoglycerate)

STAGE 2: REDUCTION
       ↓
3-PGA + ATP + NADPH ──▶ G3P (3C)
                         (glyceraldehyde-3-phosphate)
                         ← Building block for glucose, sucrose, starch

STAGE 3: REGENERATION OF RuBP
       ↓
G3P + ATP ──▶ RuBP (5C)
             ← CO₂ acceptor regenerated; cycle continues

NET RESULT: For every 3 CO₂ fixed → 1 net G3P exported
```

---

## Connections to Light Reactions

```
LIGHT REACTIONS (thylakoids)
       |
       ├── ATP ──────────────────────────────▶ Stage 2 + Stage 3 of Calvin
       └── NADPH ────────────────────────────▶ Stage 2 of Calvin

CALVIN CYCLE (stroma)
       |
       └── G3P ──▶ sucrose (for phloem) / starch (for storage)
```

---

## Why C4 and CAM Exist

```
Normal conditions: CO₂ enters via stomata → RuBisCo fixes CO₂ ✓

HOT/DRY conditions:
       ↓
Stomata CLOSE to prevent water loss
       ↓
CO₂ drops; O₂ rises inside leaf
       ↓
RuBisCo grabs O₂ instead of CO₂ → PHOTORESPIRATION (wastes ATP, releases CO₂)
       ↓
C4 solution: Pre-fix CO₂ in mesophyll as oxaloacetate (4C)
             Transport to bundle sheath cells
             Release CO₂ near RuBisCo (high local [CO₂])
             → spatial separation

CAM solution: Fix CO₂ at NIGHT (stomata open) into 4C acids
              Store in vacuole
              Release CO₂ to RuBisCo during DAY (stomata closed)
              → temporal separation
```

---

## Exam Checkpoints ✅

- [ ] Stage 1 = Fixation (CO₂ + RuBP → 3-PGA by RuBisCo)
- [ ] Stage 2 = Reduction (3-PGA → G3P uses ATP + NADPH)
- [ ] Stage 3 = Regeneration (G3P → RuBP uses ATP)
- [ ] C4 = spatial separation (two cell types)
- [ ] CAM = temporal separation (night vs. day)
- [ ] Dark reactions still require LIGHT (indirectly — need ATP and NADPH from light reactions)
