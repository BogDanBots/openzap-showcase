# OpenZap — architecture case study

OpenZap is a case study of a local-first agentic platform with modular
routing, tool execution, a web/backend surface and experimentation around
on-chain memory. The production repository remains private.

## What this case study covers

- separating routing, policy and tool-execution boundaries;
- normalizing tool results for a web/backend surface;
- keeping local state and external side effects explicit;
- treating on-chain memory as a bounded coordination concept rather than a
  hidden context store;
- designing failure handling and observability into agent workflows.

The public repository contains documentation-only abstractions. It does not
publish prompts, memory records, user context, identity data, credentials,
private endpoints, operational logs or production implementation.
