# Deep-dive: Memory Extraction

**Goal: What information is meaningful enough to become a memory?**

*   "Meaningful" is defined by the agent's specific use case.
*   The memory manager's LLM uses a system prompt with **topic definitions** to guide extraction.

**Extraction Methods:**
*   **Schema-based:** The LLM fills a predefined JSON schema using information from the conversation.
*   **Natural Language Topics:** The LLM is guided by a simple text description of the topic.
*   **Few-shot Prompting:** The LLM is "shown" what to extract through examples of input text and the ideal output memory.