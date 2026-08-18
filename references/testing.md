# Testing Reference

## Validation Ladder

Use the strongest applicable validation available:

1. static inspection
2. formatter
3. type checking
4. linting
5. unit tests
6. integration tests
7. build/package validation
8. browser/E2E tests
9. runtime smoke test
10. regression review

## Failure Loop

Never hide a failing test. Isolate the cause, fix it, and rerun the relevant checks.

## UI Testing

Verify small and large screens, touch, keyboard, focus order, loading, empty and error states, reduced motion, overflow and long content.

## Test Quality

Prefer behavioral tests over implementation-detail tests. Add regression coverage for bugs likely to return.
