# 05: Evaluation in Practice: Black Box vs. Glass Box

## 1. The "Outside-In" View (The Black Box)

**Question:** "Did the agent achieve the user's goal effectively?"

*   **What:** Evaluate the final performance against the objective.
*   **Metrics:**
    *   **Task Success Rate:** Binary score of whether the problem was solved.
    *   **User Satisfaction:** Direct user feedback (e.g., CSAT, thumbs up/down).
    *   **Overall Quality:** Accuracy, completeness of the final output.

## 2. The "Inside-Out" View (The Glass Box)

**Question:** "*Why* did the agent succeed or fail?"

*   **What:** Analyze the agent's approach by assessing its execution trajectory.
*   **Components to Assess:**
    *   LLM Planning (The "Thought")
    *   Tool Usage (Selection & Parameters)
    *   Tool Response Interpretation (The "Observation")
    *   RAG Performance
    *   Trajectory Efficiency and Robustness