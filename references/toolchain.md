# Toolchain And Platform Expectations

Use this file when deciding which Swift language and platform conventions should apply.

- Target the latest Swift for new projects (see https://www.swift.org/install/)
- Target the latest system for Apple-focussed projects (see https://developer.apple.com/platforms/)
- Target Swift 6 language mode for new projects.
- Always prefer Swift 6+ modern idioms when possible.
- Do not assume all targets in a multi-target workspace use identical build settings; verify toolchain and deployment expectations before applying broad migrations.

## Legacy Projects

- Follow the project's current Swift and platform targets.
- Implement changes in a migration-friendly style.

If an existing project or target is using Swift 5 language mode:

- Migrate to Swift 6 if trivial, otherwise suggest a migration path.
- Implement new code with Swift 6 migration in mind.
- Prefer modern concurrency-safe patterns where practical.
- Consider splitting code into multiple packages to ease migration.
- Default UI-facing types to `@MainActor` when it improves correctness; explicitly justify non-main-actor types.
