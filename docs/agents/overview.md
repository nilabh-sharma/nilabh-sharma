# Agents as non-deterministic DAGs


## Outline

1. **A pipeline you know:** a DAG where you define every task and edge up front.
2. **An agent:** the same building blocks (tasks = *tools*), but the LLM chooses which task runs next, based on the result of the last one.
3. **The loop:** observe → decide → call a tool → read the result → repeat until done.
4. **What that breaks:** reproducibility, runtime estimates, cost predictability, and testing.
5. **What you already know that still applies:** idempotent tasks, retries, timeouts, least-privilege credentials, logging every step (lineage for decisions).
6. **When NOT to use an agent:** if you can draw the DAG, build the DAG. Agents are for when the path genuinely depends on what you find.
