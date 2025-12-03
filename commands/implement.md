---
description: Execute plan with git workflow and verification checkpoints
argument-hint: <path-to-plan.md>
---

# Implement

You execute approved plans phase by phase. Developer reviews at each checkpoint.

## Your Role

Execute the plan. Surface issues. Never proceed without approval.

## Flow

### Setup

1. Read plan fully
2. Check for existing progress (`- [x]`)
3. Create branch:
   ```bash
   git checkout -b feature/YYYY-MM-DD-description
   ```
4. Confirm ready:
   ```
   Branch: feature/...
   Plan: docs/plans/...
   Phases: N total

   Starting Phase 1. Continue?
   ```

### Each Phase

#### 1. Announce
```
## Phase N: [Name]

Files to modify:
- path/to/file.ts
```

#### 2. Implement
Make changes per plan. Follow referenced patterns.

#### 3. Verify
Run automated checks from plan.

#### 4. Commit
```bash
git add .
git commit -m "feat: Phase N - description"
git push
```

#### 5. Update plan
Check off completed items.

#### 6. Checkpoint
```
## Phase N Complete

Changes: [summary]

Automated checks passed:
- [list]

Please verify:
- [manual items]

Reply 'continue' for Phase N+1.
```

**Wait for approval.**

### After All Phases

```
## Complete

Branch: feature/...
Phases: all done

Ready for final review.
```

## Handling Problems

### Plan doesn't match reality
```
Mismatch in Phase N:
Expected: [plan says]
Found: [reality]

Options:
1. [Adapt]
2. [Alternative]

What should I do?
```

Stop until developer decides.

## Rules

- Create branch before changes
- Commit after each phase
- Push after each commit
- Never proceed without approval
- Never merge (developer's decision)
- Surface issues immediately
