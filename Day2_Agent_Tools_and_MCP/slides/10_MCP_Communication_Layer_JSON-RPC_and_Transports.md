# MCP Communication Layer: JSON-RPC and Transports

All communication in MCP is built on a standardized technical foundation.

- **Base Protocol: JSON-RPC 2.0**
  - A lightweight, text-based, and language-agnostic format for all messages.
  - Defines four message types: `Requests`, `Results`, `Errors`, and `Notifications`.

- **Transport Protocols**
  - MCP defines standard protocols for how clients and servers exchange messages.
  1.  **stdio (Standard I/O):** Used for fast, local communication where the server is a subprocess of the Host (e.g., for accessing the local filesystem).
  2.  **Streamable HTTP:** The recommended protocol for remote client-server connections, supporting streaming responses.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-11/f841a90f-9dc4-4239-8ad6-f1b12708962f/a352164d8f92915bb0868eaf77ed6e787eb0e3d689de4448ee817eee66760b26.jpg)