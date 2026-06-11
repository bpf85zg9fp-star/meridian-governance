---
document_id: "GUIDE-GITHUB-MERIDIAN-SETUP-001"
title: "Meridian GitHub Repository Setup & Activation Guide"
version: "1.3"
status: "Approved by Kevin Slade"
classification: "Operational Guide"
date: "2026-06-11"
author: "Kevin Slade"
drafter: "ChatGPT"
stage_2_reviewer: "Claude (Anthropic)"
stage_3_reviewer: "Gemini"
stage_4_consolidator: "Grok"
final_approval: "Kevin Slade"
programme: "Meridian"
related_documents:
  - "RFQ-0003 v0.1 — GitHub Repository and Source Control Standard (Under Review)"
  - "RIP-003A v0.3 — Multi-Model Review and Governance Pipeline Standard"
  - "ADR-003 (pending amendment) or ADR-004 (Grok Consolidator-Adjudicator)"
  - "DISCUSSION-GITHUB-N8N-SETUP-001 (pending formal ID)"
  - "Master Checklist (pending formal ID)"
purpose: >
  Provide a single, explicit, step-by-step procedure for establishing,
  validating, and activating the Meridian GitHub repository and AI review
  ecosystem.
success_criteria:
  - "GitHub repository created and access secured."
  - "Repository structure established (provisional pending RFQ-0003)."
  - "Governance documents stored and version controlled."
  - "AI review pipeline roles documented per binding Meridian governance (RIP-003A v0.3)."
  - "n8n automation operational with Kevin Slade approval gate confirmed."
  - "Meridian documentation process repeatable and traceable."
  - "Kevin Slade final approval obtained before repository is declared operational."
changelog:
  - version: "1.3"
    date: "2026-06-11"
    stage: "Stage 4 Consolidation"
    consolidator: "Grok"
    summary: "Aligned AI review sequence and workflow diagram exactly to RIP-003A v0.3."
  - version: "1.1"
    date: "2026-06-11"
    stage: "Stage 2 Critical Review"
    reviewer: "Claude (Anthropic)"
    summary: "Corrected pipeline roles, added Kevin approval gate, flagged structure as provisional."
---
# Meridian GitHub Repository Setup & Activation Guide

## Current Situation

The programme currently has multiple draft governance documents, defined AI review roles (per RIP-003A v0.3), but no operational repository or single source of truth. This guide establishes the repository as the highest priority task.

## Phase 1 — Freeze New Document Creation

**Objective:** Halt all new governance artefact creation until the repository is operational.

**Actions:**
- Do not draft additional policies.
- Do not redesign the review process.
- Perform only repository establishment activities.

**Completion Criteria:** Repository creation is the sole active workstream.

## Phase 2 — Create GitHub Account Structure

1. Sign into GitHub.
2. Enable 2FA, passkey support, and recovery methods.
3. Create repository:
   - **Name:** `meridian-governance`
   - **Description:** Governance, RFQs, AI review artefacts and operational documentation for Meridian.
   - **Visibility:** Private
   - Initialise with README.md and .gitignore

## Phase 3 — Build Repository Structure (Provisional)

> **PROVISIONAL** — Pending approval of RFQ-0003.

meridian-governance/ ├── README.md ├── CHANGELOG.md ├── GOVERNANCE/ ├── RFQ/ ├── POLICIES/ ├── REVIEW_PIPELINE/ ├── MASTER_CHECKLISTS/ ├── TEMPLATES/ ├── DECISIONS/ ├── ARCHIVE/ └── AUTOMATION/

## Phase 4 — Populate Repository

Place documents in appropriate folders.

## Phase 5 — AI Review Pipeline Roles (per RIP-003A v0.3)

| Step | Participant          | Function                          |
|------|----------------------|-----------------------------------|
| 1    | Kevin Slade          | Instruction                       |
| 2    | ChatGPT              | Drafting                          |
| 3    | Claude (Anthropic)   | Independent Review (parallel)     |
| 4    | Gemini               | Independent Review (parallel)     |
| 5    | Grok                 | Consolidation and Adjudication    |
| 6    | Kevin Slade          | Final Approval (mandatory)        |

## Phase 6 — Version Control Discipline

1. Archive previous version.
2. Increment version number.
3. Update CHANGELOG.md.

## Phase 7 — n8n Automation

**Workflow:**

Kevin Instruction → ChatGPT Draft → (Claude + Gemini parallel) → Grok Consolidation → Kevin Final Approval → GitHub Commit

## Phase 8 — Definition of Done

- [x] GitHub repository created
- [x] Provisional folder structure established
- [x] Core files added
- [x] GUIDE-GITHUB-MERIDIAN-SETUP-001 v1.3 approved by Kevin Slade

**Guiding Principle:** Meridian needs a reliable system more than more documents.

*End of GUIDE-GITHUB-MERIDIAN-SETUP-001 v1.3 — Approved by Kevin Slade on 2026-06-11*