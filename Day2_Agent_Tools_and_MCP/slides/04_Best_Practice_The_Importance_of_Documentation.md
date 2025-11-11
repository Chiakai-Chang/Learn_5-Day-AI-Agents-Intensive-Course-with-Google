# Best Practice: The Importance of Documentation

Tool documentation (name, description, parameters) is passed to the model and is critical for correct usage.

- **Use a Clear Name:** Be descriptive and specific (e.g., `create_critical_bug_in_jira` is better than `update_jira`).

- **Describe All Parameters:** Clearly define the type and purpose of all inputs and outputs.

- **Simplify Parameter Lists:** Keep parameter lists short and clearly named to avoid confusing the model.

- **Clarify Descriptions:** Use simple, non-technical language to explain the tool's purpose and functionality.

- **Add Targeted Examples:** Use examples to clarify ambiguities and guide model behavior without expensive fine-tuning.

- **Provide Default Values:** Documented default values help the model use the tool correctly with less information.