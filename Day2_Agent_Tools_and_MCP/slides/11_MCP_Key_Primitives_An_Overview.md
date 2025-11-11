# MCP Key Primitives: An Overview

MCP defines several key concepts, or "capabilities," to structure interactions.

### Server-Side Capabilities (Offered by Server to Client)
1.  **Tools:** Functions the server makes available (e.g., `get_weather`). **This is the most widely supported and core capability.**
2.  **Resources:** Contextual data provided by the server (e.g., a file, a database record).
3.  **Prompts:** Reusable prompt templates related to the server's tools.

### Client-Side Capabilities (Offered by Client to Server)
1.  **Sampling:** Allows a server to request an LLM completion from the client.
2.  **Elicitation:** Allows a server to request additional information from the human user via the client.
3.  **Roots:** Defines filesystem boundaries where a server can operate.

**Adoption Status:** As of late 2025, `Tools` have near-universal support (~99%), while other capabilities have significantly lower adoption rates (4-34%).