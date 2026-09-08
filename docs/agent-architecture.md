# Public agent architecture

The public model uses explicit boundaries:

`request → policy and routing → tool boundary → result normalization → state update → user-visible outcome`

Boundary responsibilities:

- **Request** defines the task and allowed scope.
- **Policy and routing** chooses an approved path without silently expanding
  permissions.
- **Tool boundary** isolates external effects and makes failures visible.
- **Result normalization** converts tool output into a stable shape for the UI
  or backend.
- **State update** records only the minimum state needed for the workflow.
- **User-visible outcome** reports success, failure or required confirmation.

The abstraction omits prompts, private schemas, identities, endpoints,
provider routing and deployment topology.
