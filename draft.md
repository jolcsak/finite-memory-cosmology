# Finite-Memory Projection Corrections In Cosmological Consistency Diagnostics

## Abstract

We introduce a bounded finite-memory projection operator for diagnostic
cosmological consistency tests. The operator is formulated as an effective
projection response over normalized depth, `W(x)=1+rho*x^3`, with a passive
memory-budget bound `rho<=4`. The construction is not presented as a complete
cosmological model or an observational detection, but as a disciplined
diagnostic module for comparing projected response shapes against
backreaction-aware distance consistency reconstructions. In a BAO-only
diagnostic reconstruction, the locked K2 window overlaps the full target
envelope. In an SN+BAO source-split stress test, strict median-sign matching
exhibits a localized tension; a reconstruction-aware sign-stability gate
resolves this tension without widening the K2 window. The result motivates a
future full-likelihood comparison while preserving clear claim boundaries.

## 1. Introduction

Cosmological consistency tests increasingly distinguish background expansion,
light-propagation effects, and cosmic backreaction. A residual relative to a
standard homogeneous model is therefore not automatically evidence for new
physics: it may arise from optical sampling, reconstruction convention, or
averaging effects. This note develops a deliberately narrow projection-memory
diagnostic that can be placed alongside such tests.

The objective is not to disclose or validate a full underlying theory. Instead,
we ask whether a predeclared, bounded projection-memory operator can define a
reproducible diagnostic window and survive basic source-split stress tests.

## 2. Finite-Memory Operator

Let `x in [0,1]` denote normalized projected depth. We consider a finite-memory
response multiplier

```text
W(x) = 1 + rho*x^3.
```

The passive memory-budget condition requires the accumulated tail response not
to exceed the unit local response budget:

```text
Integral_0^1 rho*x^3 dx <= Integral_0^1 1 dx.
```

Thus

```text
rho/4 <= 1,
rho <= 4.
```

The cubic power is selected from the power-kernel family `W_p(x)=1+rho*x^p`.
Lower powers are too visible at low depth, while higher powers concentrate the
memory budget too sharply near the endpoint. The resulting locked diagnostic
window is

```text
eta in [0.25, 0.50],
rho in [3.00, 4.00].
```

## 3. Diagnostic Protocol

The diagnostic targets are reconstructed envelopes rather than direct
published likelihoods. We therefore separate three levels of comparison:

```text
sign-stable reconstructed points   -> exact sign gate
sign-unstable reconstructed points -> envelope / diagonal residual gate
controls and extrapolations        -> stress diagnostics only
```

This policy prevents an unstable reconstructed median sign from acting as a
hard falsifier while preserving the stricter sign requirement where the
reconstruction is stable.

## 4. Preliminary Results

The locked K2 window overlaps the BAO-only diagnostic envelope at all tested
points. In SN+BAO, strict median-sign matching fails at a localized point near
`z=1.1925`. That point is method-degree sensitive: lower-degree reconstructions
are positive, while higher-degree reconstructions pull the median negative.

Under the sign-stability-aware diagnostic gate, all stable-sign points pass the
exact sign check and all unstable-sign points pass the envelope / diagonal
residual check.

## 5. Limitations

This manuscript is a theory-method diagnostic note. It does not claim a full
covariance likelihood, a direct observational detection, or a complete
derivation of cosmology from an underlying action. The next stage is a
paper-aligned likelihood comparison using covariance or shrinkage-covariance
products and direct published likelihood data where available.
