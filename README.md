# Interventional Care Pathways

A local pathway analytics workbench that simulates ketamine/TMS-style treatment journeys, flags drop-off risk, and explains operational bottlenecks by clinic, payer, and care step.

## Why This Exists

interventional psychiatry clinics need care-pathway visibility that connects patient experience, treatment cadence, insurance friction, and outcomes without flattening clinical nuance.

## What It Builds

- Replays synthetic `interventional` and `psychiatry` cases against the project's evidence rules.
- Scores `interventional_coverage`, `psychiatry_risk`, and `clinics_precision` so regressions are visible in CSV and JSON.
- Plants `interventional drift` and `psychiatry gap` failures as negative controls.
- Writes citation-locked decision claims; unsupported claims fail verification.
- Exports a review dashboard and demo pack for `interventional-care-pathways` without hosted services.

## Local Run

```bash
uv sync
uv run interventional-care-pathways all
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/analysis.json`
- `outputs/scenario_report.csv`
- `outputs/decision_report.md`
- `outputs/evidence_packet.md`
- `outputs/domain_rubric.json`
- `outputs/failure_matrix.md`
- `outputs/trace_graph.mmd`
- `outputs/dashboard.html`
- `outputs/demo_pack.zip`

## Sources

- https://www.beckersbehavioralhealth.com/uncategorized/radials-ceo-on-leading-with-lived-experience/
- https://theorg.com/org/radial-1/org-chart/john-capecelatro

## Boundary

This repository uses synthetic fixtures only. It has no credentials, no customer data, no outreach data, and no dependency on a hosted API.
