---
title: "looker-list-agents Tool"
---

## About

The `looker-list-agents` tool allows LLMs to list Looker Agents using the Looker Go SDK.

## Requirements

To use the `looker-list-agents` tool, you must define it in your `server.yaml` file.

```yaml
tools:
  - kind: tool
    name: looker-list-agents
    type: looker-list-agents
    source: my-looker-instance
    description: "List all Looker agents."
```

## Parameters

None.

## Example

```json
{
  "name": "looker-list-agents"
}
```
