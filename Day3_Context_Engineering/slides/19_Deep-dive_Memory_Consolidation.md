# Deep-dive: Memory Consolidation

**Goal: Integrate new information into a coherent, accurate, and evolving knowledge base.**

*   This "self-curation" is what elevates a memory manager beyond a simple database.
*   It solves problems like information duplication, conflicts, and evolution.

**The LLM-driven Workflow:**
1.  Retrieve existing memories similar to the new information.
2.  An LLM analyzes both the existing and new memories.
3.  The LLM decides which operation to perform:
    *   **UPDATE:** Modify an existing memory.
    *   **CREATE:** Create a new memory for a novel topic.
    *   **DELETE:** Invalidate an old, incorrect memory.