# Critical Challenge: Enterprise Readiness Gaps

While MCP is growing, the core protocol lacks several features critical for enterprise adoption. Organizations must often build these themselves.

- **Authentication and Authorization:** The initial specification lacks a robust, enterprise-ready standard for auth. The current implementation can conflict with modern security practices.

- **Identity Management Ambiguity:** The protocol has no standard way to propagate the end-user's identity. It's often unclear if an action is initiated by the user, the agent, or a system account, which complicates auditing and access control.

- **Lack of Native Observability:** The base protocol doesn't define standards for logging, tracing, or metrics. These are essential for debugging, monitoring, and threat detection.

**Result:** Enterprises are not adopting the "pure" protocol but are wrapping it in layers of centralized governance (e.g., via API gateways) to add the necessary security, identity, and control.