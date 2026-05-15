# Finite-Memory Projection Corrections In Cosmological Consistency Diagnostics

Working manuscript draft. Current claim level: theory-method diagnostic.

## Abstract

We introduce a bounded finite-memory projection operator for diagnostic
cosmological consistency tests. The operator is formulated as an effective
projection response over normalized depth, $W(x)=1+\rho x^3$, with a passive
memory-budget bound $\rho \leq 4$. The construction is not presented as a complete
cosmological model or an observational detection. It is instead a disciplined
diagnostic module for comparing projected response shapes against
backreaction-aware distance consistency reconstructions. In a BAO-only
diagnostic reconstruction, the locked K2 window overlaps the full target
envelope. In an SN+BAO source-split stress test, strict median-sign matching
exhibits a localized tension; a reconstruction-aware sign-stability gate
resolves this tension without widening the K2 window. The result motivates a
future full-likelihood comparison while preserving explicit claim boundaries.

## 1. Introduction

Modern cosmological consistency tests increasingly distinguish background
expansion, light-propagation effects, curvature consistency, and cosmic
backreaction. A residual relative to a homogeneous FLRW reference model is
therefore not automatically evidence for new physics: it may arise from optical
sampling, reconstruction convention, averaging, or the choice of observable
combination.

Heinesen and Clifton recently emphasized that broad classes of cosmological
models can be separated by how they violate FLRW curvature-consistency tests
[1].
They isolate two especially relevant routes: deviations in optical properties
and deviations in large-scale expansion. This is naturally adjacent to the
older Dyer-Roeder optical-distance tradition, where light propagation through
clumpy matter distributions is treated separately from the homogeneous
background distance law [3,4]. Koksbang then applied this kind of
observable logic to constrain cosmic backreaction over an extended redshift
range, finding consistency with vanishing backreaction at one standard
deviation while also emphasizing that significant backreaction is not yet ruled
out [2]. These papers are useful here because they make the main methodological
lesson sharp: a projected cosmological residual must be tested against optical,
geometrical, and reconstruction degeneracies before it is interpreted.

This note develops a deliberately narrow finite-memory projection diagnostic
that can be placed alongside such tests. The objective is not to disclose or
validate a full underlying theory. Instead, we ask whether a predeclared,
bounded projection-memory operator can define a reproducible diagnostic window
and survive basic source-split stress tests.

The contribution is therefore threefold. First, we define a finite-memory
operator whose amplitude is bounded before comparison with reconstructed
diagnostics. Second, we give an explicit shape-selection rule that fixes the
cubic kernel from a small power-kernel family. Third, we state a sign-stability
policy for interpreting reconstructed diagnostic points whose median sign is
method-sensitive.

## 2. Minimal Effective Disclosure

Only the effective module needed for this note is used. We assume that an
observed consistency residual can be represented as a projected response over a
normalized depth coordinate,

$$
0 \leq x \leq 1 .
$$

The variable `x` should be read operationally: it orders the accumulated
projected response along the diagnostic light-path/reconstruction depth. It is
not a claim that the full underlying theory has been reconstructed from the
paper.

The finite-memory correction is a multiplicative response operator acting on a
baseline projected shape:

$$
K_2(x) = W(x)K_1(x).
$$

This note studies the locked K2 form

$$
W(x) = 1 + \rho x^3 .
$$

The form is intentionally simple. Its purpose is to test whether a bounded,
delayed, monotone memory response can be made reproducible before comparison
with diagnostic envelopes.

The baseline shape $K_1(x)$ is not treated as a fitted degree of freedom in
this note. The comparison is organized around whether the locked multiplicative
memory factor can keep the projected K2 response inside the reconstructed
diagnostic envelope under the predeclared amplitude and shape rules.

## 3. Passive Memory Bound

The passive memory-budget condition requires the accumulated tail response not
to exceed the unit local response budget. For the cubic operator,

$$
E_{\mathrm{tail}} = \int_0^1 \rho x^3\,dx = \frac{\rho}{4}.
$$

