# Timing for Retrieval: Proactive vs. Reactive

**When should the agent retrieve memories?**

1.  **Proactive Retrieval (Eager):**
    *   Memories are automatically loaded at the start of **every turn**.
    *   **Pros:** Context is always available.
    *   **Cons:** Can introduce unnecessary latency if the turn doesn't require memory.

2.  **Reactive Retrieval (Lazy / Memory-as-a-Tool):**
    *   The agent is given a tool to query memory and decides for itself **when to retrieve context**.
    *   **Pros:** More efficient; latency is only incurred when needed.
    *   **Cons:** Requires an additional LLM call to decide; agent might not know relevant info exists.