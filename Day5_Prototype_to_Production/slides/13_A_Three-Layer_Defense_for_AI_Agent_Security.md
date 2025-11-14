# A Three-Layer Defense for AI Agent Security

Fortunately, frameworks like Google's Secure AI Agents approach and the Google Secure AI Framework (SAIF) address these challenges through three layers of defense:

1.  **Policy Definition and System Instructions (The Agent's Constitution)**: Defining policies for desired and undesired agent behavior, engineered into System Instructions (SIs) that act as the agent's core constitution.
2.  **Guardrails, Safeguards, and Filtering (The Enforcement Layer)**: This layer acts as the hard-stop enforcement mechanism.
    -   **Input Filtering**: Use classifiers and services like the Perspective API to analyze prompts and block malicious inputs.
    -   **Output Filtering**: Vertex AI's built-in safety filters provide a final check for harmful content, PII, or policy violations.
    -   **Human-in-the-Loop (HITL) Escalation**: For high-risk or ambiguous actions, the system must pause and escalate to a human for review and approval.
3.  **Continuous Assurance and Testing**: Safety is not a one-time setup; it requires constant evaluation and adaptation.
    -   **Rigorous Evaluation**: Any change to the model or its safety systems must trigger a full re-run of a comprehensive evaluation pipeline.
    -   **Dedicated RAI Testing**: Rigorously test for specific risks using dedicated datasets or simulation agents, including Neutral Point of View (NPOV) and Parity evaluations.
    -   **Proactive Red Teaming**: Actively try to break the safety systems through creative manual testing and AI-driven persona-based simulation.