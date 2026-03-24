# File And Type Organization

Use this file when shaping Swift source files and type boundaries.

- Prefer one primary type per file.
- Name files after the type (`MyType.swift`).
- Use focused extension files for distinct responsibilities (`MyType+Functionality.swift`).
- For protocol-conformance files, use `MyType+ProtocolName.swift`.
- Use PascalCase file names.

In each Swift file, prefer this order:

1. imports
2. log channels (if any)
3. main type definition
4. helper types/extensions
5. `#Preview` at the bottom for SwiftUI view files

## Type organization

For classes/structs, prefer this order:

1. stored properties
2. initializers
3. computed properties
4. public methods
5. private methods (often in private extensions)

For enums, prefer:

1. cases
2. static constants/factories
3. computed properties

For protocols, prefer:

1. properties
2. methods

## Documentation comments

- Add `///` documentation comments to all types and members, including private members.
- If necessary, a blank line above a `///` comment to separate it from the previous definition.
- Explain intent/behavior, not just the symbol name.
- Add inline comments only where intent is not obvious.
