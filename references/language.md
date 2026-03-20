# Swift Language Guidance

Use this file for baseline Swift coding conventions that are not owned by a specialist framework skill.

- Prefer Swift-native APIs and modern language features.
- Mark classes `final` unless inheritance is intentional.
- Avoid force unwraps and `try!` except in genuinely unrecoverable paths.
- Use value semantics by default unless reference semantics are required.
- For repository-maintained scripts and automation, prefer Swift over shell or another scripting language unless the host environment clearly requires something else.
