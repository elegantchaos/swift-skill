# Swift Language Guidance

Use this file for baseline Swift coding conventions that are not owned by a specialist framework skill.

- Prefer Swift-native APIs and modern language features.
- Prefer Swift concurrency (`Task`, `await`, actors) for new code.
- Prefer static member lookup where it improves readability.
- Mark classes `final` unless inheritance is intentional.
- Avoid force unwraps and `try!` except in genuinely unrecoverable paths.
- Use value semantics by default unless reference semantics are required.
- Keep visibility tight (`private` by default, `public` only when necessary).
- Avoid private single-line wrappers unless they add clear value.

## Logging

- Use `assert` to document assumptions.
- Use `fatalError` to document/log unrecoverable errors.
- Avoid overly verbose logging.
- Conform types to CustomDebugStringConvertible for cleaner logging code.
- When the `elegantchaos/Logger` package is in the dependencies:
  - Use it for logging.
  - Define named log channels for individual services.
