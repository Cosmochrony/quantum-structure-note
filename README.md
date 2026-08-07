This repository contains the source of the **Quantum Structure Presentation Note** Cosmochrony paper
*The Quantum Structure Sub-Programme — Presentation Note 7*.

This work is a **structured entry point** to the quantum structure sub-programme of the
Cosmochrony corpus. It records the current, narrow scope of each constituent paper — what is
proved, what is conditional on an explicitly stated hypothesis, and what remains open — rather
than presenting a derivation chain.

## Current Status

The admissibility axioms A1--A4 force the fibre $F_n \simeq V_\rho$ with Heisenberg structure
(Note~5) and the admissibility thread $Q_8 \subset 2I \subset \mathrm{SU}(2)$ with the
spin-$\tfrac{1}{2}$ sector identified as the physically admissible sector (Note~1). $V_\rho$
already carries the complex $\mathrm{SU}(2)$ amplitude structure of the Weil representation,
supplied by O18 and O23, not derived from A1--A4.

> Given that supplied carrier, do the structures of quantum mechanics built upon it ---
> phase coherence, Born rule, singlet correlator, Bell-type correlations --- follow from
> admissibility alone, or must they be separately postulated?

That derivation is **not established**. Q1's proved theorem is a representation-theoretic
rigidity and no-go result, unrelated to phase coherence or the Born rule. Q2 proves only a
finite Laplacian-eigenvalue coincidence on $2I$. Q3 proves a theorem conditional on an explicit,
undemonstrated invariance hypothesis, not derived from admissibility or from Born–Infeld
indiscernibility. No result in this sub-programme derives phase coherence, a singlet correlator,
a Tsirelson bound, the Born rule, or a physically preferred sector from the admissibility axioms
alone. The Bell paper's claimed implication from non-injectivity to failure of Bell
factorisation is false: a finite Bell-local countermodel has non-injective observable maps,
and the paper's PR-box construction has empty support.

## Constituent Papers

| # | Paper | Central result | Status | Local path |
|---|-------|-----------------|--------|------------|
| 1 | **Q1** (Beau2026q1) — *Fourier-Support Rigidity in Conjugate Weil Sectors* | Exact rigidity theorem + no-go corollary; no phase coherence, correlator, Tsirelson bound, or Born rule | Proved | [`../q1/`](../q1/README.md) |
| 2 | **Q2** (Beau2026q2) — *An Exact Laplacian-Eigenvalue Degeneracy on $2I$* | $\lambda_{1/2}=\lambda_{3/2}=18$; no Casimir/isotropy, Born rule, Tsirelson bound, or fixed point | Proved | [`../q2/`](../q2/README.md) |
| 3 | **Q3** (Beau2026q3) — *Diagonal $2I$-Invariance Selects the Universal Singlet* | Singlet + Casimir correlator, given an explicit, undemonstrated hypothesis (H-inv) | Conditional | [`../q3/`](../q3/README.md) |
| 4 | **Bell paper** (Beau2026b) — published in *Quantum Reports* (2026) | Claimed implication from non-injectivity to failure of Bell factorisation is disproved by a finite Bell-local countermodel; PR-box support is empty | Refuted | [Bell README](../../bell-paper/README.md) |
| 5 | **BellNoGo** (Beau2026BellNoGo) — *Non-Injective Observable Maps Do Not Explain Bell Violations* | Redundant-extension and universal-pushforward theorems; correct obstruction identified as cross-context global-coupling absence (Fine's theorem) | Proved | [`../bell-noninjectivity-no-go/`](../bell-noninjectivity-no-go/README.md) |

## Status of Results

**Proved (unconditional):**
- Fourier-support rigidity theorem and no-go corollary (Q1).
- $1{,}548$ exact integer-arithmetic checks across six primes, zero failures, plus a negative
  control (Q1, numerical).
- Laplacian-eigenvalue degeneracy $\lambda_{1/2} = \lambda_{3/2} = 18$ on $2I$ (Q2).
- Non-injectivity has no Bell-discriminating power: redundant-extension and
  universal-pushforward theorems, output-entropy refutation, and identification of cross-context
  global-coupling absence as the correct obstruction (BellNoGo).

**Conditional (on Q3's explicit, undemonstrated hypothesis (H-inv)):**
- Unique invariant singlet $|\Omega_j\rangle$ for all five admissible sectors (Q3).
- Casimir correlator $E(\hat{a},\hat{b}) = -\tfrac{j(j+1)}{3}(\hat{a}\cdot\hat{b})$ (Q3).

**Open:**
- Phase coherence of the supplied Weil carrier, from the admissibility axioms.
- Q3's invariance hypothesis (H-inv) itself.
- The Born rule, in the $\mathrm{SU}(2)$ sector or beyond it.
- A setting-independent global-coupling obstruction sufficient for Bell non-factorisability;
  bare non-injectivity is not sufficient.
- A Tsirelson-type bound.
- Any sector-selection or fixed-point argument.
- Multipartite entanglement mixing the spin-$\tfrac12$ and spin-$\tfrac32$ sectors.

## Compilation

```bash
bash compile.sh
```

Produces `out/QuantumStructureNote.pdf`.

## Citation

> J. Beau, *The Quantum Structure Sub-Programme — Presentation Note 7*, Zenodo, 2026.
> DOI: [10.5281/zenodo.20562949](https://doi.org/10.5281/zenodo.20562949).
