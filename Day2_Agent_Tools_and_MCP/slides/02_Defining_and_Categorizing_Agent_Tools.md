# Defining and Categorizing Agent Tools

### What is a tool?
In AI, a tool is a function or program an LLM-based application uses to accomplish a task outside the model's native capabilities. Tools broadly fit into two categories:
1.  **To Know Something:** Retrieve data for the model to use (e.g., accessing databases, web pages).
2.  **To Do Something:** Perform an action on behalf of the user (e.g., calling an external API, executing code).

### Main Types of Tools
1.  **Function Tools:** Developer-defined external functions that the model can call as needed.
2.  **Built-in Tools:** Tools provided implicitly by the model service (e.g., Google Gemini's built-in Google Search or Code Execution).
3.  **Agent Tools:** An entire agent that is invoked as a tool by another agent, allowing for complex, multi-agent systems.