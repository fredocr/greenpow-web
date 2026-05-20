# Agent Structure Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add an agent-friendly repository structure with an RND bucket and clear promotion rules.

**Architecture:** Keep approved website source content in `context/`, agent workflow instructions in `agent/`, exploratory work in `rnd/`, accepted decisions in `docs/decisions/`, and implementation handoffs in `docs/implementation/`. Add Superpowers spec and plan records under `docs/superpowers/`.

**Tech Stack:** Markdown documentation in the existing Git repository.

---

### Task 1: Add Agent Workflow Documentation

**Files:**
- Create: `agent/operating-model.md`
- Create: `agent/build-sequence.md`
- Create: `agent/content-parity-checklist.md`
- Create: `agent/replit-instructions.md`
- Create: `agent/evolution-log.md`

- [x] **Step 1: Create agent documentation files**

Create focused Markdown files that explain agent priorities, build sequence, bilingual content parity, Replit-specific startup instructions, and workflow evolution.

- [x] **Step 2: Verify responsibilities are distinct**

Confirm `agent/operating-model.md` describes how agents choose sources, `agent/build-sequence.md` describes build order, and `agent/content-parity-checklist.md` describes bilingual page checks.

### Task 2: Add RND Bucket

**Files:**
- Create: `rnd/README.md`
- Create: `rnd/hypotheses.md`
- Create: `rnd/roadmap-ideas.md`
- Create: `rnd/mysx-research.md`
- Create: `rnd/cortex-research.md`
- Create: `rnd/carbon-data-sources.md`
- Create: `rnd/competitor-notes.md`
- Create: `rnd/experiments.md`

- [x] **Step 1: Create RND documentation files**

Create research files for hypotheses, roadmap ideas, MySx, Cortex, carbon data sources, competitors, and experiments.

- [x] **Step 2: Add promotion guardrails**

State that RND content must be promoted into `context/`, `PROJECT_BRIEF.md`, or `docs/decisions/` before production use.

### Task 3: Add Decision And Implementation Docs

**Files:**
- Create: `docs/decisions/2026-05-20-agent-repo-structure.md`
- Create: `docs/implementation/2026-05-20-next-build-handoff.md`

- [x] **Step 1: Record the structure decision**

Document why the repository separates `context/`, `agent/`, `rnd/`, `docs/decisions/`, and `docs/implementation/`.

- [x] **Step 2: Record the next build handoff**

Document that the next milestone is the Next.js app foundation with bilingual route parity and content loading.

### Task 4: Update Top-Level Guidance

**Files:**
- Modify: `README.md`
- Modify: `AGENTS.md`
- Modify: `PROJECT_BRIEF.md`

- [x] **Step 1: Update README**

Point future agents to `PROJECT_BRIEF.md`, `AGENTS.md`, `agent/`, `context/`, and `rnd/`.

- [x] **Step 2: Update AGENTS**

Add source-priority and RND handling rules.

- [x] **Step 3: Update PROJECT_BRIEF**

Add the repository structure model and RND bucket rule.

### Task 5: Verify And Commit

**Files:**
- All files above.

- [x] **Step 1: Verify file list**

Run: `find agent rnd docs -maxdepth 3 -type f | sort`

Expected: all new documentation files are listed.

- [x] **Step 2: Scan for unfinished markers**

Run a repository-wide search for unfinished marker words such as task-marker labels, fix-marker labels, filler labels, and sample Latin filler text.

Expected: no matches.

- [x] **Step 3: Review git diff**

Run: `git diff --stat`

Expected: documentation-only changes in approved folders and top-level guidance.

- [ ] **Step 4: Commit and push**

Run:

```bash
git add README.md AGENTS.md PROJECT_BRIEF.md agent rnd docs
git commit -m "docs: add agent workflow and rnd structure"
git push
```
