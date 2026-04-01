---
title: "looker-update-agent Tool"
---

## About

The `looker-update-agent` tool allows LLMs to update an existing Looker Agent using the Looker Go SDK.

## Requirements

To use the `looker-update-agent` tool, you must define it in your `server.yaml` file.

```yaml
tools:
  - kind: tool
    name: looker-update-agent
    type: looker-update-agent
    source: my-looker-instance
    description: "Update a Looker agent."
```

## Parameters

- `agent_id` (string): The ID of the agent.
- `name` (string): The name of the agent.
- `instructions` (string): The instructions (system prompt) for the agent.
- `sources` (array): Optional. A list of JSON-encoded data sources for the agent (e.g., `["{\"model\": \"my_model\", \"explore\": \"my_explore\"}"]`).
- `code_interpreter` (boolean): Optional. Enables Code Interpreter for this Agent.

## Example

```json
{
  "name": "looker-update-agent",
  "parameters": {
    "agent_id": "123",
    "name": "Updated Agent Name"
  }
}
```
