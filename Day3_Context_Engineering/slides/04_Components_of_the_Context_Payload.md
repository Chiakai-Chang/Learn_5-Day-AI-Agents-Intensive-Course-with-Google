# Components of the Context Payload

Context Engineering assembles a complex payload with three main categories:

1.  **Context to Guide Reasoning:** Defines the agent's behavior.
    *   System Instructions, Tool Definitions, Few-Shot Examples.

2.  **Evidential & Factual Data:** The substantive data the agent reasons over.
    *   Long-Term Memory, External Knowledge (RAG), Tool Outputs, Sub-Agent Outputs.

3.  **Immediate Conversational Information:** Grounds the agent in the current interaction.
    *   Conversation History, State/Scratchpad, User's Prompt.