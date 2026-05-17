# Finite-Memory Projection Corrections

This repository contains a public method-note packet for a bounded
finite-memory projection correction in cosmological consistency diagnostics.
Its role is to present a reproducible, predeclared diagnostic operator and a
modest comparison protocol for reconstruction-level envelopes.

## Status

Release-candidate method note. This is suitable for a disciplined diagnostic
proposal, not for an observational discovery claim.

## Scope

The paper may claim that a predeclared finite-memory projection operator,

```text
W(x) = 1 + rho*x^3,  rho <= 4
```

defines a bounded diagnostic correction window that is compatible with the
BAO-only reconstructed consistency envelope and remains non-violating under a
reconstruction-aware SN+BAO sign-stability gate.

The paper must not claim that:

- the K2 operator is the final cosmological law;
- any background theory is proven;
- cosmic backreaction is ruled out;
- a full covariance likelihood has been completed;
- the current diagnostics constitute an observational detection.

## Files

- `draft.md`: initial manuscript scaffold.
- `finite_memory_projection_corrections.pdf`: rendered PDF of the current draft.
- `outline.md`: section-level outline.
- `status.md`: claim discipline, current strength, and blockers.
- `reproducibility.md`: regeneration commands and source packets.
- `make_pdf.py`: lightweight ReportLab PDF renderer with display-equation support.
- `evidence/claim_matrix.csv`: distilled allowed/forbidden claims.
- `evidence/result_summary.csv`: minimal result table for the draft.
- `evidence/diagnostic_point_audit.csv`: point-level SN+BAO diagnostic gate table.
- `evidence/coordinate_mapping_policy.csv`: coordinate-mapping status and risks.
- `evidence/threshold_sensitivity.csv`: threshold-policy sensitivity plan.
- `evidence/threshold_kernel_outcomes.csv`: simple power-kernel outcomes under threshold variants.
- `evidence/open_problem_resolution_matrix.csv`: audit map from weakness to resolution.
- `evidence/source_packet_manifest.csv`: source packet map.

## Regenerate The PDF

```text
python3 -m pip install -r requirements.txt
python3 make_pdf.py
```

## Scope Boundary

This paper is self-contained as a bounded diagnostic proposal. It does not
require or prove any broader background theory.
