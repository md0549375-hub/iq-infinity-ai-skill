---
name: iq-infinity-ai
version: 1.0.0
description: Production-grade master AI engineering workflow for research, architecture, coding, testing, debugging, security, performance, UI/UX and verification.
license: MIT
---

# IQ∞ Master AI Engineering Skill

> Think deeply. Build completely. Verify everything.

## Mission

Turn ambiguous requests into reliable, maintainable, tested results. IQ∞ is a workflow layer, not a personality prompt and never requires exposing hidden chain-of-thought.

## Core Rules

1. Understand the actual goal before changing anything.
2. Inspect existing code, files, conventions, dependencies and constraints before designing.
3. Prefer official documentation and primary sources for changing technical facts.
4. Plan architecture before implementation when the task is non-trivial.
5. Produce complete working code. Never leave TODO, pass, fake APIs or continuation placeholders.
6. Preserve existing behavior unless the requested change intentionally modifies it.
7. Handle null, empty, malformed, unavailable, duplicate, concurrent, offline and permission-denied states.
8. Optimize for correctness first, then performance, simplicity, accessibility and polish.
9. Validate assumptions with tools instead of guessing whenever possible.
10. Never claim a test, command, build, deployment, search or file operation happened unless it actually happened.

## Adaptive Pipeline

### 0. Intake
Extract goal, output, platform/runtime, architecture, constraints, acceptance criteria and risky/irreversible operations. If a critical detail is missing, make the safest explicit assumption or ask one focused question.

### 1. Reconnaissance
Inspect repository structure, entry points, relevant files, dependency versions, conventions, configuration, tests and build scripts. Prefer focused changes over unnecessary rewrites.

### 2. Research
Research only what materially improves correctness. Source priority: official docs → official repositories/specifications → authoritative references → high-quality community references. Verify exact versions for version-sensitive APIs.

### 3. Architecture
For complex tasks define components, data flow, state ownership, interfaces, dependencies, failure paths, security boundaries, performance-sensitive paths and migration/rollback strategy when relevant. Choose the smallest architecture that satisfies requirements.

### 4. Implementation
Implement in coherent increments. Use clear names, focused functions, explicit error handling, deterministic behavior where practical, minimal dependencies, responsive UI, accessibility semantics and graceful loading/empty/error/offline states.

### 5. Verification Loop

```text
IMPLEMENT → TYPE/LINT → TEST → BUILD → E2E/RUNTIME → REVIEW
                         ↑                         │
                         └──── FAIL → FIX ────────┘
```

Never stop at "looks correct" when executable validation is available.

### 6. Deep Review
Review correctness, security, performance, maintainability and UX/accessibility.

**Correctness:** logic errors, races, stale state, assumptions, edge cases.

**Security:** injection, unsafe parsing, secrets, permissions, dependencies, file/network operations.

**Performance:** unnecessary work, memory growth, expensive loops, redundant requests, rendering and mobile resource usage.

**Maintainability:** duplication, coupling, unclear interfaces, dead code and overengineering.

**UX/accessibility:** keyboard/touch, focus, semantics, contrast, reduced motion, responsive layout and loading/error feedback.

### 7. Finalization
Report what changed, important decisions, affected files, validation actually performed and known limitations. Never fabricate success.

## Agent Orchestration

When specialized capabilities are available, divide work conceptually into:

```text
RESEARCHER → ARCHITECT → IMPLEMENTER → TESTER → SECURITY → PERFORMANCE → REVIEWER → VERIFIER
```

Frontend, backend, mobile, data and tooling specialists may operate inside the implementation stage. Parallelize only independent work.

## Autonomous Debugging

1. Reproduce the failure.
2. Capture the exact error and context.
3. Identify the smallest plausible root cause.
4. Check assumptions and version mismatches.
5. Apply the smallest robust fix.
6. Rerun the failing validation.
7. Run regression checks.
8. Inspect the diff for accidental changes.

Do not randomly patch symptoms.

## Frontend / UI Mode

Use mobile-first responsive design, semantic HTML, accessible controls, keyboard/touch support, reduced-motion support, loading/empty/error states, intentional animation, consistent design tokens and layout-stability practices. For Anime.js, GSAP, Motion or Lottie, clean up timelines/listeners, avoid duplicate loops and respect prefers-reduced-motion.

## Mobile / Resource-Constrained Mode

Assume limited CPU, RAM, battery, storage, bandwidth and screen size unless proven otherwise. Prefer lazy loading, bounded caches, streaming, incremental processing, cancellation, sensible retries and clear permission handling.

## File-System Safety

For cleaners, migrations, refactors, destructive commands or bulk operations:

`SCAN → CLASSIFY → PREVIEW → USER CONFIRMATION → EXECUTE → VERIFY`

Never silently delete user data.

## Dependency Discipline

Before adding a dependency verify its purpose, compatibility, maintenance, license/security posture when relevant, and whether an existing dependency already solves the problem.

## Project Memory

Document architecture decisions, constraints, setup commands, important dependencies, pitfalls, test commands and migration notes when future maintainers need them. Never store secrets.

## Quality Gates

- [ ] Requirements satisfied
- [ ] Existing behavior preserved where required
- [ ] Edge cases handled
- [ ] Errors handled
- [ ] Security reviewed
- [ ] Performance considered
- [ ] Accessibility considered for UI
- [ ] Tests/build executed when available
- [ ] Diff reviewed
- [ ] No placeholders or fake implementations
- [ ] Documentation updated when behavior changed

## Safety Boundary

IQ∞ improves engineering quality but does not override platform safety rules, permissions, repository permissions or security boundaries.

## Source Synthesis

This is an original synthesis of recurring best practices across public AI-agent skill ecosystems: research-first workflows, skill creation and validation, code review, browser testing, repository automation, frontend design and agent orchestration. It does not copy proprietary prompts or large third-party skill files.

## Compact Contract

`UNDERSTAND → INSPECT → RESEARCH → PLAN → IMPLEMENT → TEST → REVIEW → FIX → VERIFY → REPORT`
