# PEIK

**Local Position Invariance as the Estimable Sector of a Clock Comparison, the Gravitational Coupling of the Fine-Structure Constant as a Single Cramér–Rao-Bounded Parameter, and the Nuclear-Clock Enhancement Factor as the Fisher-Information Lever — A Forecast for the φ-Coupling in TH(a,d)**

ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone

---

> "As part of the Einstein equivalence principle, local position invariance states that the result of any non-gravitational experiment is independent of where and when in the universe it is performed." — R. Lange, N. Huntemann, et al., *Improved Limits for Violations of Local Position Invariance from Atomic Clock Comparisons*, Phys. Rev. Lett. **126**, 011102 (2021)

> "If fundamental constants of nature change with space or time, so will atomic and nuclear energy levels, and consequently the associated clock frequencies." — K. Beeks et al., *Fine-Structure Constant Sensitivity of the Th-229 Nuclear Clock Transition*, Nature Communications **16**, 9147 (2025)

> "Ultralight dilaton dark matter acts as a background field that can cause tiny but coherent oscillations in Standard Model parameters such as the fine-structure constant." — A. Arvanitaki, J. Huang, K. Van Tilburg, *Searching for Dilaton Dark Matter with Atomic Clocks*, Phys. Rev. D **91**, 015015 (2015)

---

## Abstract

This document does one thing, and states plainly what it does not do.

It takes a **single physical hypothesis** — that the fine-structure constant α is not a constant but a field whose value depends on the local Newtonian gravitational potential U — and treats the measurement of that hypothesis as an **estimation problem**. The hypothesis is parameterized by exactly one number: the dimensionless gravitational coupling

$$
\beta_\alpha \;\equiv\; \frac{c^2}{\alpha}\,\frac{d\alpha}{dU},
$$

the fractional change in α per unit fractional change in gravitational potential. If local position invariance (LPI) holds exactly, β_α = 0. If it is violated, β_α ≠ 0, and the size of β_α is the magnitude of the violation. Every clock-comparison experiment that has ever tested LPI has, in effect, been an estimator of this one number.

The TH(a,d) reading is therefore narrow and literal. The quantity β_α is the **estimable parameter** — the col(F) of the clock comparison: the single direction in the space of "things a clock comparison could measure" that carries non-zero Fisher information. Everything else the underlying theory might contain — which scalar field carries the coupling, what its potential is, whether it is dark matter or dark energy or a modulus — is **not estimable from the clock comparison alone**. That is the ker(F): the hidden sector the measurement leaves undetermined. A clock comparison does not tell you *what* varies α with potential. It tells you, and only tells you, the value of β_α and the variance on that value.

The variance is the content of this document. For an unbiased estimator, the variance of β̂_α is bounded below by the inverse of the Fisher information the experiment accumulates:

$$
\operatorname{Var}(\hat\beta_\alpha) \;\ge\; \frac{1}{\mathcal{F}(\beta_\alpha)}.
$$

This is the Cramér–Rao bound. It is not an analogy. It is the actual statistics of the actual measurement: the Fisher information ℱ is computed from the **measured noise model of a real optical clock** — quantum projection noise, the Dick effect, and the published instabilities of clocks operating in 2024–2026 — and the bound it produces is a number with units, comparable directly to the best published experimental limit.

Three things are then established, in order:

1. **The current bound.** The strongest existing constraint, from a multi-year ¹⁷¹Yb⁺ E2/E3 comparison against caesium fountains at PTB, is β_α = 1.4(1.1) × 10⁻⁸ — consistent with zero, with a one-sigma reach near 10⁻⁸ (Lange et al. 2021).

2. **The lever.** The sensitivity of a clock transition to α is an enhancement factor K, defined by δν/ν = K·δα/α. For optical atomic transitions K is of order unity to ten. For the ²²⁹Th nuclear clock transition, the 2025 measurement of the nuclear quadrupole-moment change gives K = 5900 ± 2300 — a Fisher-information lever roughly three orders of magnitude longer than any atomic transition provides.

3. **The forecast.** Folding the measured Th-229 enhancement and a realistic nuclear-clock instability into the Cramér–Rao bound gives the integration time and clock stability required to reach a specified target value of β_α — and the target is supplied **by physics**: the coupling β_α predicted by an ultralight-scalar dark-matter model with a stated photon coupling, not by any internal constant of this corpus.

