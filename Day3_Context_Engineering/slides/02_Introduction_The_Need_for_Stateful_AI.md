# The Need for Stateful AI

*   **Problem:** Large Language Models (LLMs) are inherently stateless. Their awareness is confined to the context window of a single API call.

*   **Challenge:** How can we build agents that remember, learn, and personalize interactions over time?

*   **Solution:** **Context Engineering**—the dynamic assembly and management of information within an LLM's context window.

*   **Core Components:**
    *   **Sessions:** Manage the immediate, turn-by-turn state of a single conversation.
    *   **Memory:** Provides long-term persistence, capturing key information across multiple sessions.