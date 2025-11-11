# Critical Challenge: Performance and Scalability

- ### Context Window Bloat
  A primary challenge is that the definitions and schemas for **every** available tool must be included in the model's context window. This metadata can consume a significant portion of the token limit.
  - **Impact:** Increased cost, higher latency, and loss of other critical context (like conversation history).

- ### Degraded Reasoning Quality
  An overloaded context window can confuse the model. With too many tool definitions, the AI may struggle to identify the correct tool or lose track of the user's original intent, leading to erratic behavior.

- ### The Future: Dynamic Tool Retrieval
  This scaling problem may force a shift to a RAG-like approach for tool discovery, where an agent first performs a "tool retrieval" search to find the most relevant tools before loading only their definitions into the context.