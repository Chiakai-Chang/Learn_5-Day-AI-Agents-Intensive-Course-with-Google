# How Agents Evolve and Learn

To avoid performance degradation or "aging," agents must be designed to learn and adapt autonomously.

- **Learning Sources:**
  - **Runtime Experience:** Session logs, traces, and especially Human-in-the-Loop (HITL) feedback.
  - **External Signals:** Updated documents, new policies, or critiques from other agents.
- **Adaptation Techniques:**
  - **Enhanced Context Engineering:** Continuously refining prompts and retrieved information.
  - **Tool Optimization and Creation:** Identifying capability gaps and creating new tools (e.g., a Python script) on the fly.
- **Example:** A compliance agent learns a new data anonymization rule from a human expert's correction and automatically applies it in the future.