# Architecture

## Problem framing

- User: Model risk managers and lending analytics leaders
- Problem: Credit models need traceable approvals, challenge reviews, and release evidence that generic experiment trackers don't surface clearly.
- Decision: Approve, challenge, or hold model releases before lending exposure changes reach production.

## System flow

1. A user submits case context, business signals, or a search question.
2. The API exposes scoring, analysis, and recommendation endpoints.
3. The web application turns those outputs into an operator-facing workflow.
4. Observability, docs, and runbooks make the project easier to evaluate and extend.

## Production posture

- Separate app, docs, demo, and data folders
- Container-ready packaging
- API endpoints for health and workflow actions
- Screenshot-ready demo surface
- Research and upstream audit artifacts included in-repo
