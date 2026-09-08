# On-chain memory concepts

On-chain memory can be described as a bounded coordination layer for durable references, commitments or workflow state. It should not be presented as a dump of private agent context or as a substitute for access control.

## Design questions

- What state is genuinely durable and why does it need chain-level persistence?
- Which values are public, encrypted, hashed or kept entirely off-chain?
- Who can create, update or invalidate a reference?
- How are stale records, replay and recovery handled?
- What does the user sign, and what remains an application-side decision?

## Deliberate limits

This showcase does not publish the production protocol, serialization, wallet identities, deployment details, memory records or cryptographic implementation. It presents the design questions and trust boundaries only.