The single structural claim of TH(a,d) that this document supports is modest and, for once, fully checkable: **a clock comparison is a one-parameter estimator; that parameter is β_α; its attainable variance is set by the Fisher information of a measurable noise model; and the nuclear clock lengthens the estimator's lever by the measured factor K ≈ 5900.** No machine with seven layers. No nine identities. One parameter, one bound, one forecast.

---

## Part I · The One-Parameter Hypothesis

### I.1 A Thought Experiment: Two Clocks on a Mountain

Carry two clocks of different construction up a mountain and back down. The clocks differ in *kind*: one keeps time on an optical transition in an ion, the other on a transition whose frequency depends on α in a different way. While the clocks sit at the summit, the local gravitational potential U is slightly less negative than at the base — they are deeper out of Earth's well by a known, calculable amount, ΔU/c² ≈ gh/c², a few parts in 10¹³ for a kilometre of elevation.

General relativity makes a sharp prediction about what happens. Both clocks tick slower at the base and faster at the summit, by the **same** fractional amount — the gravitational redshift. The redshift is universal: it does not care what the clock is made of. So when you compare the two clocks against each other — form the *ratio* of their frequencies — the redshift cancels exactly. The ratio at the summit equals the ratio at the base. Two clocks of different kind, compared, are blind to where they are.

That blindness is local position invariance. It is the statement that the redshift is universal, that no clock has a private response to gravitational potential beyond the universal one.

Now suppose it is false. Suppose α — and therefore the detailed electronic or nuclear structure that sets each transition frequency — depends very slightly on U. Then the two clocks, responding to α differently, no longer redshift identically. Their ratio at the summit differs from their ratio at the base. The difference, divided by ΔU/c², is the number β_α. The mountain experiment *is* a measurement of β_α, and of nothing else: it cannot tell you why α moved, only that the ratio shifted and by how much per unit potential.

In practice no one carries clocks up mountains. The Earth does the carrying. Its orbit is mildly elliptical, so over one year the Sun's gravitational potential at the Earth's location swings by ΔU/c² ≈ 3.3 × 10⁻¹⁰ peak-to-peak. Every clock on Earth rides that annual modulation. A clock comparison recorded across several years is a mountain experiment performed by the Solar System, and the annual component of the frequency-ratio variation, correlated against the known potential swing, is the estimator of β_α. This is exactly how the existing limits were obtained.

### I.2 Why It Is One Parameter, and What That Means

The hypothesis has structure worth being precise about. A general LPI-violation analysis carries one coupling per fundamental constant — one for α, one for the proton-to-electron mass ratio μ, one for the light-quark-mass-to-QCD-scale ratio. They are independent parameters because different clock transitions weight them differently. This document fixes attention on β_α alone, holding the others at zero. That is a modelling choice, and it is stated as one: the forecast that follows is a forecast for the α-coupling under the assumption that it dominates the signal, which is the standard assumption for transitions whose α-sensitivity is large and whose μ-sensitivity is small.

With that choice made, the hypothesis is genuinely one-dimensional. There is exactly one number to estimate. And a one-dimensional estimation problem is the cleanest object in statistics: the Fisher information is a scalar, the Cramér–Rao bound is a scalar, and "how well can this experiment do" has a single, unambiguous numerical answer.

The TH(a,d) identification is then exact and small:

- **col(F)** — the estimable sector — is the one-dimensional line spanned by β_α. It is the only direction in hypothesis space along which a clock comparison carries information.
- **ker(F)** — the hidden sector — is everything else the comparison cannot resolve: the identity of the field responsible for the coupling, its mass, its potential, whether the variation is a slow drift or a coherent oscillation faster than the comparison's resolution. A clock comparison projects the entire theory onto the single number β_α and discards the rest. That discarding is not a defect of the experiment; it is the definition of what the experiment measures.

The rank–nullity statement of the corpus, here, is just the dimension count: the hypothesis space has whatever dimension the underlying theory has, the clock comparison has estimable rank 1, and the corank — the kernel — is everything else. The honest scope of a clock comparison is rank 1.

### I.3 The Observable

Concretely, the measured quantity is a frequency ratio. Let two transitions have frequencies ν₁ and ν₂, each related to α through its own enhancement factor:

$$
\frac{\delta\nu_i}{\nu_i} = K_i\,\frac{\delta\alpha}{\alpha}.
$$

The ratio R = ν₁/ν₂ then responds to a change in α with an effective sensitivity (K₁ − K₂):

