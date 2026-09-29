# LLMs for data engineers

!!! info "Draft — publishing in Sprint 1"
    Outline below. Replace with the full article as you write it.

## Outline

1. **What an LLM actually is** — a function: text in, most-likely text out. No database, no memory between calls unless you pass it in.
2. **Tokens are your unit of volume** — like rows or bytes. Pricing, limits and latency are all measured in tokens.
3. **The context window is working memory** — think of it as the max payload of a single request. Everything the model needs must fit in it.
4. **Cost is capacity planning** — input tokens × price + output tokens × price, per call, × calls per day. Estimate it exactly as you would compute cost.
5. **Temperature and non-determinism** — why the same input can give different outputs, and why that breaks your usual testing habits.
6. **Where LLMs fit in a data platform** — enrichment (classification, extraction), interfaces (text-to-SQL, Q&A over docs), and automation (agents).

## Key takeaway (draft)

> Treat the LLM as a stateless, probabilistic transformation step. Everything else — data, memory, access control, testing — is still your job.
