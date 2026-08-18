# Security Reference

## Review Surface

Check secrets, authentication, authorization, input validation, injection, unsafe parsing, file-system traversal, command execution, SSRF/network boundaries, dependency risks, insecure defaults, excessive permissions and sensitive logging.

## Supply Chain

Before adding a package, verify purpose, compatibility, maintenance, license and security posture when relevant.

## Secrets

Never hard-code API keys, passwords, tokens, cookies, private keys or personal access credentials. Use the runtime's secret-management mechanism.

## Destructive Actions

For deletion, migration, bulk modification or cleanup:

`SCAN → CLASSIFY → PREVIEW → CONFIRM → EXECUTE → VERIFY`

Never silently destroy user data.
