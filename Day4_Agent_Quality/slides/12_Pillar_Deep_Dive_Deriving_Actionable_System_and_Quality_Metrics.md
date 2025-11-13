# 12: Pillar Deep Dive: Actionable Metrics

Metrics are the aggregated scorecard of agent performance, derived from logs and traces. They are divided into two key categories.

## 1. System Metrics: The Vital Signs

Directly measurable, quantitative indicators of operational health.

*   **Performance:** Latency (P50/P99), Error Rate
*   **Cost:** Tokens per Task, API Cost per Run
*   **Effectiveness:** Task Completion Rate, Tool Usage Frequency

## 2. Quality Metrics: Judging the Decision-Making

Second-order metrics derived by applying judgment frameworks (from Chapter 2) to the observability data.

*   **Correctness & Accuracy:** Was the answer factually correct?
*   **Trajectory Adherence:** Did the agent follow the ideal path?
*   **Safety & Responsibility:** Did the response avoid harmful content?
*   **Helpfulness & Relevance:** Was the response actually helpful?