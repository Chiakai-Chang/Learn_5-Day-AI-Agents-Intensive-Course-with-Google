# Best Practice: Granularity, Concise Output, and Validation

- ### Make Tools Granular
  - Follow the single-responsibility principle. Each tool should have one clear, well-documented purpose.
  - Avoid creating "multi-tools" that encapsulate long, complex workflows, as they are hard for LLMs to use consistently.

- ### Design for Concise Output
  - Large responses (data tables, files, images) bloat the context window, increasing cost and latency.
  - Instead of returning large data payloads, use external systems. For example, save a large query result to a temporary database and return the table name.

- ### Use Validation Effectively
  - Use schema validation for tool inputs and outputs wherever possible.
  - Schemas serve as both documentation for the LLM and a run-time check to ensure the tool is being called correctly.