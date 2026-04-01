---
title: "looker-delete-agent Tool"
---

## About

The `looker-delete-agent` tool allows LLMs to delete a Looker Agent using the Looker Go SDK.

## Requirements

To use the `looker-delete-agent` tool, you must define it in your `server.yaml` file.

```yaml
tools:
  - kind: tool
    name: looker-delete-agent
    type: looker-delete-agent
    source: my-looker-instance
    description: "Delete a Looker agent."
```

## Parameters

- `agent_id` (string): The ID of the agent.

## Example

```json
{
  "name": "looker-delete-agent",
  "parameters": {
    "agent_id": "123"
  }
}
```
