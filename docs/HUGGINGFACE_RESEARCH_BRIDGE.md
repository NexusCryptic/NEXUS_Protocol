<!--
Copyright © 2026 CrypticNews LLC. All rights reserved.
This provenance header does not replace the repository's applicable license.
-->

# Hugging Face Research Bridge

## Connected identity

The connected Hugging Face integration currently authenticates as `machackabook`.

The available credential scope is read-oriented for Hub repositories and MCP discovery, with Jobs access also present. The integration does not currently expose a write/publish scope for project repositories.

## Role in the Living System

Hugging Face is treated as a **research and model/data discovery boundary**, not as a second canonical source tree.

```text
NEXUS_Protocol
      │
      ├── defines contracts
      │
      └── Research Bridge
             │
             ├── Models
             ├── Datasets
             ├── Spaces
             └── Papers
```

## Provenance rule

An external model, dataset, Space, or paper may be referenced by the Living System only with enough metadata to reproduce the reference:

- provider
- repository ID or paper identifier
- task/domain
- version or revision when available
- license
- source URL
- reason for inclusion
- validation status

External artifacts are **not** silently reclassified as GAIA/NEXUS-originated work.

## Research sectors

### Model Registry

Track models considered for:

- local inference
- provider fallback
- embedding/retrieval
- vision
- audio/signal analysis
- code generation
- classification

### Dataset Registry

Track datasets used for:

- evaluation
- retrieval experiments
- graph construction
- document processing
- telemetry analysis

### Paper Registry

Track research relevant to:

- agent orchestration
- memory systems
- graph retrieval
- multimodal systems
- local-first runtimes
- browser execution
- WebGPU
- software evolution
- provenance and auditability

### Space / Tool Registry

Track Spaces only when their capability is relevant to the architecture. MCP-enabled Spaces may be evaluated as tool surfaces but remain externally governed resources.

## Separation from canonical source

```text
External research
      ↓
Reference
      ↓
Evaluation
      ↓
Adapter / contract
      ↓
NEXUS implementation
```

Never:

```text
External fork
      ↓
Rename
      ↓
Claim as canonical
```

## Publication boundary

The current connected Hugging Face integration is suitable for discovery and inspection. If future project artifacts need to be published there, use an explicitly authorized write-capable connection and a separate publication review.
