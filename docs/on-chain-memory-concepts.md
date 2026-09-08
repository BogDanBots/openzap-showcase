# On-chain memory: design boundaries

In this case study, on-chain memory is a bounded coordination layer for
durable references, commitments or workflow state. It is not a dump of private
agent context and it does not replace access control.

The design is evaluated against these questions:

- What state is genuinely durable, and why does it need chain-level
  persistence?
- Which values are public, encrypted, hashed or kept entirely off-chain?
- Who can create, update or invalidate a reference?
- How are stale records, replay and recovery handled?
- What does the user sign, and what remains an application-side decision?

This showcase omits the production protocol, serialization, wallet
identities, deployment details, memory records and cryptographic
implementation. It presents the design constraints and trust boundaries.
