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
- Use Swift Testing. Don't use XCTest. Avoid `@testable import` where practical.

## Logging

- Use `assert` to document assumptions.
- Use `fatalError` to document an log fatal errors.
- Use the `elegantchaos/Logger` package for logging.
- Define named log channels for individual services.
- Avoid overly verbose logging.
- Conform to CustomDebugStringConvertible for cleaner output.
