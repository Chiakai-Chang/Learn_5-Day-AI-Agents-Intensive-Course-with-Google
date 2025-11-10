# Agent Identity and Policy Enforcement

- **Agents as a New Principal:** An agent is an autonomous actor, not just code. It requires its own verifiable identity, distinct from its user and developer.
  - **Authentication (AuthN):** Standards like SPIFFE can provide a cryptographically verifiable "digital passport" for each agent.
- **Principle of Least Privilege:** Once an agent has an identity, it can be granted specific, minimal permissions (e.g., SalesAgent can access the CRM, but HRonboardingAgent cannot).
- **Policy Enforcement (AuthZ):** Policies are rules that constrain an agent's capabilities, limiting access to specific tools, data, and other agents to only what is required for its job.