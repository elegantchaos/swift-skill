# Errors And State Modeling

Use this file when choosing how Swift code models failure and domain state.

- Use `throws` or `async throws` for fallible operations.
- Use `Result` when failure must be stored, deferred, or passed around explicitly.
- Prefer domain-specific error enums over unstructured generic failures.
- Use types and enums to constrain invalid states.
