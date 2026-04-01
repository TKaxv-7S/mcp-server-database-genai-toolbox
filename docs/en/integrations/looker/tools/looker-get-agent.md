---
title: "looker-get-agent Tool"
---

## About

The `looker-get-agent` tool allows LLMs to retrieve a specific Looker Agent by ID using the Looker Go SDK.

## Requirements

To use the `looker-get-agent` tool, you must define it in your `server.yaml` file.

```yaml
tools:
  - kind: tool
    name: looker-get-agent
    type: looker-get-agent
    source: my-looker-instance
    description: "Retrieve a Looker agent."
```

## Parameters

- `agent_id` (string): The ID of the agent.

## Example

```json
{
  "name": "looker-get-agent",
  "parameters": {
    "agent_id": "123"
  }
}
```
