# Operator Brief: Radial

Radial gets a local, deterministic pressure test around interventional, psychiatry, and clinics. The useful part is not the dashboard; it is the repeatable evidence path from fixture to failure to operator action.

## Highest-leverage checks

- interventional evidence replay -> block release until cited evidence is regenerated (interventional_coverage, evidence ev_0044).
- care-pathway operator packet -> accept only if decision claims cite fixture evidence (psychiatry_risk, evidence ev_0143).
- clinics regression harness -> open a regression issue with trace and benchmark delta (clinics_precision, evidence ev_0066).
- psychiatry boundary probe -> route to reviewer with evidence packet (care-pathway_latency, evidence ev_0121).

## What makes this useful

The workflow is intentionally local and deterministic. A reviewer can run the same fixture set, inspect the evidence IDs, open the dashboard, and see exactly why a recommendation passed, went to review, or blocked.
