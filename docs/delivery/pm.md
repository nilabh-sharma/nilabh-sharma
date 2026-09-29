# Managing AI projects

!!! info "Draft"

## How AI delivery differs from data delivery

| Area | Data project | AI project |
|---|---|---|
| Definition of done | Output matches spec | Output meets an agreed quality threshold on an evaluation set |
| Estimation | Mostly deterministic | Needs time-boxed experimentation |
| Testing | Reconciliation, DQ rules | Evaluation sets, human review, regression on prompts |
| Run cost | Compute and storage | Plus per-call inference cost, which scales with usage |
| After go-live | Monitoring pipelines | Plus monitoring output quality and drift |

## Practical rules (draft)

1. Agree the evaluation set and pass threshold with the business **before** building.
2. Time-box experiments; decide go/no-go on evidence.
3. Budget inference cost explicitly — it's opex that grows with adoption.
4. Data readiness is the most common blocker. Check it first.
