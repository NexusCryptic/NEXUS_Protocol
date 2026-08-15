<!--
Copyright © 2026 CrypticNews LLC. All rights reserved.
This provenance header does not replace the repository's applicable license.
-->

# Living System Sector Registry

This registry converts the recurring project architecture into reviewable sectors. A sector is a responsibility boundary, not a separate product by default.

## 01 — Protocol / Nexus Protocol

**Function:** contracts, schemas, lifecycle, interoperability, versioning.

**Primary repository:** `NexusCryptic/NEXUS_Protocol`

**Artifacts:** protocol schemas, module contracts, event definitions, compatibility rules, governance rules.

## 02 — Kernel / OmniKernel⁹

**Function:** module lifecycle, scheduling, runtime state, watchdogs, portability.

**Primary repository:** `NexusCryptic/NEXUS_CORE`

**Target structure:**

```text
kernel/
  boot/
  scheduler/
  module-loader/
  eventbus/
  memory/
  graph/
  telemetry/
  watchdog/
  governance/
```

## 03 — Memory Fabric

**Function:** persistent artifact identity, relationships, retrieval metadata, snapshots, evolution history.

**Primary support repository:** `NexusCryptic/The-Ledger`

**Artifact classes:** conversations, code, HTML, images, research notes, decisions, datasets, models, builds, telemetry, repository references.

## 04 — Cartographer

**Function:** repository/project topology, dependency relationships, compatibility clusters, convergence density, lineage.

**Outputs:** repository graph, sector map, branch map, artifact map, duplicate detection, migration candidates.

## 05 — Dream Engine / Synthesis

**Function:** decompose intent into components, map dependencies, construct artifacts, validate, reflect, and produce a traceable result.

**Governance:** generated output is proposed work until reviewed.

## 06 — Runtime / PWA / Desktop

**Function:** host the Living System interface, multi-window workspace, event mesh, local persistence, renderer adapters.

**Existing design lineage:** Infinity Canvas, browser runtime, BroadcastChannel mesh, service-worker/PWA concepts.

## 07 — Planetarium / Visualization

**Function:** turn the topology graph into a navigable visual workspace with node inspection and telemetry.

**Artifact classes:** graph views, orbital maps, node inspectors, runtime dashboards.

## 08 — AI Gateway / Council

**Function:** provider-neutral routing between model providers and local tools.

**Known project integrations:** Gemini CLI, OpenAI/Codex concepts, Ollama/local models, MCP-oriented routing.

**Rule:** provider credentials remain external to the repository.

## 09 — Storybook / Narrative Workspace

**Function:** persistent narrative/context representation for project worlds and user-facing exploration.

**Boundary:** narrative material is an artifact class; it does not become a privileged execution mechanism.

## 10 — Signal / Fourier / Telemetry

**Function:** stream ingestion, FFT/spectrum analysis, event generation, peak tracking, recorder/ledger integration.

**Artifact classes:** spectrum snapshots, signal metadata, derived events, analyzer configurations.

## 11 — Infrastructure / Recovery

**Function:** device inventory, PXE/recovery workflows, network topology, portable deployment.

**Boundary:** destructive operations require explicit human confirmation and are never encoded as automatic defaults.

## 12 — Research / Hugging Face

**Function:** models, datasets, Spaces, papers, and technical references that support the architecture.

**Current connected account:** `machackabook`.

**Current permission boundary:** read-oriented Hub access; this connection is suitable for discovery/inspection, not for silently publishing project artifacts to Hugging Face.

## 13 — Governance / Audit

**Function:** provenance, review state, permissions, change records, release gates, secret scanning, license checks.

**Canonical evidence surface:** `NexusCryptic/The-Ledger`.

## Artifact lifecycle

```text
SOURCE
  ↓
IDENTIFY
  ↓
CLASSIFY
  ↓
HASH / PROVENANCE
  ↓
SECTOR ASSIGNMENT
  ↓
DEPENDENCY MAP
  ↓
NORMALIZE
  ↓
REVIEW
  ↓
CONVERGE
  ↓
RELEASE
```

## Required metadata

Every promoted artifact should carry:

- stable artifact ID
- source repository
- source path or external reference
- source commit/version when available
- creation/import timestamp
- artifact type
- sector
- license/provenance status
- secret-scan status
- transformation status
- reviewer/review state
- destination path

## Prohibited from the corpus

Do not commit:

- API keys
- OAuth tokens
- passwords
- private signing keys
- recovery codes
- unredacted personal addresses
- credential inventories
- secrets copied from local configuration files

The project can document that such resources exist without publishing their values.
