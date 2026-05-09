---
title: "Securing MCP: A Control Plane for Agent Tool Execution"
url: "https://devblogs.microsoft.com/blog/securing-mcp-a-control-plane-for-agent-tool-execution"
date: "2026-04-22"
author: "Jack Batzner"
feed_url: "https://devblogs.microsoft.com/feed/"
---
The Model Context Protocol (MCP) is quickly becoming a common way for AI agents to discover and use tools. It provides a consistent interface to databases, APIs, file systems, and third-party services, which makes it easier to plug capabilities into agent workflows. However, MCP standardizes the execution surface without defining how that surface should be governed. Tool definitions are fed directly to the model, tool servers can be hosted by anyone, and there is no built-in point where policy is evaluated before a call is executed.
