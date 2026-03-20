# File And Type Organization

Use this file when shaping Swift source files and type boundaries.

- Prefer one primary type per file.
- Name files after the primary type.
- Use focused extension files for distinct responsibilities.
- Keep visibility tight and broaden access only when needed.

Suggested member order for a primary type:

1. stored properties
2. initializers
3. computed properties
4. public or internal methods
5. private helpers
