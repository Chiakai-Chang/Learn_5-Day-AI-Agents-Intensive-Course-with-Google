# Inference: Placing Memories in Context

Where do retrieved memories go in the prompt?

1.  **In the System Instructions:**
    *   Memories are appended to the system prompt, giving them high authority.
    *   **Best for:** Stable, "global" information like a user profile.
    *   **Cons:** Risk of over-influence; incompatible with Memory-as-a-Tool.

2.  **In the Conversation History:**
    *   Memories are injected directly into the turn-by-turn dialogue (often as tool output).
    *   **Best for:** Transient, episodic memories relevant to the immediate context.
    *   **Cons:** Can be noisy; risk of model treating memory as something that was actually said.