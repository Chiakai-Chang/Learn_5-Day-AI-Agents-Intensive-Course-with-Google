# 06: The Judges: Automated & AI-Driven Evaluation

Knowing *what* to evaluate is half the battle. *How* to judge it requires a sophisticated, hybrid approach.

## Automated Systems for Scale

1.  **Automated Metrics:**
    *   **What:** String/embedding similarity (ROUGE, BERTScore), task-specific benchmarks.
    *   **Value:** Provide speed, reproducibility, and trend indicators for regression testing.
    *   **Limitation:** Shallow; they capture surface similarity, not deep reasoning.

2.  **LLM-as-a-Judge:**
    *   **What:** Use a powerful LLM (e.g., Gemini Advanced) to evaluate another agent's output against a detailed rubric.
    *   **Value:** Scalable, fast, and nuanced feedback on qualitative aspects.

3.  **Agent-as-a-Judge:**
    *   **What:** Use one agent to evaluate the full execution *trace* of another.
    *   **Value:** Assesses the process itself (plan quality, tool use), not just the output.