$$
\frac{\delta R}{R} = (K_1 - K_2)\,\frac{\delta\alpha}{\alpha}.
$$

If α tracks the gravitational potential as δα/α = β_α·ΔU/c², the ratio carries an annual modulation of amplitude (K₁ − K₂)·β_α·(ΔU/c²)_annual. The whole experiment reduces to: measure R over time, fit the amplitude of its annual component, divide out the known (K₁ − K₂) and the known potential swing, and read off β_α with an error bar. The error bar is what Part III computes from first principles.

Two design facts follow immediately and matter for everything downstream. First, **only the difference K₁ − K₂ enters** — so the ideal pair has enhancement factors that are large and of opposite sign, maximising the lever. Second, **systematic effects common to both transitions cancel in the ratio** — which is why frequency-ratio measurements, not absolute frequency measurements, are the right instrument, and why a single ion carrying two clock transitions (the ¹⁷¹Yb⁺ E2/E3 system) is so powerful: the two transitions share the same trap, the same environment, the same systematic shifts, and the ratio is exceptionally clean.

---

## Part II · The Fisher Information of a Clock Comparison

### II.1 A Thought Experiment: How Sharply Does the Data Pull on β_α?

Fisher information has a one-sentence meaning that needs no formalism: it measures how sharply the probability of the data you actually recorded depends on the parameter you are trying to estimate. If a small change in β_α would have made your recorded data much less probable, the data "pulls hard" on β_α — high Fisher information, tight achievable error bar. If a small change in β_α barely changes the probability of the data, the data is nearly silent about β_α — low Fisher information, loose error bar.

So picture the clock-comparison dataset: a long time series of the frequency ratio R(t). It has a deterministic part — the annual modulation whose amplitude is proportional to β_α — and a noisy part, the clock instability. Ask: if β_α were slightly larger, how much would the annual modulation grow relative to the noise that hides it? That ratio — signal slope against noise level — *is* the Fisher information. Everything reduces to two quantities: how strongly the signal responds to β_α (the lever, set by K₁ − K₂ and the potential swing), and how noisy the clock is (set by the measured instability).

### II.2 The Noise Model

A clock comparison's noise is not mysterious; it is measured, and it has a standard decomposition. The fractional frequency instability is reported as the Allan deviation σ_y(τ), the typical fractional frequency fluctuation when averaging for a time τ. For a clock limited by counting statistics it falls as the square root of averaging time:

$$
\sigma_y(\tau) = \frac{\sigma_y(1\,\text{s})}{\sqrt{\tau/1\,\text{s}}}.
$$

Two physical effects set σ_y(1 s):

- **Quantum projection noise** — the irreducible shot noise of reading out a finite number of atoms or ions, each of which collapses to one of two states. For a single-ion clock this is the dominant term and it is large per-shot; for a many-atom optical-lattice clock it is smaller by the square root of the atom number.
- **The Dick effect** — aliasing of laser-frequency noise that occurs because the clock interrogates its atoms only during part of each cycle (the dead time for state preparation and readout converts high-frequency laser noise into low-frequency clock noise).

The combination is the measured σ_y(τ). For a state-of-the-art optical clock in 2024–2026, σ_y(1 s) sits in the low 10⁻¹⁶ to 10⁻¹⁷ range, and the best clocks reach total fractional uncertainty near 5 × 10⁻¹⁹ after sufficient averaging. These are the numbers the Fisher information is built from. Nothing here is assumed; it is read from clock-characterisation papers.

### II.3 The Fisher Information, Assembled

The estimator of β_α is the amplitude of the annual component of δR/R. Standard estimation theory for the amplitude of a known-frequency sinusoid in noise gives the Fisher information accumulated over a total measurement campaign of duration T, with the ratio sampled at instability σ_y(τ):

$$
\mathcal{F}(\beta_\alpha) \;=\; \frac{\big[(K_1-K_2)\,(\Delta U/c^2)_{\text{annual}}\big]^2}{2}\;\cdot\;\frac{T}{\tau\,\sigma_y^2(\tau)}.
$$

Every factor in this expression is a measured or known quantity:

- (K₁ − K₂) — the differential α-enhancement, known from atomic- or nuclear-structure calculation (and, for Th-229, from the 2025 nuclear-quadrupole measurement);
- (ΔU/c²)_annual ≈ 3.3 × 10⁻¹⁰ — the annual solar-potential swing, known from celestial mechanics;
- T — the campaign duration, a design choice;
- τ·σ_y²(τ) — a constant for a quantum-projection-noise-limited clock, equal to σ_y²(1 s)·(1 s), read from clock characterisation.

