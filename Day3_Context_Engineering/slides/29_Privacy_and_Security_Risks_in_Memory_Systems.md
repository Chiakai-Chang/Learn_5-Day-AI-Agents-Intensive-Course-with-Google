# Privacy and Security Risks in Memory

Memories contain user data and require stringent controls.

**Analogy: The Corporate Archivist**
*   The archivist's job is to preserve knowledge while protecting the company.

**Key Safeguards:**
*   **Data Isolation:** Strictly enforce user-level isolation with Access Control Lists (ACLs).
*   **PII Redaction:** Sanitize and redact sensitive personal information *before* it is committed to memory.
*   **Memory Poisoning Prevention:** Validate information to prevent a malicious user from corrupting the agent's knowledge via prompt injection.
*   **Exfiltration Risk Mitigation:** Rigorously anonymize shared memories (like procedural ones) to prevent data leaks.