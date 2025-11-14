# Core Challenges of Agentic Systems

Deploying agentic systems introduces a new class of challenges that require an evolution in our operational discipline. Unlike traditional ML models, agents are autonomously interactive, stateful, and follow dynamic execution paths.

This creates unique operational headaches that demand specialized strategies:

- **Dynamic Tool Orchestration**: An agent's "trajectory" is assembled on the fly as it picks and chooses tools. This requires robust versioning, access control, and observability for a system that behaves differently every time.
- **Scalable State Management**: Agents can remember things across interactions. Managing session and memory securely and consistently at scale is a complex systems design problem.
- **Unpredictable Cost & Latency**: An agent can take many different paths to find an answer, making its cost and response time incredibly hard to predict and control without smart budgeting and caching.