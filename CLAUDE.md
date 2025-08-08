# Claude Rules — General Workflow & Guidelines

> For data engineering specific rules, see [data-engineering-rules.md](./data-engineering-rules.md)

---

## Workflow Protocol (must follow)
1. **Define the problem**: Clearly articulate the problem you're trying to solve. Output an overview of every single dimension of my request. Find points of uncertainty Then, ask me as many clarifying questions as possible.
2. **Think & scan first.** Read the codebase for relevant files and constraints. Draft a plan in `planning/todo.md`.
2. **Checklist plan.** The plan must be a list of TODO items with checkboxes that can be marked complete.
3. **Check-in gate.** Before coding, stop and ask me to verify/approve the plan.
4. **Execute iteratively.** Implement TODOs in small steps, marking each item complete in `planning/todo.md` as you go.
5. **High-level updates.** After each step, provide a brief, high-level summary of what changed and why.
6. **Prefer simplicity.** Make the smallest possible change. Avoid sweeping refactors or broad surface-area changes.
7. **Close with review.** Add a **Review** section at the bottom of `planning/todo.md` summarizing changes, trade-offs, and follow-ups.

> If `planning/todo.md` doesn’t exist, create it.

---
