# Luria-Delbrück Fluctuation Test

**Topic Area:** Mutation
**Lecture:** [[Mutations]]
**Exam:** Final
**Importance:** MEDIUM-HIGH YIELD ⭐⭐

---

## One-Line Definition
The Luria-Delbrück fluctuation test (1943) proved that bacterial mutations arise **spontaneously and randomly before selection**, not as adaptive responses to the environment — founding the field of bacterial genetics.

---

## The Experiment

**Setup:**
- Grow many small replicate cultures of T1-sensitive *E. coli* from identical starting inocula
- Also grow one large bulk culture
- Plate all cultures on T1 phage; count resistant colonies

**Two competing hypotheses:**

| Hypothesis | Prediction | Variance |
|-----------|-----------|---------|
| Adaptive mutation | Phage exposure induces resistance → similar results across cultures | **Low variance** |
| Spontaneous mutation | Mutations arise randomly before phage contact → early mutations expand into clones → **jackpot cultures** | **High variance** |

**Result:** High variance, jackpot cultures — **spontaneous mutation confirmed**.

---

## Poisson Distribution for Mutation Rate

Since mutations are rare events:
$$P(k) = \frac{e^{-\mu} \cdot \mu^k}{k!}$$

**P(0) method** (most reliable):
$$f_0 = e^{-\mu}$$
$$\mu = -\ln(f_0)$$
$$\text{mutation rate} = \frac{\mu}{N}$$

where f₀ = fraction of cultures with zero mutant colonies, N = cells per culture at plating.

### Worked Example
- 20 cultures, N = 2 × 10⁷ cells, 12 cultures have zero resistant colonies
- f₀ = 12/20 = 0.60
- μ = −ln(0.60) ≈ 0.511 mutations per culture
- Mutation rate ≈ 0.511 / (2 × 10⁷) ≈ **2.56 × 10⁻⁸ per cell per generation**

---

## Mutation Rate vs. Mutation Frequency

| Term | Definition | Why use |
|------|-----------|---------|
| **Mutation rate** (μ) | Probability of mutation per cell per generation | More accurate; derived from P(0) method |
| **Mutation frequency** | Total mutants / total cells | Less accurate — distorted by jackpots |

**From NLM:** "Mutation frequency is less accurate than mutation rate because frequencies are heavily skewed by early jackpot events."

---

## Double Mutations
Rate of two independent simultaneous mutations = **product of individual rates**:
$$\mu_{A \text{ and } B} = \mu_A \times \mu_B$$

Example: If μ(leu⁻) = 2 × 10⁻⁷ and μ(trp⁻) = 5 × 10⁻⁷, then μ(leu⁻ trp⁻) = 1 × 10⁻¹³.

---

## Common Exam Traps (from NLM)
- The Luria-Delbrück experiment did **not** prove all mutations are random — it proved at least phage resistance mutations are spontaneous
- **Mutation frequency ≠ mutation rate** — jackpot cultures inflate frequency
- When two equally likely mutations produce a phenotype, μ_single = √(μ_double)

---

## Connections
- [[DNA Repair Pathways]] — repair reduces spontaneous mutation rate
- [[Luria-Delbrück Fluctuation Test]]
- [[Mutations]] — classification of mutation types
- [[Mutations]]
