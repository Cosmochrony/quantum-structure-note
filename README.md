This repository contains the source of the **Quantum Structure Presentation Note** Cosmochrony paper
*The Quantum Structure Sub-Programme — Presentation Note 7*.

This work is a **structured entry point** to the quantum structure sub-programme of the
Cosmochrony corpus, not a summary of results. It maps the constituent papers, identifies
the logical chain from admissibility to the Born rule, records the status of every result
as proved, numerical, or open, and states the remaining open deliverables.

## Central Question

The admissibility axioms A1--A4 force the fibre $F_n \simeq V_\rho$ with Heisenberg structure
(Note~5) and the admissibility thread $Q_8 \subset 2I \subset \mathrm{SU}(2)$ with the
spin-$\tfrac{1}{2}$ sector identified as the physically admissible sector (Note~1). $V_\rho$
already carries the complex $\mathrm{SU}(2)$ amplitude structure of the Weil representation,
supplied by O18 and O23, not derived from A1--A4.

> Given that supplied carrier, do the structures of quantum mechanics built upon it ---
> phase coherence, Born rule, singlet correlator, Bell-type correlations --- follow from
> admissibility alone, or must they be separately postulated?

The sub-programme answers: **conditional on the supplied carrier, they follow**. Phase
coherence of that carrier, the singlet correlator $E(\hat{a},\hat{b}) = -\hat{a}\cdot\hat{b}$,
the Tsirelson bound $|S_{\mathrm{CHSH}}| \leq 2\sqrt{2}$, and the Born rule are derived within
the $\mathrm{SU}(2)$ sector without importing any further quantum postulate; the carrier's own
complex scalar structure is not derived. $\mathrm{SU}(2)$ is identified as the unique
stable fixed point of the admissibility flow, and all results extend to the universal spin-$j$
case for the five admissible sectors of $2I$. Bell factorizability does not apply in
non-injective effective descriptions.

This sub-programme is the *first physics* of the corpus: before spacetime geometry, before
gauge structure, before gravity, the admissibility constraints already force quantum
correlations upon the supplied complex Weil carrier.

## Logical Chain

$$\underbrace{F_n \simeq V_\rho,\;\text{BI indisc.}}_{\text{A1--A4, O18}}
\;\Longrightarrow\;
\underbrace{\text{phase coherence}}_{\text{Q1 Thm 2.7}}
\;\Longrightarrow\;
\underbrace{E(\hat{a},\hat{b}) = -\hat{a}\cdot\hat{b}}_{\text{Q1 Thm 2.14}}
\;\Longrightarrow\;
\underbrace{|S_{\mathrm{CHSH}}| \leq 2\sqrt{2}}_{\text{Q1 Cor 2.16}}
\;\Longrightarrow\;
\underbrace{\text{Born rule}}_{\text{Q1 Thm 2.18}}$$

$$\Longrightarrow\;
\underbrace{\mathrm{SU}(2) \text{ fixed point}}_{\text{Q2 Thm 8.6}}
\;\Longrightarrow\;
\underbrace{E = -\tfrac{j(j+1)}{3}\hat{a}\cdot\hat{b},\;\text{all }j}_{\text{Q3 Thm 5.2}}$$

Six conceptually distinct steps:

1. **Phase coherence from BI indiscernibility** (Q1) — any admissible transition preserves
   the BI indiscernibility of conjugate Weil blocks $\rho_c$ and $\rho_{q-c}$; otherwise the
   rank of the Gram--Schmidt span inflates beyond the admissible bound of O22.
2. **Singlet correlator from four structural inputs** (Q1) — bilinearity from the carrier's
   preserved coherence, linearity of $\mathfrak{su}(2)$ observables (O23), rotation invariance
   from isotropic saturation (O23), and unit normalisation from the parity involution (O18)
   force $E(\hat{a},\hat{b}) = -\hat{a}\cdot\hat{b}$, conditional on the supplied carrier.
3. **Tsirelson bound as corollary** (Q1) — Cauchy--Schwarz on the derived correlator gives
   $|S_{\mathrm{CHSH}}| \leq 2\sqrt{2}$ unconditionally.
4. **Born rule from structural uniqueness** (Q1) — the unique probability assignment
   compatible with positivity, normalisation, linearity, and the derived correlator is
   $P(a=+1|\hat{a}) = |\langle +\hat{a}|\psi\rangle|^2$; no Gleason theorem is needed.
