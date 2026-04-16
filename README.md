# Credit Risk Model Governance Console

![Demo Screenshot](demo/screenshot.png)

## Overview

Track model experiments, approvals, drift, and release decisions for credit risk and lending models under governance controls.

## Real-world problem

- User: Model risk managers and lending analytics leaders
- Problem: Credit models need traceable approvals, challenge reviews, and release evidence that generic experiment trackers don't surface clearly.
- Decision improved: Approve, challenge, or hold model releases before lending exposure changes reach production.
- KPI target: Reduce governance cycle time and model release risk.

## Why this matters

This repo is positioned as a real product for a real team, not a framework-only demo. The goal is to show how research-backed AI, analytics, or graph systems become deployable workflows with docs, UI, screenshots, and business-facing outputs.

## Project profile

- Domain: Model Risk Management
- Project type: `ml`
- Tags: credit-risk, governance, mlops, finance

## Workflow

1. Ingest the operational context for the user and case.
2. Score risk, quality, or opportunity using the project API.
3. Compare current signals against a business baseline.
4. Generate a recommendation or operator brief for the next step.

## Quick start

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python scripts/bootstrap_data.py
uvicorn src.app.main:app --host 0.0.0.0 --port 8000 --reload
```

Open `http://localhost:8000/` to use the interactive application.

## Key endpoints

- `GET /`
- `GET /health`
- `GET /bootstrap`
- `GET /project`
- `POST /score`
- `POST /analyze`
- `POST /query`
- `POST /recommend`

## Documentation

- [Architecture](docs/architecture.md)
- [Evaluation](docs/evaluation.md)
- [Runbook](docs/runbook.md)
- [Innovation memo](research/innovation_memo.md)
- [Upstream audit](research/upstream_audit.md)
