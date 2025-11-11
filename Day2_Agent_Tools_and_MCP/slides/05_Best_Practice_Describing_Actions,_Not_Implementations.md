# Best Practice: Describing Actions, Not Implementations

Your instructions to the model should focus on the goal, not the specific tool to achieve it. This prevents conflicts and allows for dynamic tool use.

### Key Principles:

- **Describe *What*, Not *How***
  - **Good:** "Create a bug to describe the issue."
  - **Bad:** "Use the `create_bug` tool."

- **Don't Duplicate Instructions**
  - Avoid restating the tool's documentation in the prompt. This can confuse the model and creates a maintenance burden.

- **Don't Dictate Workflows**
  - Describe the final objective and let the model determine the sequence of tool calls autonomously.

- **DO Explain Tool Interactions**
  - If one tool has a side effect that impacts another (e.g., a `fetch_web_page` tool saves a file), document this interaction so the agent knows how to access the result.