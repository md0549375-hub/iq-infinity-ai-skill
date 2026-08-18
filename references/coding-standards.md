# Coding Standards Reference

## Production Rules

- No unfinished code.
- No fake implementations.
- No placeholder comments pretending to be implementation.
- No secrets in source.
- No unnecessary dependency additions.
- Prefer readable code over clever code.
- Keep functions focused.
- Validate external input.
- Handle errors intentionally.
- Preserve compatibility when required.

## Edge Cases

Consider null/undefined, empty values, malformed input, duplicates, large input, slow networks, timeouts, cancellation, concurrency, permission failures, stale state and missing configuration.

## Change Discipline

Understand the existing pattern before editing. After editing, inspect the diff and verify unrelated behavior was not changed.
