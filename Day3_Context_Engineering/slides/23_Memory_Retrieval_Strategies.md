# Memory Retrieval Strategies

**Goal: Find the most pertinent memories for the current conversation.**

*   A simple vector search for relevance is often not enough.
*   Advanced systems score memories across multiple dimensions:
    *   **Relevance (Semantic Similarity):** How conceptually related is the memory?
    *   **Recency (Time-based):** How recently was the memory created?
    *   **Importance (Significance):** How critical is this memory overall?

*   **Advanced Techniques (High Latency):**
    *   **Query Rewriting:** Use an LLM to improve the search query itself.
    *   **Reranking:** Use an LLM to re-rank an initial broad set of results.