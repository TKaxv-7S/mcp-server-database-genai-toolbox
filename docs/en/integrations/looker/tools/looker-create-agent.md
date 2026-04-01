---
title: "looker-create-agent Tool"
---

## About

The `looker-create-agent` tool allows LLMs to create a Looker Agent using the Looker Go SDK.

## Requirements

To use the `looker-create-agent` tool, you must define it in your `server.yaml` file.

```yaml
tools:
  - kind: tool
    name: looker-create-agent
    type: looker-create-agent
    source: my-looker-instance
    description: "Create a new Looker agent."
```

## Parameters

- `name` (string): The name of the agent.
- `instructions` (string): The instructions (system prompt) for the agent.
- `sources` (array): Optional. A list of JSON-encoded data sources for the agent (e.g., `["{\"model\": \"my_model\", \"explore\": \"my_explore\"}"]`).
- `code_interpreter` (boolean): Optional. Enables Code Interpreter for this Agent.

## Example

```json
{
  "name": "looker-create-agent",
  "parameters": {
    "name": "My Agent",
    "instructions": "You are a helpful assistant.",
    "sources": ["{\"model\": \"my_model\", \"explore\": \"my_explore\"}"],
    "code_interpreter": true
  }
}
```
