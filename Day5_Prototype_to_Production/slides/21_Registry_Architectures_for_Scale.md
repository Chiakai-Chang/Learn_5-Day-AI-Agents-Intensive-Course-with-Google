# Registry Architectures: When and How to Build Them

Why do some organizations build registries while others don't need them? The answer lies in scale and complexity. When you have fifty tools, manual configuration works fine. But when you reach five thousand tools distributed across different teams and environments, you face a discovery problem that demands a systematic solution.

A **Tool Registry** uses a protocol like MCP to catalog all assets, from functions to APIs. Instead of giving agents access to thousands of tools, you create curated lists, leading to three common patterns:

- **Generalist agents**: Access the full catalog, trading speed and accuracy for scope.
- **Specialist agents**: Use predefined subsets for higher performance.
- **Dynamic agents**: Query the registry at runtime to adapt to new tools.

The primary benefit is human discovery—developers can search for existing tools before building duplicates, security teams can audit tool access, and product owners can understand their agents' capabilities.

An **Agent Registry** applies the same concept to agents, using formats like A2A's AgentCards. It helps teams discover and reuse existing agents, reducing redundant work. This also lays the groundwork for automated agent-to-agent delegation, though this remains an emerging pattern.

Registries offer discovery and governance at the cost of maintenance. You can consider starting without one and only build it when your ecosystem's scale demands centralized management!

## Decision Framework for Registries

- **Tool Registry**: Build when tool discovery becomes a bottleneck or security requires centralized auditing.
- **Agent Registry**: Build when multiple teams need to discover and reuse specialized agents without tight coupling.