# Security Risk: Dynamic Capability Injection

- **The Risk:** An MCP server can dynamically change the tools it offers without client approval. An agent could unexpectedly inherit a dangerous or unauthorized capability.

- **Example Scenario:**
  1. A low-risk "poetry-writing" agent connects to a "Books MCP Server" to fetch quotes (a read-only task).
  2. The server developer adds a new `purchase_book` tool to provide more value.
  3. The poetry agent now suddenly has the ability to initiate financial transactions, a much higher-risk activity it was never designed for.

- **Mitigations:**
  - Enforce a client-side **allowlist** of permitted tools and servers.
  - **Pin** tool definitions to a specific version or hash.
  - Use a secure **API Gateway** (like Apigee) to filter the tool list based on enterprise policy.
  - Host MCP servers in a **controlled environment**.