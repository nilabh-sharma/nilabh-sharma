# Nilabh Sharma — Data, AI & Delivery

**AI for data engineers — explained in the language you already speak: pipelines, tables, grain, SLAs and lineage.**

Most AI material is written for ML researchers or for complete beginners. This site is for people who have spent years moving, modelling and governing data — and want to understand where LLMs, RAG and agents actually fit, without the hype.

## The core idea

Almost every "new" AI concept maps onto something a data engineer already knows:

| AI concept | What you already know | The part that is genuinely new |
|---|---|---|
| **RAG** (retrieval-augmented generation) | An ETL pipeline whose sink is a vector index | Retrieval is by *meaning*, not by key |
| **Embeddings** | A derived column | It changes whenever the embedding model changes |
| **Chunking** | Choosing the grain of a table | Wrong grain silently ruins answer quality |
| **Agents** | A DAG orchestrated by Airflow / Workflows | The LLM decides the next task at runtime |
| **Evaluation** | Data-quality tests and reconciliation | Outputs are probabilistic, so tests are statistical |
| **Guardrails** | Row-level security and data contracts | They apply to *generated* text, not just stored data |

## Start here

<div class="grid cards" markdown>

- **[RAG is just ETL with a new sink](foundations/rag.md)**
  The retrieval pipeline, stage by stage, mapped to ETL.

- **[LLMs for data engineers](foundations/llms.md)**
  Tokens, context windows and cost — as capacity planning.

- **[Agents as non-deterministic DAGs](agents/overview.md)**
  What changes when the orchestrator can think.

- **[Building my first Claude agent](agents/first-agent.md)**
  A real build log: a Databricks table-profiling agent.

</div>

## Learning in public

This site is written as I work through my own AI upskilling plan. Each article is published at the end of a two-week sprint, with what worked, what didn't, and what I'd do differently.