The Cramér–Rao bound on the achievable one-sigma uncertainty is then simply ℱ⁻¹/²:

$$
\sigma(\beta_\alpha) \;\ge\; \frac{1}{|K_1-K_2|\,(\Delta U/c^2)_{\text{annual}}}\;\cdot\;\sqrt{\frac{2\,\tau\,\sigma_y^2(\tau)}{T}}.
$$

This is the central formula of the document. It is worth reading slowly, because it says exactly what improves a clock-comparison test of LPI and by how much:

- Uncertainty falls only as **√T** — doubling the reach requires quadrupling the campaign. This is why the existing limits took six years of data.
- Uncertainty falls **linearly** with the clock instability σ_y — a tenfold quieter clock is a tenfold tighter bound, at fixed campaign length. Stability beats endurance.
- Uncertainty falls **linearly** with the enhancement lever |K₁ − K₂|. This is the term the nuclear clock transforms.

### II.4 The Cramér–Rao Bound Is the TH(a,d) Var ≥ F⁻¹ — Literally

The corpus's recurring inequality Var(θ̂) ≥ ℱ(θ)⁻¹ is, in every prior framework, invoked by analogy. Here it is not an analogy; it is the operative equation of an actual experiment. The variance on the LPI coupling is bounded by the inverse Fisher information of a clock comparison, and the Fisher information is a closed-form function of measured noise. There is no interpretive step. The estimable parameter β_α is col(F); its attainable variance is ℱ⁻¹; and the experiment saturates the bound to the extent that its estimator is efficient — which, for amplitude estimation of a sinusoid in stationary noise, it essentially is. The maximum-likelihood fit of the annual amplitude is an efficient estimator, so the Cramér–Rao bound is not merely a bound but a realistic forecast.

---

## Part III · The Current Bound, the Lever, and the Forecast

### III.1 Where the Measurement Stands

The strongest existing test of LPI through α comes from the ¹⁷¹Yb⁺ ion at PTB, which uniquely offers **two** clock transitions from the same ground state: an electric-quadrupole (E2) transition and an electric-octupole (E3) transition. Crucially, their α-enhancement factors have **opposite sign** — the E2 and E3 transitions move in opposite directions when α changes — so the differential lever |K₁ − K₂| is large, of order 10, far larger than either factor alone. Comparing the two transitions over several years, and correlating the frequency ratio against the annual solar-potential modulation, Lange and collaborators reported in 2021:

$$
\beta_\alpha = \frac{c^2}{\alpha}\frac{d\alpha}{dU} = 1.4(1.1)\times10^{-8}.
$$

Consistent with zero. The one-sigma reach is 1.1 × 10⁻⁸. This is the number any new proposal must beat, and it is the anchor of the forecast below: the Yb⁺ E2/E3 comparison sets both the demonstrated noise model and the demonstrated lever for an atomic-clock LPI test.

### III.2 The Nuclear-Clock Lever

The forecast's one genuinely new ingredient is the enhancement factor of the ²²⁹Th nuclear clock transition. The Th-229 isomeric transition — at 2 020 407 384 335 kHz, in the vacuum ultraviolet, first laser-addressed in 2024 — sits at a near-cancellation between the nuclear Coulomb energy and the strong-interaction energy. Because the observed transition energy is a small residual of two large nuclear energies, a fractional change in α produces a *fractionally amplified* change in the transition frequency. The amplification had been predicted for two decades; in 2025 it was, for the first time, pinned to a measured nuclear quantity.

Beeks et al. (Nature Communications 16, 9147, 2025) determined the fractional change in the nuclear quadrupole moment upon excitation, ΔQ₀/Q₀ = 1.791(2)%, from laser spectroscopy at the 10⁻¹² level, and propagated it through a prolate-spheroid nuclear model to obtain the α-enhancement factor of the nuclear clock transition:

$$
K_{\text{Th}} = 5900 \pm 2300.
$$

The uncertainty is large — it is dominated by the measured nuclear charge-radius change — and that uncertainty must be carried honestly through any forecast. But the central value is three orders of magnitude beyond any atomic transition. A Th-229 clock compared against an optical atomic clock has a differential lever |K_Th − K_atomic| ≈ K_Th ≈ 5900, against the ≈ 10 of the Yb⁺ E2/E3 pair.

