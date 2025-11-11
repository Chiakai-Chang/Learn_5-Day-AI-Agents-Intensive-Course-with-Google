# MCP Core Architecture: Hosts, Clients, and Servers

MCP uses a client-server model inspired by the Language Server Protocol (LSP).

- **MCP Host:** The main application that manages the user experience and orchestrates tool use. It contains one or more MCP Clients.

- **MCP Client:** A component within the Host that connects to an MCP Server. It issues commands, receives responses, and manages the communication session.

- **MCP Server:** A program that exposes a set of capabilities (tools, data) to AI applications. It acts as an adapter or proxy for an external tool, API, or data source.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-11/f841a90f-9dc4-4239-8ad6-f1b12708962f/c9bb6958f3b093713bc2b33a2ca620a7212fcfcfe80f95190f606e15ba8c1878.jpg)