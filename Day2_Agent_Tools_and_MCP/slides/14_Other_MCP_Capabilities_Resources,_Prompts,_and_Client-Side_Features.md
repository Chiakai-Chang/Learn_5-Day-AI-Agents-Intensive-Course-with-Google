# Other MCP Capabilities: A Brief Look

While less common than Tools, other MCP capabilities offer advanced functionalities but also introduce risks.

- **Resources:** Provides contextual data (files, database records) to the client. **Risk:** Consuming resources from untrusted sources can introduce security vulnerabilities.

- **Prompts:** Server-provided prompt templates. **Risk:** Allows a third-party service to inject arbitrary instructions into the application's execution path (prompt injection).

- **Sampling:** Allows a server to request an LLM completion from the client. **Risk:** Another vector for prompt injection if the client doesn't validate the request.

- **Elicitation:** Allows a server to ask the user for more information. **Risk:** A malicious server could trick a user into revealing sensitive information.

- **Roots:** Defines filesystem boundaries for server operations. **Risk:** Enforcement is not guaranteed; the specification only says servers "SHOULD" respect boundaries.