# Sessions in Multi-Agent Systems

How do collaborating agents share information?

1.  **Shared, Unified History:**
    *   All agents read from and write to a single, central conversation log.
    *   **Best for:** Tightly coupled, collaborative tasks requiring a single source of truth.

2.  **Separate, Individual Histories:**
    *   Each agent maintains its own private log and acts as a "black box."
    *   Communication happens via explicit messages (e.g., Agent-as-a-Tool, A2A Protocol).
    *   **Best for:** Decoupled tasks where process privacy is desired.