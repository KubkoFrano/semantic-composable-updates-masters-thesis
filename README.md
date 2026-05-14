# Semantic, composable updates for asynchronous application state

**Student:** Jakub Fraňo
**Supervisor:** RNDr. Jozef Šiška, PhD.

## Overview
Modern applications rely on asynchronous communication, optimistic local updates, and partial data loading. Traditional protocols that send full-state snapshots or opaque setters are inefficient and complicate merging changes.

Conflict-Free Replicated Data Types (CRDTs) offer a theoretical foundation for commutative, idempotent updates that can be applied without full state knowledge. However, existing CRDT approaches assume fully replicated peers and often generate large metadata, making them less practical for centralized servers or partial replicas.
By representing changes as meaningful operations rather than opaque states, such a protocol allows clients to apply updates optimistically, supports server-side merging and compression of operations, reduces bandwidth, and enables partial or lazy loading of state.

## Goal
Design a protocol for semantic, composable updates that supports optimistic local updates, server-side update compression, and lazy loading and study its properties compared to other solutions.

## Technical pillars
- operation-based changes
- client-server architecture
- **semantic compression**
- path-based substriptions

## Calendar
| Date Range | Phase | Milestone / Task |
| :--- | :--- | :--- |
| **Mar 16 – Mar 22** | Research | Existing solutions and synchronization approaches |
| **Mar 23 – Mar 29** | Research | Operational Transformation (OT) |
| **Mar 30 – Apr 05** | Research | Conflict-Free Replicated Data Types (CRDTs) |
| **Apr 06 – Apr 12** | Concept | Problem definition and solution proposal |
| **Apr 13 – Apr 19** | Modeling | Formal model and protocol brainstorming |
| **Apr 20 – Apr 26** | Development | Design a prototype; decide on frameworks & libraries |
| **Apr 27 – May 03** | Validation | Brainstorming validation strategies |
| **May 04 – May 10** | Conclusion | LaTeX setup & final presentation |

## TODO
- Define formal model
- Define protocol
- Implement prototype
- Test