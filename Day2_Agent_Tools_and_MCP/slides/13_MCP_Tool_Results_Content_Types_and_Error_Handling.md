# MCP Tool Results: Content Types and Error Handling

### Content Types
Tools can return results in various formats:
- **Unstructured Content:**
  - `Text`: Plain string data.
  - `Audio`/`Image`: Base64-encoded data with a MIME type.
  - `Resource`: A link to or embedded data for a larger resource (e.g., a file).
- **Structured Content:**
  - Always a JSON object. Should be validated against the tool's `outputSchema`.

### Error Handling
MCP defines two standard error mechanisms:
1.  **Protocol Errors (JSON-RPC):** For issues like an unknown tool or invalid arguments. The server returns a standard JSON-RPC error object.
2.  **Tool Execution Errors:** For failures within the tool itself (e.g., a backend API fails). The server returns a result object with the `"isError": true` parameter set. This channel can be used to provide helpful failure guidance to the LLM.