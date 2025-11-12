# When to Trigger Memory Generation?

This is a critical architectural choice, balancing data freshness against cost and latency.

**Triggering Strategies:**
*   **Session Completion:** At the end of a multi-turn session (cost-effective, lower fidelity).
*   **Turn Cadence:** After a specific number of turns (e.g., every 5 turns).
*   **Real-Time:** After every single turn (highest cost, highest fidelity).
*   **Explicit Command:** Upon a direct user command (e.g., "Remember this").
*   **Memory-as-a-Tool (Advanced):** The agent itself decides when to call a `create_memory` tool.