The unit baseline budget is

$$
E_0 = \int_0^1 1\,dx = 1.
$$

Passivity requires

$$
E_{\mathrm{tail}} \leq E_0,\qquad
\frac{\rho}{4} \leq 1,\qquad
\rho \leq 4 .
$$

This is the key discipline of the construction: the memory depth is bounded
before the diagnostic comparison. The bound is not chosen by looking for the
best residual fit.

## 4. Kernel-Shape Selection

The cubic kernel is selected from the power-kernel family

$$
W_p(x) = 1 + \rho x^p .
$$

For this family, the passive memory rule generalizes to

$$
\int_0^1 \rho x^p\,dx \leq \int_0^1 1\,dx,\qquad
\frac{\rho}{p+1} \leq 1,\qquad
\rho \leq p+1 .
$$

Two additional effective-operator rules select the usable shape:

$$
\Delta W_p(0.25) = (p+1)0.25^p \leq 0.10 ,
$$

$$
\int_{0.75}^{1} (p+1)x^p\,dx \leq 0.75 .
$$

The first rule rejects kernels that disturb the already locked low-depth
response too early. The second rejects kernels whose memory budget collapses
too sharply onto the last quarter of the path. In the present audit, `p=1` and
`p=2` are too visible at low depth, while `p>=4` is too endpoint-concentrated.
The cubic `p=3` case is the remaining admissible power-kernel representative.

The locked diagnostic window is therefore

$$
W(x) = 1 + \rho x^3,\qquad
\eta \in [0.25,0.50],\qquad
\rho \in [3.00,4.00].
$$

## 5. Diagnostic Targets And Gate Policy

The targets used here are reconstructed diagnostic envelopes rather than direct
published likelihoods. The comparison is therefore deliberately separated into
three levels:

```text
sign-stable reconstructed point   -> exact sign gate
sign-unstable reconstructed point -> envelope / diagonal residual gate
controls and extrapolations       -> stress diagnostics only
```

Operationally, let $y_i$ denote the reconstructed diagnostic median at the
tested point $i$, and let $[L_i,U_i]$ denote the corresponding reconstructed
diagnostic envelope. A locked prediction $\hat y_i$ passes the envelope gate
when

$$
L_i \leq \hat y_i \leq U_i .
$$

If a diagonal diagnostic width $\sigma_i$ is available, the normalized residual
gate is

$$
\left|\hat y_i-y_i\right|/\sigma_i \leq 1 .
$$

A reconstructed point is sign-stable only when the relevant method/degree
families agree on the sign of the diagnostic median. If the reconstruction
sign is method-sensitive, the median sign is not used as a hard falsifier.
Instead, the locked K2 prediction must remain inside the diagnostic envelope
and have a normalized residual not exceeding one standard diagnostic width.

This policy is not a substitute for a full likelihood. It is a triage rule that
prevents a method-sensitive reconstructed median from being overinterpreted.

This distinction is important for the SN+BAO stress test below. A strict
median-sign gate asks whether the prediction follows the sign of one
reconstructed median. The sign-stability gate asks a weaker but better-posed
question: whether the prediction violates a sign that is stable across
reconstruction choices. Only the second question is used as a paper-level
diagnostic pass/fail rule here.

## 6. Results

The minimal result summary is:

| Diagnostic | Result | Interpretation |
|---|---:|---|
| BAO-only window overlap | 1.0000000000 | Locked K2 overlaps the BAO-only diagnostic envelope at all tested points. |
| BAO-only best curve overlap | 1.0000000000 | The best locked K2 BAO-only curve remains inside the envelope. |
| SN+BAO sign-stable pass fraction | 1.0000000000 | All sign-stable SN+BAO points pass exact sign matching. |
| SN+BAO sign-unstable likelihood pass fraction | 1.0000000000 | All sign-unstable SN+BAO points pass envelope / diagonal residual handling. |

