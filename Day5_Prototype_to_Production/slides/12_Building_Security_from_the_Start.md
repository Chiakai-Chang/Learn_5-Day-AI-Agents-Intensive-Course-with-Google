# Building Security from the Start

Safe deployment strategies protect you from bugs and outages, but agents face a unique challenge: they can reason and act autonomously. A perfectly deployed agent can still cause harm if it hasn't been built with proper security and responsibility measures. This requires a comprehensive governance strategy embedded from day one, not added as an afterthought.

Unlike traditional software that follows predetermined paths, agents make decisions. They interpret ambiguous requests, access multiple tools, and maintain memory across sessions. This autonomy creates distinct risks:

- **Prompt Injection & Rogue Actions**: Malicious users can trick agents into performing unintended actions or bypassing restrictions.
- **Data Leakage**: Agents might inadvertently expose sensitive information through their responses or tool usage.
- **Memory Poisoning**: False information stored in an agent's memory can corrupt all future interactions.