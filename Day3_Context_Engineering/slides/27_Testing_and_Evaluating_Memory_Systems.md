# Testing and Evaluating Memory Systems

Evaluation is a multi-layered process to ensure the agent remembers the right things and uses them effectively.

1.  **Memory Generation Quality:**
    *   Is the agent remembering the right things?
    *   **Metrics:** Precision, Recall, F1-Score (compared against a "golden set").

2.  **Memory Retrieval Performance:**
    *   Can the agent find the right memory at the right time?
    *   **Metrics:** Recall@K, Latency.

3.  **End-to-End Task Success:**
    *   Does memory actually help the agent perform its job better?
    *   **Method:** Use an LLM "judge" to compare the agent's final output to a golden answer.