# CI/CD Stages: Pre-Merge, Staging, and Production

1.  **Phase 1: Pre-Merge Integration (CI)**. Provides rapid feedback to the AI Engineer or Prompt Engineer. Runs fast checks like unit tests, code linting, dependency scanning, and crucially, the agent quality evaluation suite. Catches issues before they pollute the main branch.
2.  **Phase 2: Post-Merge Validation in Staging (CD)**. Once a change passes all CI checks and is merged, the focus shifts to operational readiness. The CD process deploys the agent to a staging environment (a high-fidelity replica of production). Here, comprehensive tests like load testing and integration tests are run, along with internal user testing ("dogfooding").
3.  **Phase 3: Gated Deployment to Production**. After thorough validation in staging, the final step is deploying to production. This is almost never fully automatic, typically requiring a Product Owner's final sign-off. The exact deployment artifact validated in staging is promoted to production with appropriate safeguards.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-14/b1a68d18-4646-4f28-8873-68da9fe1ef9b/64f6db80e0da0c15165f956712e2e7c682f05849b9f6a65a39073eec835983e5.jpg)
Figure 3: Different stages of the CI/CD process

This three-phase CI/CD workflow requires robust automation infrastructure and proper secrets management. This automation is powered by:

- **Infrastructure as Code (IaC)**: Tools like Terraform define environments programmatically, ensuring they are identical, repeatable, and version-controlled.
- **Automated Testing Frameworks**: Frameworks like Pytest execute tests and evaluations at each stage, handling agent-specific artifacts.

Sensitive information like API keys should be managed securely using a service like Secret Manager and injected at runtime, rather than being hardcoded.