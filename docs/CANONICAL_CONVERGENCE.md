<!--
Copyright © 2026 CrypticNews LLC. All rights reserved.
This provenance header does not replace the repository's applicable license.
-->

# NEXUS Canonical Convergence

**Status:** Architecture baseline / review branch  
**Canonical protocol:** `NexusCryptic/NEXUS_Protocol`  
**Implementation target:** `NexusCryptic/NEXUS_CORE`  
**Public presentation:** `NexusCryptic/NEXUS`  
**Research / artifact lineage:** `NexusCryptic/The-Ledger`

## Purpose

This document establishes a reviewable convergence model for the Living System / GAIA / NEXUS work represented by the connected GitHub repositories and the project documents available in this workspace.

The objective is **convergence without destructive flattening**: preserve repository history and independent artifacts while giving each project a canonical place in one architecture.

## Canonical topology

```text
                              ◈ SOURCE / CANON
                                      │
                         NEXUS_Protocol (contracts)
                                      │
                              NEXUS_CORE (kernel)
                                      │
        ┌─────────────────────────────┼──────────────────────────────┐
        │                             │                              │
   Memory Fabric                 Event Mesh                    Governance
        │                             │                              │
   The-Ledger                 Provider / Tool Bus             Audit Trail
        │                             │                              │
        └─────────────────────────────┼──────────────────────────────┘
                                      │
                              Living System Runtime
                                      │
              ┌───────────────────────┼───────────────────────┐
              │                       │                       │
         GAIA / NEXUS            Cartographer             Dream Engine
              │                       │                       │
        Planetarium / UI        Graph / Topology       Synthesis / Build
              │                       │                       │
              └───────────────────────┼───────────────────────┘
                                      │
                              Public NEXUS Surface
```

## Architectural law

```text
Identity
  ↓
Capability
  ↓
Communication
  ↓
Persistence
  ↓
Telemetry
  ↓
Reflection
  ↓
Governance
  ↓
Convergence
  ↓
◈
```

The root is conceptual and immutable. Implementations may evolve, but every accepted module must expose provenance, capabilities, interfaces, persistence behavior, telemetry, and governance metadata.

## Sector model

| Sector | Canonical responsibility |
|---|---|
| Protocol | Stable contracts, schemas, lifecycle, interoperability |
| Kernel | Scheduling, module loading, runtime state, watchdogs |
| Memory | Append-only history, artifacts, relationships, retrieval |
| Ledger | Evidence, provenance, decisions, change history |
| Cartographer | Repository/project topology and convergence mapping |
| Dream Engine | Decomposition, synthesis, artifact generation |
| Runtime | Browser/PWA/desktop execution and window orchestration |
| Planetarium | Graph visualization, telemetry, node inspection |
| AI Gateway | Provider-neutral model/tool routing |
| Council | Multi-provider analysis and review |
| Storybook | Narrative/workspace representation |
| Signal | Audio/FFT/telemetry stream ingestion and analysis |
| Infrastructure | PXE, recovery, device/network integration |
| Research | Papers, datasets, model references, experimental notes |
| Governance | Permissions, auditability, safety, review gates |

## Repository roles

### Canonical

- `NexusCryptic/NEXUS_Protocol` — normative contracts and architecture.
- `NexusCryptic/NEXUS_CORE` — intended runtime/core implementation target; currently requires replacement of its demonstration scaffold with the canonical implementation through reviewed changes.

### Primary implementation / project surfaces

- `NexusCryptic/NEXUS` — public-facing project surface.
- `machackabook/NEXUS` — private historical/project artifact surface.
- `NexusCryptic/Project-NexusCryptic` — large private project repository; inventory confirms it is accessible to the connected GitHub account, but content inspection was not available during this pass.
- `NexusCryptic/CrypticNEXUS` — project branch/surface.
- `NexusCryptic/NEXUS_Proto` — prototype lineage.
- `NexusCryptic/NEX` — compact project surface.
- `NexusCryptic/Gaia-The-Nexus-Generation` — GAIA project surface.
- `NexusCryptic/Welcome-Sentience` — sentience/runtime-facing project surface.
- `NexusCryptic/The-Ledger` — ledger/provenance surface.

### Excluded from convergence until proven relevant

- `NexusCryptic/demo-repository` — demonstration repository; not treated as a Living System source.
- `NexusCryptic/TOPSecret` — intentionally unclassified because its contents were not inspected; no assumptions are made about its relationship to the canonical system.

No external fork is treated as a canonical branch. External projects may be recorded as dependencies or research references only when explicitly identified as such.

## Convergence rules

1. **Never erase history to create convergence.** Use additive documentation, migrations, and reviewed changes.
2. **Protocol before implementation.** New modules first declare their contract in `NEXUS_Protocol`.
3. **Core consumes contracts.** `NEXUS_CORE` implements protocol-defined interfaces.
4. **Ledger records provenance.** Every migration records source repository, source path, destination path, commit, timestamp, and review status.
5. **Public surfaces contain publishable material only.** Credentials, tokens, private keys, personal addresses, and other secrets never enter the convergence corpus.
6. **Forks remain distinguishable.** A derived or external repository is never relabeled as original project work.
7. **Generated artifacts are labeled.** AI-generated documentation/code is identified as generated and remains reviewable.
8. **Human approval remains the release gate.** Automated analysis may recommend changes; release-quality changes require review.

## Review sequence

```text
Inventory
  → Classify
  → Map lineage
  → Extract artifacts
  → Normalize metadata
  → Validate licenses
  → Detect secrets
  → Generate documentation
  → Implement contracts
  → Test
  → Review
  → Merge
```

## Source limitations

This baseline is based on the connected GitHub inventory, repositories/files that were readable through the GitHub connection, and the project documents available in this workspace. It is **not** a claim that every conversation, local filesystem artifact, private service, or historical repository outside those sources has been exhaustively recovered.
