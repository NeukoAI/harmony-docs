# How Honcho Powers Memory

To support relationship-aware memory, Harmony uses [Honcho's](https://honcho.dev) stateful memory architecture.

Honcho organizes memory using four primitives:

| Primitive | Purpose |
|---|---|
| **Workspaces** | Isolation boundary for the campaign environment |
| **Peers** | Persistent entities (participants and agents) whose profiles evolve over time |
| **Sessions** | Bounded interaction threads where events and messages are logged |
| **Messages** | Atomic interaction records that trigger background reasoning |

As messages accumulate, Honcho runs asynchronous reasoning and creates structured representations. This enables context retrieval that is not limited to literal recall, but includes **pattern-level understanding across sessions**.

For this campaign, that means the system can carry forward relational context instead of starting from zero every cycle. It can track changing participant behavior, contradictory signals, and evolving trust patterns — while keeping responses grounded in current phase state.
