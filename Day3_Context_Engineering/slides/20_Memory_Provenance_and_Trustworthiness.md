# Memory Provenance & Trust

**"Garbage in, garbage out" is critical for LLMs.** An agent must be able to evaluate the quality of its own memories.

*   **Provenance:** A detailed record of a memory's origin and history.
*   **Why it matters:**
    1.  **Memory Consolidation:** Informs conflict resolution by establishing a hierarchy of trust.
    2.  **Inference:** Informs how much the agent should rely on a memory.

*   **Source Types (Hierarchy of Trust):**
    1.  **Bootstrapped Data (High Trust):** Pre-loaded from systems like a CRM.
    2.  **Explicit User Input (High Trust):** Direct commands like "Remember this."
    3.  **Implicit User Input (Lower Trust):** Inferred from conversation.
    4.  **Tool Output (Brittle):** Best for short-term caching.