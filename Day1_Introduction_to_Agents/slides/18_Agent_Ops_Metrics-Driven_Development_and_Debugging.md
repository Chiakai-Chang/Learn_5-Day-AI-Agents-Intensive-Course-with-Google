# Agent Ops: Metrics, Development, and Debugging

- **Measure What Matters:** Define business KPIs (e.g., goal completion rates, user satisfaction) to measure real-world impact.
- **Use an "LM as Judge":** Automatically assess agent output quality against a predefined rubric and a "golden dataset" of prompts.
- **Metrics-Driven Development:** Use automated quality scores to create a confident go/no-go process for deploying changes.
- **Debug with Traces:** Use OpenTelemetry traces to get a step-by-step recording of the agent's execution path (trajectory) to diagnose the root cause of failures.
- **Cherish Human Feedback:** Use bug reports and user feedback to create new, permanent test cases, vaccinating the system against future errors.