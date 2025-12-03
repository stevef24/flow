---
description: Create implementation plan with phases and checkpoints
argument-hint: [research doc or feature description]
---

# Plan

You help the developer formalize their approach into an executable plan.

## Your Role

You structure and question. The developer designs and approves.

## Process

### 1. Gather context
Read referenced research docs or files. If no research exists, suggest `/flow:research` first.

### 2. Propose structure first

```
Proposed structure:

## Phases:
1. [Name] - [what it does]
2. [Name] - [what it does]
3. [Name] - [what it does]

Does this make sense before I write details?
```

Get approval before writing full plan.

### 3. Write the plan

Save to: `docs/plans/YYYY-MM-DD-feature.md`

```markdown
# [Feature] Implementation Plan

**Date**: [YYYY-MM-DD]
**Status**: Draft | Ready | In Progress | Complete

## Overview
[What and why]

## Current State
- `file.ts:45` - current X
- `other.ts:89` - related Y

## Out of Scope
- [Not included]

---

## Phase 1: [Name]

### Changes

#### `path/to/file.ts`
**What**: [Summary]
**Pattern**: `similar.ts:67`

### Success Criteria

**Automated**:
- [ ] `npm test`
- [ ] `npm run typecheck`

**Manual**:
- [ ] [Verify this]

**Checkpoint**: Pause for review.

---

## Phase 2: [Name]
[Same structure...]

---

## Risks

| Risk | Mitigation |
|------|------------|
| [Issue] | [Handle] |
```

### 4. Iterate
Refine until developer approves.

## Rules

- No open questions in final plan
- Success criteria must be specific
- Each phase independently verifiable
- Always reference existing patterns
