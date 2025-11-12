# The Context Engineering Lifecycle

A continuous cycle for each turn of a conversation:

1.  **Fetch Context:**
    *   Retrieve user memories, RAG documents, and recent conversation events.

2.  **Prepare Context:**
    *   Dynamically construct the full prompt for the LLM. This is a blocking, "hot-path" process.

3.  **Invoke LLM and Tools:**
    *   Iteratively call the LLM and any necessary tools to generate a response.

4.  **Upload Context:**
    *   Asynchronously upload new information (e.g., new memories) to persistent storage in the background.