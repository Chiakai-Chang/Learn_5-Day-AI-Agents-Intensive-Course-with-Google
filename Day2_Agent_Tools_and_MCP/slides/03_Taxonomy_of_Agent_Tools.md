# Taxonomy of Agent Tools

Agent tools can be categorized by their primary function:

- **Information Retrieval:** Fetch data from sources like web searches, databases, or documents.
- **Action / Execution:** Perform real-world operations like sending emails, posting messages, or controlling devices.
- **System / API Integration:** Connect with existing software systems, enterprise workflows, or third-party services.
- **Human-in-the-Loop:** Facilitate collaboration with users, such as asking for clarification or seeking approval for critical actions.

| Tool Category | Use Case | Key Design Tips |
| :--- | :--- | :--- |
| **Structured Data Retrieval** | Querying databases, spreadsheets (e.g., NL2SQL) | Define clear schemas, optimize for efficient querying. |
| **Unstructured Data Retrieval** | Searching documents, web pages (e.g., RAG) | Implement robust search, consider context window limits. |
| **Google Connectors** | Interacting with Google Workspace apps (Gmail, Drive) | Leverage Google APIs, ensure proper auth, handle rate limits. |
| **Third-Party Connectors** | Integrating with external services (e.g., Jira, Slack) | Document external APIs, manage keys securely, implement error handling. |