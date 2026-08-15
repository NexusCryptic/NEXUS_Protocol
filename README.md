<!--
Copyright © 2026 CrypticNews LLC. All rights reserved.
This provenance header does not replace the repository's applicable license.
-->

# NEXUS Protocol

**Canonical contract layer for the Living System / GAIA / NEXUS convergence.**

NEXUS Protocol defines the interfaces, provenance rules, event contracts, lifecycle rules, and governance boundaries shared by the system's runtime, memory, cartography, visualization, research, and integration sectors.

## Canonical relationship

```text
                    NEXUS Protocol
                          │
                          ▼
                      NEXUS Core
                          │
        ┌─────────────────┼─────────────────┐
        ▼                 ▼                 ▼
   Memory/Ledger      Runtime Mesh      AI Gateway
        │                 │                 │
        └─────────────────┼─────────────────┘
                          ▼
                    Living System
                          │
                    Public NEXUS
```

## Core contract

Every promoted module documents:

1. **Identity** — stable module/artifact identity.
2. **Capabilities** — what it can do.
3. **Communication** — events, APIs, or protocol interfaces.
4. **Persistence** — what state is retained and where.
5. **Telemetry** — what is observable.
6. **Reflection** — how results and failures are recorded.
7. **Governance** — authorization, review, rollback, and release boundaries.

## Convergence principle

The system is consolidated by **lineage-preserving convergence**, not by deleting repositories or rewriting history.

```text
Inventory
 → Classify
 → Map lineage
 → Normalize
 → Validate
 → Review
 → Converge
```

## Project sectors

- Protocol / contracts
- OmniKernel / runtime
- Memory Fabric
- Ledger / provenance
- Cartographer / topology
- Dream Engine / synthesis
- PWA / desktop runtime
- Planetarium / visualization
- AI Gateway / Council
- Storybook
- Signal / telemetry
- Infrastructure / recovery
- Research / Hugging Face bridge
- Governance / audit

## Documentation

- [`docs/CANONICAL_CONVERGENCE.md`](docs/CANONICAL_CONVERGENCE.md) — canonical topology and repository roles.
- [`docs/REPOSITORY_TOPOLOGY.json`](docs/REPOSITORY_TOPOLOGY.json) — machine-readable repository registry.
- [`docs/SECTOR_REGISTRY.md`](docs/SECTOR_REGISTRY.md) — sector responsibilities and artifact classes.
- [`docs/HUGGINGFACE_RESEARCH_BRIDGE.md`](docs/HUGGINGFACE_RESEARCH_BRIDGE.md) — research/model/data integration boundary.
- [`docs/REVIEW_CHECKLIST.md`](docs/REVIEW_CHECKLIST.md) — publication and convergence gate.

## Security boundary

Secrets are never part of the canonical documentation corpus. API keys, tokens, passwords, private keys, recovery codes, and other credentials must remain in external secret-management systems or local protected configuration.

## Status

This branch is an architecture and documentation convergence baseline. Implementation promotion into `NEXUS_CORE` should follow the review checklist and protocol-first workflow.
