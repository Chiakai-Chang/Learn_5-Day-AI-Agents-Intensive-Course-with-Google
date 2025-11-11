# Deep Dive: MCP Tool Definition and Schema

The `Tool` is the core entity in MCP. Its definition must conform to a specific JSON schema.

### Key Fields in a Tool Definition:
- **`name`**: A unique identifier for the tool (e.g., `get_stock_price`).
- **`title`**: (Optional but recommended) A human-readable name.
- **`description`**: A human- and LLM-readable description of what the tool does. **Crucial for the model's reasoning.**
- **`inputSchema`**: A JSON schema defining the tool's expected input parameters.
- **`outputSchema`**: (Optional but recommended) A JSON schema defining the structure of the tool's output.
- **`annotations`**: (Optional) Hints about the tool's behavior (e.g., `readOnlyHint`, `destructiveHint`). These are not guaranteed and should be used with caution.