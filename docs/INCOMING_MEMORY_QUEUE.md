# Incoming Memory Queue

This queue is the controlled landing zone for material arriving from other Living System conversations, repositories, uploads, or model work.

## Intake contract

Every incoming block receives a stable record ID, observed timestamp, source repository/conversation/file, exact path where applicable, commit SHA when GitHub-backed, Git blob SHA when available, SHA-256 when the raw artifact can be hashed, ISO/BEAT verification fields when those project-specific checks are supplied, sector classification, lineage target, and promotion state.

### Statuses

`INCOMING` → `CORRELATED` → `VERIFIED` → `ELIGIBLE` → `PROMOTED`

A record can instead become `REJECTED` without deleting the source artifact.

## Current queue

### LS-MEM-20260815-GEMMA-001

**Name:** Gemma Resonance Gambit  
**Reported by:** Architect  
**Status:** `INCOMING`  
**Expected sector:** AI Gateway / Resonance / Memory Verification  
**Expected target:** `NEXUS_CORE` implementation with protocol-level contract in `NEXUS_Protocol`  
**Required evidence:** exact GitHub repository, commit SHA, changed path(s), Git blob SHA, and raw-artifact SHA-256.

Current GitHub search has not positively identified the exact named Gambit. Do not substitute the unrelated public `machackabook/gemma` repository or the confirmed `machackabook/GMNINEXUS` repository merely because their names are related.

### LS-MEM-20260815-META-AI-001

**Name:** Meta-AI convergence material  
**Status:** `INCOMING`  
**Expected sector:** AI Gateway / Council / Orchestration  
**Required evidence:** source chat or repository artifact plus provenance hash.

### LS-MEM-20260815-CHAT-001+

Additional project-chat exports should be appended as individual records. The archive should preserve original chronology and never silently merge two records simply because their concepts overlap.

## Promotion rule

A memory block becomes canonical only when its evidence record identifies **what it is, where it came from, which exact object was observed, and how its integrity was checked**.