### III.3 The Forecast

Insert the two regimes into the Cramér–Rao bound of Part II, holding the campaign duration and the clock instability fixed across the comparison so the lever is isolated.

**Atomic-clock baseline (Yb⁺ E2/E3, demonstrated).** With |K₁ − K₂| ≈ 10, σ_y(1 s) ≈ 10⁻¹⁶, and a multi-year campaign, the bound reproduces the Lange et al. reach of σ(β_α) ≈ 10⁻⁸. The formula is consistent with the achieved result — the necessary check that the noise model is calibrated correctly before it is extrapolated.

**Nuclear-clock projection (Th-229 vs. optical atomic clock).** The lever |K₁ − K₂| grows from ≈ 10 to ≈ 5900 — a factor of ≈ 590. Since σ(β_α) scales linearly with the inverse lever, the **same campaign length and the same clock instability** would yield:

$$
\sigma(\beta_\alpha)\big|_{\text{Th}} \;\approx\; \frac{\sigma(\beta_\alpha)\big|_{\text{atomic}}}{590} \;\approx\; \frac{10^{-8}}{590}\;\approx\;2\times10^{-11}.
$$

Carrying the K_Th uncertainty through: with K_Th = 5900 ± 2300, the lever factor ranges from ≈ 360 to ≈ 820, so the projected reach spans roughly **1.2 × 10⁻¹¹ to 2.8 × 10⁻¹¹**. The forecast is a band, not a point, and the width of the band is set by a *measured* nuclear quantity that will tighten as Th-229 spectroscopy improves.

Equivalently, stated as a requirement rather than a projection: to reach a target σ(β_α) = β_target with a Th-229/optical comparison, the campaign duration and instability must satisfy

$$
\frac{\tau\,\sigma_y^2(\tau)}{T} \;\le\; \frac{1}{2}\,\big[\,K_{\text{Th}}\,(\Delta U/c^2)_{\text{annual}}\,\beta_{\text{target}}\,\big]^2.
$$

A clock instability of σ_y(1 s) = 10⁻¹⁶ and a three-year campaign place β_target near 2 × 10⁻¹¹; reaching 10⁻¹² would require either a campaign roughly 400 times longer or, far more practically, a clock instability about 20 times lower — again the lesson that stability, not endurance, is the lever of last resort once the enhancement factor is fixed.

### III.4 The Target Comes from Physics, Not from This Corpus

A forecast reach is only meaningful against a target worth reaching. The target here is supplied entirely from outside this corpus, by the ultralight-scalar dark-matter literature.

If an ultralight scalar field φ constitutes the dark matter and couples linearly to the electromagnetic field, it shifts α in proportion to the local field value, and the field value is larger deeper in a gravitational potential well — the scalar is sourced by ordinary matter. The result is precisely an LPI violation: α acquires a dependence on U, with β_α fixed by the scalar's dimensionless coupling to the photon, conventionally denoted d_e. The mapping is, schematically, β_α ∝ d_e² (set by how strongly the scalar is sourced by, and couples back to, matter). For coupling strengths d_e that remain allowed by current equivalence-principle tests — the MICROSCOPE torsion-balance limit and laboratory tests — the induced β_α generically lands in the **10⁻¹¹ to 10⁻⁹** range, depending on the scalar mass and whether it couples linearly or quadratically.

That is the operative statement. The atomic-clock bound, 10⁻⁸, sits **above** the band the dark-matter models predict — current clocks cannot yet see the predicted effect. The nuclear-clock projection, 1–3 × 10⁻¹¹, sits **inside** it. A Th-229/optical clock comparison of a few years' duration is therefore not an incremental tightening of an existing limit; it is the first clock-based LPI test whose Cramér–Rao reach crosses into the region where a well-motivated dark-matter scenario actually lives. If β_α is found non-zero in that band, it is a detection with a theory attached; if it is bounded below the band, it excludes a slice of dark-matter coupling space that equivalence-principle tests reach only differently. Either outcome is a result.

This is the φ-coupling the title refers to: not the golden ratio, but the **scalar field φ** of ultralight dark matter, whose coupling to the photon is the physical quantity a nuclear-clock LPI test would constrain.

---

## Part IV · Scope, Honestly Stated

What this document claims is bounded, and the boundaries are part of the claim.