5. **$\mathrm{SU}(2)$ as stable fixed point** (Q2) — co-admissibility
   $\lambda_{1/2} = \lambda_{3/2} = 18$ on $2I$; the admissibility flow under spectral
   refinement in the LPS limit selects $j = \tfrac{1}{2}$ as the unique stable sector.
6. **Universal spin-$j$ generalisation** (Q3) — for all five admissible sectors
   $j \in \{\tfrac{1}{2}, 1, \tfrac{3}{2}, 2, \tfrac{5}{2}\}$: proto-state is the singlet
   $|\Omega_j\rangle$ (Schur on Clebsch--Gordan), universal correlator
   $E = -\tfrac{j(j+1)}{3}(\hat{a}\cdot\hat{b})$, sectorwise Born rule.

## Constituent Papers

| # | Paper | Stage | Local path |
|---|-------|-------|------------|
| 1 | **Q1** (Beau2026q1) — *Phase coherence and the spin-$\tfrac{1}{2}$ quantum sector* | Phase coherence, singlet correlator, Tsirelson, Born rule at $j=\tfrac{1}{2}$ | [`../q1/`](../q1/README.md) |
| 2 | **Q2** (Beau2026q2) — *Co-admissibility and $\mathrm{SU}(2)$ as stable fixed point* | Co-admissibility $\lambda_{1/2} = \lambda_{3/2}$, fixed-point selection | [`../q2/`](../q2/README.md) |
| 3 | **Q3** (Beau2026q3) — *Universal spin-$j$ quantum sector* | Proto-state, universal correlator, Born rule for all admissible $j$ | [`../q3/`](../q3/README.md) |
| 4 | **Bell paper** (Beau2026b) — *Bell non-applicability in non-injective frameworks* (published, *Quantum Reports* 2026) | Structural non-applicability of Bell factorizability | [`../../bell-paper/`](../../bell-paper/README.md) |

## Status of Results

**Proved (unconditional on admissibility; phase coherence, correlator, Tsirelson bound, and
Born rule are further conditional on the complex Weil carrier supplied by O18/O23, whose own
complex scalar structure is not derived):**
- Phase coherence from BI indiscernibility (Q1 Theorem 2.7).
- Observable rank signature $\mathrm{rank}\,W^{(c)}_n = 0$ as a falsifiable coherence
  witness (Q1 Corollary 2.9).
- Singlet correlator $E(\hat{a},\hat{b}) = -\hat{a}\cdot\hat{b}$ at spin-$\tfrac{1}{2}$
  (Q1 Theorem 2.14).
- Tsirelson bound $|S_{\mathrm{CHSH}}| \leq 2\sqrt{2}$ (Q1 Corollary 2.16).
- Born rule at spin-$\tfrac{1}{2}$ (Q1 Theorem 2.18).
- Co-admissibility $\lambda_{1/2} = \lambda_{3/2} = 18$ on $2I$ (Q2).
- $\mathrm{SU}(2)$ as unique stable fixed point of the admissibility flow (Q2 Theorem 8.6).
- Proto-state is the singlet for all admissible $j$ (Q3 Theorem 4.1).
- Universal correlator $E = -\tfrac{j(j+1)}{3}(\hat{a}\cdot\hat{b})$ (Q3 Theorem 5.2).
- Born rule for all five admissible $j$ (Q3 Corollary 6.1).
- Bell factorizability non-applicable in non-injective frameworks (Bell paper, published).

**Numerical:**
- $\mathrm{rank}\,W^{(c)}_n = 0$ confirmed for $q = 29$ across all four conjugate pairs
  throughout the admissible regime. Extension to
  $q \in \{61, 101, 151, 211, 307, 401\}$ identified as a validation target.

## Open Deliverables

1. **Born rule for general observables** — the $\mathrm{SU}(2)$ case is complete; the
   general case requires either an extension of the parity-sector argument to arbitrary
   fibre structures, or a direct Gleason-type theorem for the admissible measure on $V_\rho$.
2. **Numerical validation across the full prime range** — systematic verification of the
   rank-$W^{(c)}_n = 0$ signature for $q \in \{29, 61, 101, 151, 211, 307, 401\}$ would
   provide comprehensive empirical confirmation and track the boundary transition as a
   function of $q$.

## Compilation

```bash
bash compile.sh
```

Produces `out/QuantumStructureNote.pdf`.

## Citation

> J. Beau, *The Quantum Structure Sub-Programme — Presentation Note 7*, Zenodo, 2026.
> DOI: [10.5281/zenodo.20562949](https://doi.org/10.5281/zenodo.20562949).
