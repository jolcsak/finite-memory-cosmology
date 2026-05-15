# Paper 5 Candidate: Finite-Memory Projection Corrections

This paper packet distills the cosmology branch into the smallest publishable
theory-method draft. Its role is to present a reproducible finite-memory
projection operator and diagnostic comparison protocol without exposing or
requiring the full Tau Core program.

## Status

Working paper scaffold. This is ready for a theory-method diagnostic draft, not
for an observational discovery claim.

## Scope

The paper may claim that a predeclared finite-memory projection operator,

```text
W(x) = 1 + rho*x^3,  rho <= 4
```

defines a bounded diagnostic correction window that is compatible with the
BAO-only reconstructed consistency envelope and passes a reconstruction-aware
SN+BAO sign-stability gate.

The paper must not claim that:

- Tau Core is fully disclosed or proven;
- the K2 operator is the final Tau cosmology law;
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
- `evidence/source_packet_manifest.csv`: source packet map.

## Regenerate The PDF

```text
python3 -m pip install -r requirements.txt
python3 make_pdf.py
```

## Relation To Tau Core

The paper exposes only an effective cosmology module: projected depth, passive
finite memory, and the diagnostic K2 window. It intentionally does not disclose
the full Tau Core ontology, full action program, galactic branch, or internal
gate history.
