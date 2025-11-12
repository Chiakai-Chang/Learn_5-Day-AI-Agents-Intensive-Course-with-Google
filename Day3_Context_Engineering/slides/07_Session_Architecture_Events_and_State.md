# Session Architecture: Events and State

Every session contains two key components:

1.  **Events (Chronological History):**
    *   The building blocks of the conversation, logged in order.
    *   **Types:** User Input, Agent Response, Tool Call, Tool Output.
    *   Analogous to the list of `Content` objects passed to the Gemini API.

2.  **State (Working Memory):**
    *   A structured "scratchpad" holding temporary data relevant to the current conversation.
    *   Example: Items in a shopping cart.