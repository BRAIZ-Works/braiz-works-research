# BRAIZ Works Research

BRAIZ Works Research is the public research and technical-report library of BRAIZ Works LLC.

**Repository visibility:** public.

This repository publishes public-safe whitepapers, citation metadata, versioned release artifacts, reader-facing material, and integrity evidence while preserving a strict boundary around proprietary implementation details, private evidence, credentials, internal prompts, and reconstruction-sensitive architecture.

## Whitepaper library

The canonical paper locations are:

1. **[WP-01 — Verified Completion for Agentic AI](WP-01-verified-completion-for-agentic-ai/paper.md)**
2. **[WP-02 — The Enterprise Execution Gap](WP-02-enterprise-execution-gap/paper.md)**
3. **[WP-03 — Evidence-First AI Operations](WP-03-evidence-first-ai-operations/paper.md)**
4. **[WP-04 — Safe Change Without Proof Collapse](WP-04-safe-change-without-proof-collapse/paper.md)**
5. **[WP-05 — Producer Assurance vs Independent QA](WP-05-producer-assurance-vs-independent-qa/paper.md)**
6. **[WP-06 — Quality-Normalized AI Compression](WP-06-quality-normalized-ai-compression/paper.md)**
7. **[WP-07 — The Shadow-State Problem in Enterprise AI](WP-07-shadow-state-problem-in-enterprise-ai/paper.md)**
8. **[WP-08 — Recovery Is Part of Completion](WP-08-recovery-is-part-of-completion/paper.md)**
9. **[WP-09 — Public Case Study Series: From Intake to Verified Outcome](WP-09-public-case-study-series/paper.md)**
10. **[WP-10 — What Enterprises Should Demand From Agentic AI Systems](WP-10-enterprise-controls-for-agentic-ai/BRAIZ_Works_Research_WP-10_What_Enterprises_Should_Demand_From_Agentic_AI_Systems_v1.0.0.pdf)**

WP-01 through WP-09 link to their canonical Markdown paper. WP-10 currently links to its canonical PDF because no `paper.md` is present in that paper directory.

## Repository structure

Each current whitepaper lives in one top-level `WP-XX-...` directory. The former duplicate `papers/WP-02-enterprise-execution-gap/` path has been retired from the live tree; the canonical WP-02 location is:

`WP-02-enterprise-execution-gap/`

Versioned WP-02 v1.0.0 manifests and checksum projections are preserved unchanged as historical release evidence. They describe the exact repository/release state they were created against and are not current-tree manifests.

## Publication model

Repository source and formal versioned releases are distinct surfaces. Released paper files are not silently replaced; material corrections use successor versions. Public artifacts exclude credentials, private owner/admin evidence, internal prompts, protected implementation mechanics, and reconstruction-sensitive materials.

The repository-level release index is maintained under `releases/release-index.json`.

## Reader-facing site

The `site/` directory contains the reader-facing web projection. WP-02 has a dedicated rendered reader page; the library landing page links to the canonical public artifacts for the full WP-01 through WP-10 series.

## Rights

© 2026 BRAIZ Works LLC. All rights reserved. See `RIGHTS.md`.
