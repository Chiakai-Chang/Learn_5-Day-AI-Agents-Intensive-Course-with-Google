# Agent Deployment and Production Services

Deployment gives the agent its "body and legs," turning a local prototype into a scalable, reliable service.

- **Core Need:** Agents require services for session history, memory persistence, logging, and security.
- **Deployment Options:**
  - **Standard Infrastructure:** Use Docker containers on runtimes like Cloud Run or GKE for maximum control.
  - **Managed Platforms:** Purpose-built options like Vertex AI Agent Engine simplify deployment and management.
- **Getting Started:** Many frameworks offer simple deploy commands for initial exploration, but production environments require investment in CI/CD and automated testing.