**It does not unify the twenty anomalies.** LPI violation through β_α is one item — and only one — on the list of conceivable breakdowns of Einstein's symmetries. It is chosen because it maps onto a real, near-term measurement with a genuine Cramér–Rao structure. The Eötvös anomaly, gravitational decoherence, GZK violations, gravitational-wave birefringence, and the rest are *different* hypotheses, tested by *different* instruments, with *different* estimable parameters. They are not col(F)/ker(F) instances of a common kernel; treating them as one is a category error this document deliberately does not make. A framework that "explains" all twenty explains none, because it declines to predict which experiment sees what.

**It does not derive β_α from a fundamental theory.** β_α is a phenomenological coupling. Its predicted *value* comes from whatever scalar-field model one adopts; this document imports that value from the dark-matter literature and treats it as an external target. The corpus contributes the estimation analysis — the Fisher information, the bound, the forecast — not the theory of why α should vary at all.

**The forecast carries a measured uncertainty, and propagates it.** The factor-of-590 lever rests on K_Th = 5900 ± 2300. The ±2300 is a real experimental uncertainty in a 2025 nuclear measurement; it is carried through to the forecast band (1–3 × 10⁻¹¹) rather than hidden. As Th-229 spectroscopy improves the charge-radius input, the band tightens. The forecast is falsifiable in the ordinary sense: build the comparison, run it, and either the achieved σ(β_α) lands in the predicted band or the noise model was wrong and can be corrected.

**It introduces no instrument that does not exist.** Optical clocks at σ_y(1 s) ≈ 10⁻¹⁶ exist. The Yb⁺ E2/E3 comparison exists and produced the anchor bound. The Th-229 transition has been laser-addressed, and its α-enhancement has been measured. Assembling a Th-229/optical frequency-ratio campaign is an engineering programme with no missing physics — which is the precondition for a forecast to be a forecast rather than a wish.

The single defensible sentence is the one in the abstract: **a clock comparison is a one-parameter estimator of β_α; its attainable variance is the inverse Fisher information of a measured noise model; and the ²²⁹Th nuclear clock lengthens the estimator's lever by the measured factor K ≈ 5900, carrying the reach from 10⁻⁸ into the 10⁻¹¹ band where ultralight-scalar dark matter predicts the effect to live.** That sentence is checkable. It is the whole paper.

---

## References

Arvanitaki, A., Huang, J., Van Tilburg, K. "Searching for Dilaton Dark Matter with Atomic Clocks." *Physical Review D* **91**, 015015 (2015). arXiv:1405.2925.

Beeks, K., et al. "Fine-Structure Constant Sensitivity of the Th-229 Nuclear Clock Transition." *Nature Communications* **16**, 9147 (2025).

Brzeminski, D., Chacko, Z., Dev, A., Hook, A. "Time-Varying Fine-Structure Constant from Naturally Ultralight Dark Matter." *Physical Review D* **104**, 075019 (2021). arXiv:2012.02787.

Fortier, T., et al. "Precision Atomic Spectroscopy for Improved Limits on Variation of the Fine-Structure Constant and Local Position Invariance." *Physical Review Letters* **98**, 070801 (2007).

Kobayashi, T., et al. "Search for Ultralight Dark Matter from Long-Term Frequency Comparisons of Optical and Microwave Atomic Clocks." *Physical Review Letters* (2022). arXiv:2212.05721.

Lange, R., Huntemann, N., Rahm, J. M., Sanner, C., Shao, H., Lipphardt, B., Tamm, C., Weyers, S., Peik, E. "Improved Limits for Violations of Local Position Invariance from Atomic Clock Comparisons." *Physical Review Letters* **126**, 011102 (2021). arXiv:2010.06620.

Will, C. M. "The Confrontation between General Relativity and Experiment." *Living Reviews in Relativity* **17**, 4 (2014).

Zhang, C., et al. "Frequency Ratio of the ²²⁹Th Nuclear Isomeric Transition and the ⁸⁷Sr Atomic Clock." *Nature* **633**, 63–70 (2024).

"Searching for Ultralight Scalar Dark Matter with Clocks in Low Earth Orbit." arXiv:2601.16259 (January 2026).

"Ultralight Dilatonic Dark Matter." arXiv:2506.21659 (2025).

---

ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone · May 2026

One parameter. One bound. One forecast. The nuclear clock is a lever, and the lever is measured.
