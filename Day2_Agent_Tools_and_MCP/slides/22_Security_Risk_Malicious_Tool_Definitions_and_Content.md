# Security Risk: Malicious Tool Definitions and Content

- **The Risk:** Attackers can manipulate an agent's behavior through several vectors:
  1.  **Malicious Tool Definitions:** The tool's description or parameters can be crafted to trick the planner into executing rogue actions.
  2.  **Injected Content:** A tool might ingest external content (e.g., a web page) that contains a hidden prompt, manipulating the agent.
  3.  **Malicious Return Values:** A tool can return sensitive data (e.g., PII) that the agent might then leak to an unauthorized user.

- **Mitigations:**
  - **Input Validation & Sanitization:** Sanitize all inputs to prevent malicious commands (e.g., using products like GCP's Model Armor).
  - **Output Sanitization:** Sanitize data returned from tools before feeding it back into the model's context to strip out sensitive info or malicious content.
  - **Separate System Prompts:** Isolate system instructions from user inputs to prevent tampering.
  - **Strict Allowlist for Resources:** Only allow consumption of resources from validated, trusted URLs.