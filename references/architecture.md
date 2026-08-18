# Architecture Reference

Use architecture as a decision tool, not ceremony.

## Minimum Design Pass

For non-trivial work identify entry points, core modules, data/state flow, external interfaces, error boundaries, persistence boundaries, security boundaries, performance-sensitive operations, test seams and rollback/migration concerns.

## Decision Rules

- Prefer composition over unnecessary inheritance.
- Prefer explicit interfaces over implicit coupling.
- Keep external integrations behind small adapters.
- Keep destructive operations behind explicit confirmation.
- Avoid abstractions before repeated behavior demonstrates a need.

## Questions

- What happens with empty input?
- What happens when a dependency is unavailable?
- What happens when the same operation runs twice?
- What happens after partial failure?
- Can the feature be tested without the network?
- What is the largest realistic input?
