# Working rules for this repo

## Token economy (standing rule, every task)

Applies to the main conversation only, not to subagents.

- Keep replies short: result first, no recaps, no option lists unless asked.
- Read only the files and line ranges the task needs; prefer Grep and targeted reads over whole-file reads.
- Batch independent tool calls in one turn; do not re-read files already in context.
- Delegate to subagents freely for real work (design, build, QA). Subagents and ECC agents run on their own token budgets: do not ration or trim their work, let them go as deep as the task needs.
- Verify once in a bounded pass (build, one desktop and one mobile screenshot), not in a loop.
- Summaries to the user: under ~10 lines unless they ask for detail.

## ECC

ECC (`ecc@ecc`) is enabled at project scope. Use the relevant ECC agents for real engineering work (design, build, review, QA), picking only what the task needs.
