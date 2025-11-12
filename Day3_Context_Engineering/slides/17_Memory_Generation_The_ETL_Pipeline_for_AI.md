# Memory Generation: The ETL Pipeline for AI

Memory generation is an LLM-driven **ETL (Extract, Transform, Load)** pipeline that turns raw data into structured insights.

**Analogy: The Gardener**
*   A gardener doesn't just throw new seeds (information) onto the plot. They perform **consolidation**—pulling weeds (deleting conflicts), pruning branches (refining memories), and planting new saplings in the right spot.

**High-Level Stages:**
1.  **Ingestion:** Receive raw data (e.g., conversation history).
2.  **Extraction:** Use an LLM to pull out meaningful content based on topic definitions.
3.  **Consolidation:** A "self-editing" process to merge, update, or delete memories to resolve conflicts and deduplicate.
4.  **Storage:** Persist the curated memory to a durable database.