# Advanced Pattern: Memory-as-a-Tool

**A sophisticated approach where the agent decides for itself when to create or retrieve a memory.**

*   **How it works:** Memory generation and retrieval are exposed to the agent as tools (e.g., `create_memory`, `search_memory`).

*   **Shift in Responsibility:** The agent's LLM, guided by the tool's description and the conversation's context, autonomously decides when it's appropriate to call these tools.

*   **Benefits:**
    *   More efficient and robust than triggering on every turn.
    *   Allows the agent to be more deliberate about what it remembers and when it accesses that memory.