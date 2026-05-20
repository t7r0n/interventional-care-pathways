# Interventional Care Pathways

A local pathway analytics workbench that simulates ketamine/TMS-style treatment journeys, flags drop-off risk, and explains operational bottlenecks by clinic, payer, and care step.

![Interventional Care Pathways working dashboard](outputs/project_working.svg)

## Why it exists

interventional psychiatry clinics need care-pathway visibility that connects patient experience, treatment cadence, insurance friction, and outcomes without flattening clinical nuance.

Most internal demos stop at a pretty chart. This repository is built around the harder part: a repeatable path from fixture, to failure, to evidence, to the operator action a serious team would actually trust.

## What is inside

- A deterministic replay harness tuned around interventional, psychiatry, and clinics.
- Company-specific strategy code in `src/interventional_care_pathways/strategy.py`, not just README-level customization.
- Citation-locked reports where every decision claim has to point back to a generated evidence ID.
- Two visual artifacts generated from the latest run: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, and benchmark artifacts.

![Interventional Care Pathways evidence map](outputs/evidence_map.svg)

## Signals it measures

- `interventional coverage`
- `psychiatry risk`
- `clinics precision`
- `care-pathway latency`

## Failure modes it plants

- interventional drift
- psychiatry gap
- clinics misroute
- care-pathway blindspot

## Run it locally

```bash
uv sync
uv run interventional-care-pathways all
uv run pytest -q
uv run ruff check .
```

## Outputs worth opening

- `outputs/dashboard.html`
- `outputs/project_working.svg`
- `outputs/evidence_map.svg`
- `outputs/operator_brief.md`
- `outputs/decision_report.md`
- `outputs/strategy_model.json`
- `outputs/demo_pack.zip`

## Sources

- https://www.beckersbehavioralhealth.com/uncategorized/radials-ceo-on-leading-with-lived-experience/
- https://theorg.com/org/radial-1/org-chart/john-capecelatro

## Boundary

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.
