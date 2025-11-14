# Evolve: Learning and Improving from Production Data

While the "Act" phase provides the system's immediate, tactical reflexes, the "Evolve" phase is about long-term, strategic improvement. It begins by looking at the patterns and trends collected in your observability data and asking a crucial question: "How do we fix the root cause so this problem never happens again?"

This is where you move from reacting to production incidents to proactively making your agent smarter, more efficient, and safer. You turn the raw data from the "Observe" phase into durable improvements in your agent's architecture, logic, and behavior.

## The Engine of Evolution: An Automated Path to Production

An insight from production is only valuable if you can act on it quickly. This is where the automated CI/CD pipeline you built in pre-production becomes the most critical component of your operational loop. A fast, reliable path to production allows you to close the loop between observation and improvement in hours or days, not weeks or months.

When you identify a potential improvement, the process should be:

1.  **Commit the Change**: The proposed improvement is committed to your version-controlled repository.
2.  **Trigger Automation**: The commit automatically triggers your CI/CD pipeline.
3.  **Validate Rigorously**: The pipeline runs the full suite of unit tests, security scans, and the agent quality evaluation suite against your updated datasets.
4.  **Deploy Safely**: Once validated, the change is deployed to production using a safe rollout strategy.

This automated workflow transforms evolution from a slow, high-risk manual project into a fast, repeatable, and data-driven process.

## The Evolution Workflow: From Insight to Deployed Improvement

1.  **Analyze Production Data**: Identify trends in user behavior, task success rates, and security incidents from production logs.
2.  **Update Evaluation Datasets**: Transform production failures into tomorrow's test cases, augmenting your golden dataset.
3.  **Refine and Deploy**: Commit improvements to trigger the automated pipeline—whether refining prompts, adding tools, or updating guardrails.

This creates a virtuous cycle where your agent continuously improves with every user interaction.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-14/b1a68d18-4646-4f28-8873-68da9fe1ef9b/7b2536b978d5c42e3ab021ea27e430dff06dc25da9aec13f6ff52b24c079566e.jpg)