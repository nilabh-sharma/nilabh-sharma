# Building my first Claude agent

!!! info "Build log — publishing in Sprint 4"

## The use case

An agent that **profiles a Databricks table and drafts data-quality rules**:

1. Reads table metadata (schema, row count, partitioning)
2. Runs profiling queries (null rates, distinct counts, min/max, pattern checks)
3. Proposes DQ expectations with a rationale for each
4. Flags columns that look like PII

## Success criteria (defined before building)

- [ ] Produces sensible rules for 8 of 10 test tables
- [ ] Never runs a write or DDL statement (read-only credentials)
- [ ] Every query it ran is logged and reproducible
- [ ] Cost per table profiled is known

## Sections to write

- Design: the tools the agent can call
- Build: minimal version with the Claude API / Agent SDK
- Evaluation: results on 10 real tables
- What went wrong, and what I changed