The strict SN+BAO median-sign test exhibits a localized tension near
`z=1.1925`. The diagnostic audit shows that this point is method-degree
sensitive: lower-degree reconstructions are positive, while higher-degree
reconstructions pull the median negative. The locked K2 prediction does not
follow the negative median sign at that point, but it remains inside the broad
diagnostic envelope with a small normalized residual. Under the sign-stability
gate, this is treated as a likelihood/envelope pass rather than a hard
sign-failure.

The current status is therefore:

```text
BAO-only: diagnostic pass
SN+BAO strict median-sign: localized warning
SN+BAO sign-stability-aware gate: diagnostic pass
claim level: theory-method diagnostic, not observational discovery
```

## 7. Expected Significance

The main significance of the construction is not that it proves a new
cosmological model. Its value is methodological:

- it gives a compact finite-memory operator whose amplitude is bounded before
  comparison with data;
- it interfaces naturally with FLRW consistency, optical-propagation, and
  backreaction tests;
- it demonstrates a way to handle sign-unstable reconstructed diagnostics
  without silently overclaiming;
- it provides a small public module that can be tested independently of the
  full underlying theory program.

The near-term audience is likely narrow: researchers interested in
cosmological consistency tests, backreaction, light propagation, and
method-level modified-gravity phenomenology. The higher-impact route requires
a later full covariance or shrinkage-covariance likelihood comparison with
direct public likelihood products.

## 8. Limitations

This manuscript is a theory-method diagnostic note. It does not claim:

- a full covariance likelihood;
- a direct observational detection;
- exclusion of cosmic backreaction;
- a complete derivation of cosmology from an underlying action;
- disclosure or reconstruction of a full Tau Core theory.

The next stage is a paper-aligned likelihood comparison using covariance or
shrinkage-covariance products and direct published likelihood data where
available.

## 9. Conclusion

We have defined a finite-memory projection correction as a bounded diagnostic
operator rather than as a complete cosmological model. The locked cubic form
$W(x)=1+\rho x^3$ follows from a passive memory budget and a simple
shape-selection audit over power kernels. With $\rho \leq 4$, the operator gives
a compact K2 diagnostic window that can be compared against reconstructed
cosmological consistency envelopes without fitting the memory depth after the
fact.

Within the distilled diagnostic packet used here, the locked K2 window is
compatible with the BAO-only envelope and passes the reconstruction-aware
SN+BAO sign-stability gate. The strict SN+BAO median-sign warning is retained
as a limitation rather than hidden: it marks a reconstruction-sensitive point
that should be revisited with direct likelihood products.

The result is therefore a paper-ready method claim, not an observational
discovery claim. Its next meaningful test is a covariance-aware likelihood
comparison against public likelihood data.

## 10. Data And Code Availability

This draft uses a distilled diagnostic packet rather than a direct public
likelihood product. The public repository contains the manuscript scaffold, the
current PDF renderer, and compact result tables used in this note. The current
diagnostic evidence files are:

- `evidence/result_summary.csv`;
- `evidence/claim_matrix.csv`;
- `evidence/source_packet_manifest.csv`.

The PDF can be regenerated locally with:

```text
python3 -m pip install -r requirements.txt
python3 make_pdf.py
```

The underlying comparison should be treated as a reconstruction-level
diagnostic until direct likelihood products or covariance/shrinkage-covariance
inputs are added.

## References

[1] A. Heinesen and T. Clifton, "Observational Tests for Distinguishing Classes
of Cosmological Models", arXiv:2604.07244, 2026.
https://arxiv.org/abs/2604.07244

[2] S. M. Koksbang, "First observational constraints on cosmic backreaction
over an extended redshift range", arXiv:2604.11249, 2026.
https://arxiv.org/abs/2604.11249

[3] C. C. Dyer and R. C. Roeder, "The Distance-Redshift Relation for Universes
with No Intergalactic Medium", The Astrophysical Journal 174, L115-L117,
1972.

[4] C. C. Dyer and R. C. Roeder, "Distance-Redshift Relations for Universes
with Some Intergalactic Medium", The Astrophysical Journal 180, L31-L34,
1973.
