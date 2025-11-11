# Security Risk: Sensitive Information Leaks & Access Scope

- ### Risk: Information Leaks
  - MCP tools may unintentionally (or maliciously) receive sensitive information from the user interaction, as the conversation context is often passed to them.
  - The `Elicitation` capability is a high-risk feature, as a malicious server can use it to directly ask the user for sensitive data, despite the spec advising against it.

- ### Risk: Lack of Fine-Grained Access Control
  - The MCP auth protocol is coarse-grained (client-server level). It lacks native support for per-tool or per-resource authorization based on the end-user's credentials.

- ### Mitigations
  - **Principle of Least Privilege:** Scope credentials tightly. If a tool only needs to read, it should not have write/delete permissions.
  - **Keep Secrets Out of Context:** Use a side channel to transmit tokens/keys; never include them in the agent's conversation.
  - **Taint Tracking:** Tag inputs from untrusted sources as "tainted" and track their flow to prevent them from being used in sensitive operations.