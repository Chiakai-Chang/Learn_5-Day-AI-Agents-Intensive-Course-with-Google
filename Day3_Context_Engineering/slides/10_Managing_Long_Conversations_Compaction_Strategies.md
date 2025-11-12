# Managing Long Conversations: Compaction

**Problem:** As conversation history grows, it hits limits and increases cost, latency, and noise.

**Analogy: Packing a Suitcase**
*   You can't stuff everything in; it becomes heavy and disorganized.
*   You can't pack too little; you'll miss essential items.
*   Success hinges on carrying *only what you need*.

**Compaction Strategies:**
*   **Keep Last N Turns:** A simple "sliding window."
*   **Token-Based Truncation:** Cut off older messages once a token limit is reached.
*   **Recursive Summarization:** Replace older parts of the conversation with an AI-generated summary.