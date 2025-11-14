# Act: Managing System Health and Risk

Observations without action are just expensive dashboards. The "Act" phase is about real-time intervention—the levers you pull to manage the agent's performance, cost, and safety based on what you observe.

Think of "Act" as the system's automated reflexes designed to maintain stability in real-time. In contrast, "Evolve", which will be covered later, is the strategic process of learning from behavior to create a fundamentally better system.

Because an agent is autonomous, you cannot pre-program every possible outcome. Instead, you must build robust mechanisms to influence its behavior in production. These operational levers fall into two primary categories: managing the system's health and managing its risk.

## Managing System Health: Performance, Cost, and Scale

- **Designing for Scale**: Decouple the agent's logic from its state. Use horizontal scaling (stateless, containerized services), asynchronous processing for long-running tasks, and externalized state management.
- **Balancing Competing Goals**: Balance speed (latency), reliability (handling glitches with retries), and cost (shortening prompts, using cheaper models, batching).

## Managing Risk: The Security Response Playbook

When a threat is detected, the response should follow a clear sequence: contain, triage, and resolve.

1.  **Contain**: Immediate containment, typically with a "circuit breaker" (feature flag to disable the affected tool).
2.  **Triage**: Route suspicious requests to a human-in-the-loop (HITL) review queue to investigate the exploit's scope and impact.
3.  **Resolve**: Develop a patch (e.g., updated input filter or system prompt) and deploy it through the automated CI/CD pipeline.